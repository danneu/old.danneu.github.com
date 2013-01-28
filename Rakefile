require "rake"
require "yaml"
config = YAML.load_file("_config.yml")

desc "Generate the site"
task :build do
  system "jekyll --no-server --no-auto"
end

desc "Deploy to git repository"
task :deploy, :message do |t, args|
  message = args[:message]
  branch = config["git"]["branch"]
  raise "Specify commit message." if message.nil or message.empty?
  raise "Specify config['git']['branch']" if branch.nil? or branch.empty?
  Rake::Task[:build].invoke
  system "git add ."
  system "git commit -am '#{message}'"
  system "git push origin #{branch}"
end

desc "Build and deploy site. (Run from source branch)"
task :builddeploy, :message do |t, args|
  message = args[:message]
  branch = config["git"]["branch"]
  raise "Specify commit message." if message.nil? or message.empty?
  raise "Specify config['git']['branch']" if branch.nil? or branch.empty?
  Rake::Task[:build].invoke
  system "git checkout master"
  system "git rm -qr ."
  system "cp -r _site/. ."
  system "rm -r _site"
  system "git add -A"
  system "git commit -m '#{message}'"
  system "git push origin master"
end

##namespace :assets do
##  task :precompile do
##    puts `bundle exec jekyll build`
##  end
##end
require "jekyll"
require "tmpdir"
require "rubygems"

# Auto publish

# Change your GitHub reponame
GITHUB_REPONAME = "julymaker/julymaker.github.io"


desc "Generate blog files"
task :generate do
  Jekyll::Site.new(Jekyll.configuration({
    "source"      => ".",
    "destination" => "_site"
  })).process
end

desc "Generate and publish blog to gh-pages"
task :publish => [:generate] do
  Dir.mktmpdir do |tmp|
    cp_r "_site/.", tmp

    pwd = Dir.pwd
    Dir.chdir tmp

    system "git init"
    system "git config --local user.name JulyMaker"
    system "git config --local user.email julio.martin.saez@gmail.com"
    system "git add ."
	  message = "Site updated at #{Time.now.utc}"
	  system "git commit -m #{message.inspect}"
    system "git remote add origin https://github.com/#{GITHUB_REPONAME}.git"
    system "git push origin master --force"

    Dir.chdir pwd
  end
end


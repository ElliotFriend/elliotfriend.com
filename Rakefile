#!/usr/bin/env ruby

require 'html-proofer'

desc "clean"
task :clean do
  if Dir.exists?('_site') then
    rm_rf '_site'
  end
end

desc "build the site"
task :build do
  sh "bundle exec jekyll build"
end

desc "Check the quality of the HTML output"
task :proof do
  options = { :assume_extension => true,
              :verbose => true,
              :check_html => true,
              :check_favicon => true,
              :check_external_hash => true }
  HTMLProofer.check_directory("./_site", options).run
end

desc "Default task is to clean, build, and proof"
task :default => [ :clean, :build, :proof ] do
  puts "Task complete"
end

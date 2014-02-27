# encoding: utf-8

require 'bundler'
Bundler.require

desc 'Build our app to build.js'
task :build do
  env = Opal::Environment.new
  env.append_path 'assets/javascripts'

  File.open('./build/javascripts/application.js', 'w+') do |out|
    out << env['application'].to_s
  end
end

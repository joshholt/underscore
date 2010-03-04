require 'rubygems'
require 'closure-compiler'

desc "Use the Closure Compiler to compress Underscore.js"
task :build do
  js  = File.open('./lib/underscore.js', 'r')
  min = Closure::Compiler.new.compile(js)
  File.open('./lib/underscore-min.js', 'w') {|f| f.write(min) }
end


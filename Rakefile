# -*- ruby -*-

require "rubygems"
require "hoe"
require './lib/amf/version.rb'

Hoe.plugin :gemspec
Hoe.plugin :minitest
Hoe.plugin :yard
Hoe.plugin :bundler
Hoe.plugin :git
Hoe.plugin :ignore

Hoe.spec "amf" do
  developer("RobertLongIV", "RobertLongIV@example.com")
  developer("So Awesome Man", "callme@1800AWESO.ME")

  license "Apache 2.0" # this matches the license in the LICENSE file

  self.email                = 'callme@1800AWESO.ME'

  self.name                 = 'amf-ruby'
  self.version              = AMF::VERSION
  self.summary              = 'Ruby Gem for serializing and deserializing AMF'
  self.description          = self.summary
  self.urls                 = ['https://github.com/awesome/amf-ruby']
  self.testlib              = :minitest
  self.readme_file          = 'README.md'
  self.history_file         = 'History.txt'

  # third-party
  self.yard_title           = self.name
  self.yard_markup          = 'markdown'

  self.extra_dev_deps += [
    ["hoe-yard",                  "~> 0.1"],
    ["hoe-ignore",                "~> 1.0"],
    ["hoe-bundler",               "~> 1.2"],
    ["hoe-gemspec",               "~> 1.0"],
    ["hoe-git",                   "~> 1.6"],
    ["minitest",                  "~> 5.9"],
    ["yard",                      "~> 0.8"],
    ["redcarpet",                 "~> 3.3"] # yard/markdown
  ]

  self.clean_globs += [
    '.yardoc',
    'vendor',
    'Gemfile.lock',
    '.bundle',
  ]

  self.spec_extras = {
    :required_ruby_version => '>= 1.9.2'
  }
end

# # require rake tasks
# current_dir = File.expand_path(File.dirname(__FILE__))
# Dir.glob(File.join(current_dir, 'lib/tasks/*.rake')).each {|r| import r} 

# vim: syntax=ruby

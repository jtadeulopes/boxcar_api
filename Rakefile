require 'rubygems'
require 'rake'
require 'echoe'

require 'rspec/core/rake_task'

RSpec::Core::RakeTask.new :spec do |t|
  t.rspec_opts = %w(-fp --color)
end

Echoe.new('boxcar_api', '1.0.1') do |p|
  p.description    = "A simple way to send notifications to yourself, or your users through Boxcar."
  p.url            = "http://github.com/boxcar/boxcar_api"
  p.author         = "Jonathan George"
  p.email          = "help@boxcar.io"
  p.ignore_pattern = ["tmp/*", "script/*"]
  p.development_dependencies = ["httparty"]
  p.runtime_dependencies = ["httparty"]
end

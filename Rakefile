require 'rake'

require 'puppet-lint/tasks/puppet-lint'
PuppetLint.configuration.send('disable_autoloader_layout')

require 'rspec/core/rake_task'

RSpec::Core::RakeTask.new(:spec) do |t|
  t.pattern = 'spec/*/*_spec.rb'
end

task :default => [:spec, :lint]

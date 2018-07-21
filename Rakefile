task :default => [:mkdir, :report]

require 'rspec/core/rake_task'
task :report do
  `tj3 -o reports Umzug.tjp`
end

task :mkdir do
  Dir.mkdir 'reports'
end

task :default => [:mkdir, :report]

OUTPUTDIR = "reports"

require 'rspec/core/rake_task'
task :report do
  Kernel.system "tj3 -o #{OUTPUTDIR} Umzug.tjp"
end

task :mkdir do
  unless Dir.exist? OUTPUTDIR
    Dir.mkdir OUTPUTDIR
  end
end

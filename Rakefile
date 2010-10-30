
desc "Run rspec" 
task :spec do
  require "rspec/core/rake_task"

  RSpec::Core::RakeTask.new do |t|
    t.rspec_opts = %w(-fs -c)
  end
end

desc "Build the gem"
task :gem do
  sh 'gem build *.gemspec'
end

desc "Synonym for spec"
task :test => :spec
desc "Synonym for spec"
task :tests => :spec

desc "Synonym for gem"
task :pkg => :gem
desc "Synonym for gem"
task :package => :gem
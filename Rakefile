namespace :greeting do

desc 'outputs hello to the terminal'
task :hello do
  puts "hello from Rake!"
end

desc 'outputs hello to the terminal'
task :hola do
  puts "hola de Rake!"
end


end

desc 'console mah bonsole'

task :console do
  binding.pry
end


namespace :db do

  desc 'migrates a table'
  task :migrate => :environment do
    Student.create_table
  end

  desc 'seeds a table'
  task :seed do
    require_relative './db/seeds.rb'
  end
end
task :environment do
  require_relative './config/environment'
end

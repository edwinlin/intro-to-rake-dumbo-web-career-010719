desc 'outputs hello to the terminal'
task :hello do
  puts "hello from Rake!"
end

namespace :greeting do 
	desc 'puts out hello from Rake!'
	task :hello do
	  puts 'hello from Rake!'
	end

	desc 'puts out hola from Rake!'
	task :hola do
	  puts 'hola de Rake!'
	end
end

task :console do	
end

namespace :db do
  desc 'migrate changes to your database'
  task :migrate => :environment do
    Student.create_table
  end

  desc 'seed the database with some dummy data'
  task :seed do
    require_relative './db/seeds.rb'
  end

end

task :environment do
  require_relative './config/environment'
end


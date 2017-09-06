namespace :greeting do
  desc 'says hello'
  task :hello do
    puts 'hello from Rake!'
  end
  task :hola do
    puts 'hola de Rake!'
  end

end



namespace :db do
  task :environment do
    require_relative './config/environment'
  end
  desc 'migrate changes to your database'
  task :migrate => :environment do # => creates dependency
    Student.create_table
  end
  desc 'seed database with dummy info'
  task :seed do
    require_relative './db/seeds.rb'
  end
end

# desc 'seed database with dummy data'
#   task :seed do
#     require_relative .db/seeds.rb
#   end
# end

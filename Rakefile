require "bundler/gem_tasks"
require_relative "lib/notepasser/init_db"

desc "Run migrations"
namespace :db do
  task :migrate do
    version = ENV["VERSION"] ? ENV["VERSION"].to_i : nil
    ActiveRecord::Migrator.migrate('db/migrate', version)
  end
end

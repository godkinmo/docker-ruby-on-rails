# README

This README would normally document whatever steps are necessary to get the
application up and running.

Things you may want to cover:

* Ruby version

* System dependencies

* Configuration

* Database creation

* Database initialization

* How to run the test suite

* Services (job queues, cache servers, search engines, etc.)

* Deployment instructions

## Create Rails Project
./develop rails new . --skip-test-unit

# Pass-thru to `docker-compose ps`
./develop 

# call `docker-compose ps` ourselves
./develop ps 

# Start our containers
./develop up -d

# Stop our containers
./develop down

# Fancier commands - list our the working directory
# from our application container ("app" service)
./develop run --rm -w /code app ls -lah

# If we add another gem, all we need to do is, update both Gemfile in `docker/app/Gemfile` and `Gemfile`:
cd docker
./build

# Debug rails not startup
./develop run --rm -w /code app rails server

* ...

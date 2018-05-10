# README

This is a simple project to show you how to use Docker ans Ruby on Rails

* Install [Docker](https://docs.docker.com/install/)
* Install [docker-compose](https://docs.docker.com/compose/install/)
* Clone this repository `git clone https://github.com/leogomezzz/docker_ruby.git`
* Create this folder ../volumes/db_data with 777 permissions (it's not the best, but it'll work for now)
`cd docker_ruby && mkdir -p ../volumes/db_data && chmod 777 -R ../volumes`
* run `docker-compose up` on terminal

* In other terminal, run `docker ps`, copy the ID of noteapp_web container and run `docker exec -it ID bash`, like `docker exec -it 2e532e8129ed bash`

* Run `rake db:migrate`

* In your browser, access [http://localhost/notes](http://localhost/notes)

* To access your database administration tool, use [http://localhost:8080](http://localhost:8080) and use the credentials below:
	* server: db
	* username: appuser (or root)
	* password: password

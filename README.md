<p> # springBootAPI </p>

``Docker Postgres``
<h5>https://hub.docker.com/_/postgres </h5>

``docker pull postgres:alpine`` => for get image from dockerhub

``docker run --name postgres-spring -e POSTGRES_PASSWORD=password -d -p 5432:5432 postgres:alpine``

``docker ps`` => for showing images -> `d5db3bb590c0`

``docker port postgres-spring``
- 5432/tcp -> 0.0.0.0:5432

``docker exec -it d5db3bb590c0 bin/bash``  => into postgresql image containerized

- ``psql -U postgres`` => where "postgres is the user"
- ``\l`` => to see dbs
- ``CREATE DATABASE demodb;``
- ``\c demodb`` => access to demodb
- ``\d`` ``\dt`` => relations? (d: everything - dt: tables)
- ````

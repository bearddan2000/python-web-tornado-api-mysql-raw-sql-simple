# python-web-tornado-api-mysql-raw-sql-simple

## Description
Simple web app that serves an api
for a tornado project.

Uses sqlalchemy and raw sql to query a table `dog`.

Remotely tested with *testify*.

## Tech stack
- python
  - tornado
  - sqlalchemy
  - testify
  - requests
- mysql

## Docker stack
- python:latest
- mariadb:latest

## To run
`sudo ./install.sh -u`
- Get all dogs: http://localhost/dog
  - Schema id, breed, and color
- CRUD opperations
  - Create: curl -i -X PUT localhost/dog/<id>
  - Read: http://localhost/dog/<id>
  - Update: curl -i -X POST localhost/dog/<id>/<breed>/<color>
  - Delete: curl -i -X DELETE localhost/dog/<id>

## To stop
`sudo ./install.sh -d`

## For help
`sudo ./install.sh -h`

## Credit
- [HTTPServer config](https://phrase.com/blog/posts/tornado-web-framework-i18n/)
- [Code based on](https://www.tornadoweb.org/en/stable/)
- [Sqlalchemy code](https://medium.com/swlh/tornado-and-sqlalchemy-847eecbc0445)
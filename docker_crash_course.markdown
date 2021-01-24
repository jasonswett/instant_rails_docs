---
layout: page
title: Docker Crash Course
permalink: /docker-crash-course/
---

If you haven't used Docker much before, it might be unclear how to develop on a Dockerized Rails application.

There are two main Docker commands that will be helpful for you to be familiar with: `docker-compose run` and `docker-compose up`.

## docker-compose up

`docker-compose up` looks at all the services specified in your project's `docker-compose.yml` and starts them.
If you're used to running `rails server` to spin up a Rails server, you'll do `docker-compose up` instead on a Dockerized project.

In the case of Instant Rails, those services include a Rails web service, a PostgreSQL service, a Redis service and a Webpacker service.
Running `docker-compose up` will run all these services.

Note that when you first [generate an Instant Rails app](/getting-started), `docker-compose up` is run automatically for you.

## docker-compose run

In a Dockerized application, all commands need to be prefixed with `docker-compose run <container name> <command>` in order for the command to be run inside
a container rather than on the host machine.

For example, to run a migration, do:

```bash
docker-compose run web rails db:migrate
```

Or, to open a Rails console, run:

```bash
docker-compose run web rails console
```

I like to alias `docker-compose run web` to something like `drw` so I can run e.g. `drw rails db:migrate` instead of the longer version.

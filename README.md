# dev-java-cli-maven-postgres-liquibase-view

## Description
Creates a small database table
called `dog`. This table, `dog`, has been normalized to 3NF.
Two new tables have been added, `breedLookup` and `colorLookup`.
Creates a new table `dog_expanded` that joins
`dog`, `breedLookup` and `colorLookup`. Added clustered indexes on
`dog`.breedId and `dog`.colorId and a non-clustered index for
`dog_expanded`.id. Turned `dog_expanded` into a view with an
implicit index on `dog_expanded`.id. All output normally
seen in a terminal will be in `java-srv/log` which will dump to the screen. The project may seem to hang but the logs from the container must be written to the project this can take up to 3 min.

Uses liquibase migration tool to augment
the schema.

## Tech stack
- java
- liquibase
- maven
  - log4j
  - mysql driver

## Docker stack
- maven:3-openjdk-17
- mariadb:latest
- webdevops/liquibase:mysql

## To run
`sudo ./install.sh -u`
Creates java-srv/log

## To stop
`sudo ./install.sh -d`
Removes java-srv/log

## For help
`sudo ./install.sh -h`

## Credit
- [Java code based on](https://github.com/htorun/dbtableprinter)

## dev-java specific search
- [Search by cli](https://github.com/bearddan2000?tab=repositories&q=dev-java-cli&type=&language=&sort=)
- [Search by maven](https://github.com/bearddan2000?tab=repositories&q=dev-java-maven&type=&language=&sort=)
- [Search by postgres](https://github.com/bearddan2000?tab=repositories&q=dev-java-postgres&type=&language=&sort=)
- [Search by liquibase](https://github.com/bearddan2000?tab=repositories&q=dev-java-liquibase&type=&language=&sort=)
- [Search by view](https://github.com/bearddan2000?tab=repositories&q=dev-java-view&type=&language=&sort=)
- [Search by log4j](https://github.com/bearddan2000?tab=repositories&q=dev-java-log4j&type=&language=&sort=)
- [Search by mysql](https://github.com/bearddan2000?tab=repositories&q=dev-java-mysql&type=&language=&sort=)
- [Search by driver](https://github.com/bearddan2000?tab=repositories&q=dev-java-driver&type=&language=&sort=)

## General search
- [Search by dev](https://github.com/bearddan2000?tab=repositories&q=dev&type=&language=&sort=)
- [Search by java](https://github.com/bearddan2000?tab=repositories&q=java&type=&language=&sort=)
- [Search by cli](https://github.com/bearddan2000?tab=repositories&q=cli&type=&language=&sort=)
- [Search by maven](https://github.com/bearddan2000?tab=repositories&q=maven&type=&language=&sort=)
- [Search by postgres](https://github.com/bearddan2000?tab=repositories&q=postgres&type=&language=&sort=)
- [Search by liquibase](https://github.com/bearddan2000?tab=repositories&q=liquibase&type=&language=&sort=)
- [Search by view](https://github.com/bearddan2000?tab=repositories&q=view&type=&language=&sort=)
- [Search by log4j](https://github.com/bearddan2000?tab=repositories&q=log4j&type=&language=&sort=)
- [Search by mysql](https://github.com/bearddan2000?tab=repositories&q=mysql&type=&language=&sort=)
- [Search by driver](https://github.com/bearddan2000?tab=repositories&q=driver&type=&language=&sort=)

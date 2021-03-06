# Wildlife-Tracker

A Java and spark web-app that aids wildlife rangers in recording of animals sightings. The animals sighted could be either classified as endangered or not.

## Description

The Forest Service is considering a proposal from a timber company to clearcut a nearby forest of Douglas Fir. Before this proposal may be approved, they must complete an environmental impact study. This application was developed to allow Rangers to track wildlife sightings in the area.

An app that aims at tracking the wildlife numbers. Rangers are able to spot animals, both endangered and non-endangered then record them in a sightings record.

## Installation

##### Technologies Used
- Java
- Spark
- JUnit
- Velocity Template Engine
- PSQL

##### Setup

To use the code, you can clone the repository at: [https://github.com/YomZsamora/Wildlife-Tracker](https://github.com/YomZsamora/Wildlife-Tracker).
* `$ git clone https://github.com/YomZsamora/Wildlife-Tracker.git`
* `$ cd wildlife-tracker` 
* `$ gradle run`
* Go to localhost:4567 in your browser

##### Database Instructions (postgres/psql)
* Run in terminal: `postgres`
* Run in new terminal window: `psql`
* Run in psql: `CREATE DATABASE wildlife_tracker;`
* Run in psql: `CREATE TABLE animals (id serial PRIMARY KEY, animal_name varchar, endangered varchar, animal_health varchar, animal_age varchar);`
* Run in psql: `CREATE TABLE sightings (id serial PRIMARY KEY, animal_id int, location varchar, ranger_name varchar, timestamp timestamp);`
* Run in psql: `\connect wildlife_tracker`



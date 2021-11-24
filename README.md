# Sparkify Data Modelling and ETL using Apache Cassandra

## Motivation

The startup, Sparkify, is a music streaming app and wants to analyse what songs their users are listening to. Their current data is available as local CSV files and cannot be easily analised. The purpose of the ETL process is to create a tables for fast queries with an Apache Cassandra database.

## Data model

A denormalized dataset was created to match the three specific queries that needed to be executed:

1. Give the artist, song title and song's length that was heard during a specific sessionId and itemInSession
2. Give the artist, song (sorted by itemInSession) and user (first and last name) for a specific userid and sessionid
3. Give every user name (first and last) who listened to a specific the song

## File descriptions

- `import-to-cassandra.ipynb`: Imports individual CSV files, create Cassandra database, create tables and insert data into tables, and finally drop tables.

## How to run the files and notebooks

Dependencies and virtual environment details are located in the `Pipfile` which can be used with `pipenv`.

## License

GNU GPL v3

## Author

Coenraad Pretorius

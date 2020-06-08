# Data-Modelling-with-apache-cassandra
______________________________________________

## Introduction

### Project: Data Modeling with Cassandra
A startup called Sparkify wants to analyze the data they've been collecting on songs and user activity on their new music streaming app. The analysis team is particularly interested in understanding what songs users are listening to. Currently, there is no easy way to query the data to generate the results, since the data reside in a directory of CSV files on user activity on the app.

They'd like a data engineer to create an Apache Cassandra database which can create queries on song play data to answer the questions, and wish to bring you on the project. Your role is to create a database for this analysis.
Project Steps
Below are steps you can follow to complete each component of this project.

## INFO
Apache Cassandra is an open source NOSQL database built with a masterclass architecture and linear scalability. 
NOSQL database can store larger amount of data than relational databases.

### Project Steps:
1.Design tables to answer the queries outlined in the project template
2. Write Apache Cassandra CREATE KEYSPACE and SET KEYSPACE statements
3. Develop your CREATE statement for each of the tables to address each question
4. Load the data with INSERT statement for each of the tables
5. Include IF NOT EXISTS clauses in your CREATE statements to create tables only if the tables do not already exist.
5. Test by running the proper select statements with the correct WHERE clause

Since Data Modelling in Apache Cassandra follows the one table one query rule, Different tables were created to suit different queries

 Tables include
 1. Song_library with partition as sessionId and clustering column as itemInSession
 2. Song_library_by_user with partition as user_id and clustering column as itemInSession and sessionId
 3. song_library_by_song with partiton as song and clustering column as userId
 
 NOTE! 
 To validate our data and output, I used both the SQL queries and Pandas queries to see if my reuslts match and they did
 

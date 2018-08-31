REST API for News System with comments



1. Structure of the application

NewsSystemApplication - Main class of the application, implements CommandLineRunner interface that allows add some information to database as a test

Package rest
AppREStController - The controller allows displaying information depending on what address you choose and adding information to the database

package config
DatabaseConfiguration - This  class contains the configuration of the connection to the mongoDB database.

package domain
Commnet, News - The classes are a reflection of the table in the mongoDB database

package repository
CommentRepository, NewsRepository - Interfaces enabling operations on the Comment and News tables in the database

package service
CommentService, NewsService - The services allow operations on data in the database using repositories
ServiceInterface - Common interface for services enabling operations on the database
CustomInterfaceComment - additional custom interface allowing other operations (findByNewsId)



2. Aditional infos

Application created using Spring framework 
The application uses mongoDB.
(Firstly I created the database locally but I wanted to connect the application to the database I created in AWS.

The basic structure of the project generated at start.spring.io.

Used Gradle mechanism for resolving dependencies

Application validates information that can be sent to the database (See classes Comment and News in domain package)



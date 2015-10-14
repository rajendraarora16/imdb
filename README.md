# imdb
IMDB(Internet movie database management)

**WIKI:**
IMDb is now the world's most popular and authoritative source for movie, TV and celebrity content. It offers a searchable database of more than 100 million data items including more than 2 million movies, TV and entertainment programs and more than 4 million cast and crew members.

Visit here: http://www.imdb.com/

As per the request, I've created the similar project. 


To see demo, Visit here:

**[DEMO][1]**
-------------
-------------

Create table into your database:

    create database `imdb`;
    use `imdb`;
    
    create table if not exists `imdb_table`
    (
    userId INT NOT null auto_increment,
    userName VARCHAR(100) not null,
    userEmail VARCHAR(100) not null,
    userPassword VARCHAR(100) not null,
    userJoinDate VARCHAR(100) not null,
    PRIMARY KEY(userId));
    
    create table if not exists `verifyAccount`
    (
    id INT NOT NULL auto_increment,
    userEmail VARCHAR(100) not null,
    verification VARCHAR(100) not null,
    passCode VARCHAR(100) not null,
    PRIMARY KEY(id));
    
    
    create table if not exists `forgetPassword`
    (
    id INT NOT NULL auto_increment,
    userEmail VARCHAR(100) not null,
    passCode VARCHAR(100) not null,
    PRIMARY KEY(id));
    
    create table if not exists `newsArticle`
    (
    id INT NOT NULL auto_increment,
    newsURL VARCHAR(100) not null,
    userName VARCHAR(100) not null,
    userEmail VARCHAR(100) not null,
    title VARCHAR(1000) not null,
    article text(100000) not null,
    articleDate VARCHAR(100) not null,
    PRIMARY KEY(id));
    
    create table if not exists `movies`
    (
    id int not null auto_increment,
    movieURL VARCHAR(100) not null,
    userName VARCHAR(100) not null,
    userEmail VARCHAR(100) not null,
    movieName VARCHAR(100) not null,
    imgURL VARCHAR(100) not null,
    actName VARCHAR(100) not null,
    releasingDate VARCHAR(100) not null,
    directorName VARCHAR(100) not null,
    producerName VARCHAR(100) not null,
    writerName VARCHAR(100) not null,
    screenplayName VARCHAR(100) not null,
    starringName VARCHAR(100) not null,
    musicName VARCHAR(100) not null,
    productionName VARCHAR(100) not null,
    distributorName VARCHAR(100) not null,
    runningTime VARCHAR(100) not null,
    country VARCHAR(100) not null,
    language VARCHAR(100) not null,
    budget VARCHAR(100) not null,
    boxofficeName VARCHAR(100) not null,
    discription VARCHAR(1000) not null,
    PRIMARY KEY(id)
    );
    
    create table if not exists `Bio`
    (
    id int not null auto_increment,
    bioURL VARCHAR(100) not null,
    userName VARCHAR(100) not null,
    userEmail VARCHAR(100) not null,
    fullName VARCHAR(100) not null,
    imgURL VARCHAR(100) not null,
    born VARCHAR(100) not null,
    residence VARCHAR(100) not null,
    occupation VARCHAR(100) not null,
    yearsActive VARCHAR(100) not null,
    religion VARCHAR(100) not null,
    relatives VARCHAR(100) not null,
    discription VARCHAR(1000) not null,
    PRIMARY KEY(id)
    );


**If any query comes, Kindly drop at contact.rajendraarora@gmail.com**







  [1]: http://imdbdemo-imdbdemo.rhcloud.com/

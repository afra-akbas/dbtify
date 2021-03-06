<img align="right" src="https://user-images.githubusercontent.com/32341138/87282744-3d27a600-c4fd-11ea-8a98-449f22a9b9d7.png">

# DBtify

This is the third project of Cmpe321 Introduction to Database Systems. For the other projects of this course, you can visit [Cmpe321](https://github.com/afra-akbas/cmpe321) repository.

## Project Description
In this project, I implemented a simple song management platform,
called DBtify, with a web-based user interface. There are listeners, songs, albums,
and artists in the platform. These entities have the following properties:

• Listener: Username and e-mail. They are both unique which means there exists
only one listener with a specific username and e-mail address.

• Artist: Name and surname. They are not necessarily unique independently but
we can assume there exists only one artist with a name and surname couple.

• Album: ID, genre, and title. By definition, each ID is unique. Each album must
contain at least one song.

• Song: ID and title. By definition, each ID is unique. Each song must reside in
only one album. Each song may be produced by one or multiple artists.

Two types of people are using DBtify: Listeners and artists. Since we do not have to, I did not
implement an authentication mechanism. I am allowed to provide two options for
being a listener or an artist. The person can choose what he/she is and cannot perform
other type of person’s operations.

## Requirements
My UI must support the following operations:

• Artists shall be able to add/update/delete albums.

• Artists shall be able to add/update/delete songs in the albums.

• Listeners shall be able to separately view all songs, albums, and artists in DBtify.

• Listeners shall be able to view all songs and albums of an artist.

• Listeners shall be able to view all songs of an album.

• Listeners shall be able to like songs and albums.

• Listeners shall be able to view other listeners’ liked songs as well as his/her liked
songs.

• Listeners shall be able to view popular songs (according to number of likes) of an
artist.

• Listeners shall be able to rank all artists by the total number of likes of their songs.

• Listeners shall be able to view songs of a specific genre.

• Listeners shall be able to search a keyword and view the songs that contain this
keyword in their titles.

• Listeners shall be able to view the artists who produced a song together. This must
be implemented as a stored procedure. Parameters of this procedure are the
artist’s name and surname.

• The system shall have three triggers:
1. When an album is deleted, all the songs in this album must also be deleted.
2. When a song is deleted, it must be removed from listeners’ likes.
3. When a listener likes an album, all the songs of this album must also be liked
by that listener.

## For Installation
WE NEED TO RUN 'npm i' in order to install nodejs packages.

     npm i

#### BACKEND: 
THEN TO RUN BACKEND 'node app.js' 

     node app.js

#### FRONTEND:
MY FRONTEND CODE IN 'client/' path. Build file is in 'client/build'. When we run the backend, build file servers as a static file. I develop with React js. 


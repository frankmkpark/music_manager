
/** 
Note to grader: 
This README file work as a quick instruction for our application.
Our final report provide more detail
**/


Files included in our submission:

1. TanYParkMLiC_dump.sql: This is a self-contained schema file that includes tables, data, and stored procedures. 
2.TanYParkMLiC_app.py: This Python file contains the access point for the application
3. Final Report__TanYParkMLiC.pdf : This is the final report for our database project.

Installation Process & Library requirement:

1. Import and create the database in the user's local MySQL host server using the provided dump file: TanYParkMLiC_dump.sql. This is a self-contained file with the CREATE command. In the local MySQL server, go to "Server > Data Import > Import from Self-Contained File > Start Import." After importing, the database named “musify” should appear on the user’s local server. Verify that the database contains tables, data within each table, and stored procedures.

2. The application code is written in Python and uses the PyMySQL library to connect to the MySQL Server. To run this application code, the user must have a compatible Python version (3.7 or above) and install the PyMySQL library package using the pip command before starting the application.

3. The application code also requires the user to install Pandas and Matplotlib library. We use these two libraries to do the data visualization work.

4. After installing the database and all the Python libraries mentioned above, the user can run the application code in any IDE that supports the Python language.

How to use the application:

The user will be prompted to enter the local server username (default is 'root') and password. This application assumes the user uses localhost for the connection. A message, "You have successfully connected to the database," indicates a successful connection. If the connection fails, an "Error connecting to the database" message will appear. Remember, both input fields for username and password are case-sensitive.

After the user connects to the database, we provide a menu for the user. The user can choose to log in to the existing music account, create a new account, update the password associated with the current account, or close the connection with the database. In our database, we initially stored eight users and their passwords. For grading purposes, we shared all the user names and their passwords in our report, or grader can check our database users table. Graders can choose to create a new account to test our “C” operation, update the password to test our “U” operation, or log into the existing account below to test more operations. 

After the user logs into their music account, we provide a menu for the user to perform the below tasks: manage playlists, explore music, view band distribution graph, view album release year distribution graph, discover interesting facts, and log out.
Manage Playlists - The user can create a new playlist, update the current playlist name, delete a playlist associated with his/her account, insert a song into the playlist, delete a song from the playlist, or exit the current menu. Please note that all input box is case sensitive.

Explore Music - This function allows the user to explore the music in our database. The user can find the song by band name, album name, genre type, and song name or exit the current menu. Please note that all input box is case sensitive.

View Band Distribution Graph - Here, we provide the user an opportunity to quickly learn the music in our database through a graph of the bands’ founded years.

View Album Release Year Distribution Graph - Here, we provide the user an opportunity to quickly learn the music in our database through a graph of the albums’ release year.

Discover interesting facts - Here, we provide the user another opportunity to learn about our database by listing four fun facts: the top five albums with the longest playtime, a list of bands with their latest album, the top five most popular genres by the number of songs, top five most active users by the number of reviews.

Log out of your music account - This option allows the user to log out of the account and back to the last menu where the user can choose to log in to the music account again, create a new account, update the password for their current account, or close the connection with the database.

Finally, You need to choose "close connection" option to close the connection with database. We doing this extra step is provide a "fake" log-in experience to our user.



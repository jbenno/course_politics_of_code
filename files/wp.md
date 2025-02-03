<sup>|[&uarr; Back to course home page](/README.md)</sup>  
# Installing and Running a Wordpress Blog

Statistics on the share of Wordpress in websites: [https://w3techs.com](https://w3techs.com/)

#### Prerequisites
- FTP client (e.g. FileZilla https://filezilla-project.org or CyberDuck https://cyberduck.io/)
- Webspace with FTP access (read/write/execute) and PHP 7.x running
- sql database on the webspace
- 
#### Webspace
You can use the domains, webspace, ftp-server and database I will provide in class where X is a number assigned to you:  
  [Google Spreadsheet with the necessary info](https://docs.google.com/spreadsheets/d/118Fu6Br2QPHFbI8Zc8nGP0wuzAbDL70zWBIL62IieTw/edit?usp=sharing)  
URL `http://cX.f3c.me`  (eg. c1.f3c.me, c2.f3c.me, etc.)  
ftp `ftp.cX.f3c.me`  

#### Installation
1. Download the current Wordpress distribution at https://wordpress.org/download/
If you download the compressed file `wordpress-x.x.x.tar` or `wordpress-x.x.x.zip` you have to decompress it after downloading it. It will unpack into a folder `wordpress`.
2. Transfer (upload) all files and subfolders inside the `/wordpress` folder to your webspace. Do not upload the folder itself, grab everything inside of it and dump it into the webspace. Use `ftp.cX.f3c.me` (`X` being your assigned number), login and password as provided. Make sure you are using `FTP` and not `SFTP`. 
3. Open the url `http://cX.f3c.me` in your browser (`X` being your assigned number).  
  Select the language.  
  Populate the form. Fill in the database name, username, (**database name and username should be the same**) and password as provided in the Google Spreadsheet. Don't change the field 'host' - it stays with localhost.  
  -> In the field 'Table Prefix' fill in your unique prefix. IMPORTANT: Do not use 'wp_' - change it. Your new prefix should look like: `1_` or `2_` or `3_`, etc. 
  Then continue.
  Populate the next form - chose a name like wp_admin for the user name; more users can be added later.  
  Generally you should chose an email address that you don't need to work with on this blog later. The administrater email should be seperate from the users.
  **Copy the password because it will not be displayed later.**
  Log in with the admin user name and the copied password.
  In the Menu go to `users` and add yourself as a user. Set the field `Role` to `Administrator` - otherwise you will not be able to do much.
  Log out, and log in with your user name and password.
  The web user interface you are working in is called `dashboard` and can be accessed under the URL `http://cX.f3c.me/wp_admin`.
  
#### SQL Database
https://w008f8b5.kasserver.com/mysqladmin/kaslogin.php
  
#### Themes
- The "themes" are administrated in the dashboard under the menu item `Appearence`.
- The files for the themes are located in the folder `/wp-content/themes`.
- To install new themes you can upload the theme's files to a new folder under /wp-content/themes

[Here we have a closer look on how the theme scripts work](/files/wp/README.md)


***

<sup>|[&uarr; Back to course home page](/README.md)</sup>  
  
<sup>NYU Abu Dhabi ***[Politics of Code](/README.md)*** by [Joerg Blumtritt](https://jbenno.net) [@jbenno](https://twitter.com/jbenno) - Other classes I teach: [github.com/jbenno](https://github.com/jbenno/teaching/blob/master/README.md)</sup>


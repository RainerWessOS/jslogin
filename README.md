# jslogin

jslogin - A secure javascript login script - no userids or passwords are stored in the script.

How to use: Copy this file into a folder on your webspace, make a  subdirectory user were the individual private websites for the users are stored. For every user you allow to login, are two files nessesary. A little .gif-image and a website (.htm). Lets say you want a user "Paul" with the password "Asd613" to login.  Place a little .gif-image named Paul_Asd613.gif in the user directory.Which image doesnt matter, it will be shown nowhere, as small as posible. Then create a website Paul_Asd613.htm in the user directory. This is the website the user will see after he logged in.

How it works:
When a user tries to login the script tries to load an image {userid}_{password}.gif - if this is successful the userid and password are valid and the welcome-page for the user is loaded. If user/password are not valid  loading the image fails - In this case no website is loaded. The image is just there to prevent http 404 (file not found) error messages for nonexisting oder mistyped user/password - combinations, which would be the case if the private website would be directly loaded.
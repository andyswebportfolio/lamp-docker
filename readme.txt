  _                                _            _             
 | |                              | |          | |            
 | | __ _ _ __ ___  _ __ ______ __| | ___   ___| | _____ _ __ 
 | |/ _` | '_ ` _ \| '_ \______/ _` |/ _ \ / __| |/ / _ \ '__|
 | | (_| | | | | | | |_) |    | (_| | (_) | (__|   <  __/ |   
 |_|\__,_|_| |_| |_| .__/      \__,_|\___/ \___|_|\_\___|_|   
                   | |                                        
                   |_|                                        

#####
Installing

Use this.

mkdir lamp-docker;
cd lamp-docker;
mkdir www;
cd www;
gh repo clone andyswebportfolio/lamp-docker;
cd lamp-docker;
rm -r -f .git;
git init;
cp -R . ../;
cd ../;
rm -r -f lamp-docker;
mv readme.txt ../


In english:

Make a lamp-docker folder,
Open it,
Make a www folder inside it,
Open that,
Clone lamp-docker itself,
open it,
delete git,
make a new git (break the connection to lamp-docker), 
copy it out of the lamp-docker folder, 
delete the lamp-docker folder.
Move the readme up a level.

,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,
Usage:

# Navigate to the folder in Terminal
# Start Docker itself
# Run Docker Compose in Terminal
# Use: docker-compose up -d 
(use of -d to detach allows you to continue to use the terminal)

# When finished:
# Stop the containers with
# docker stop $(docker ps -a -q)
# Close Docker program

# To View:
# Docker container ls

# Services
 - phpMyAdmin

http://localhost:8080 is for phpMyAdmin
User = root
Password = root_password (possible the same as SQL database(?)

# Web Root

http://localhost

,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,


#####
What?

A LAMP stack to be used with docker as a development environment.
A blank canvas to build on.

#####
Where?

Development environment. You'll want to set up a secure environment for production, either by checking and securing this one or creating another one elsewhere.

#####
How?

# Known Prerequisites:
# Docker Installed

# Pull from GitHub
# Delete the git file and the readme

Recommended:
# Update versions of the programs used in the Docker Compose File, or
# Update to new version of lamp-docker by pulling it as above, then:
# import your html, mysql_data and .git files respectively.

#####
Who?

The original tutorial for this build came from: https://medium.com/@mikez_dg/how-to-set-up-a-simple-lamp-server-with-docker-images-in-2023-9b0e24476ec6

The ASCII art is from: https://patorjk.com/software/taag/#p=display&f=Big&t=lamp-docker

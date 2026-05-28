# Dedicated-CS2-Modded-Server-Docker-ARRCON-and-SimpleAdmin-
Got this running with the help of a tutorial. Def recommend watching. 
https://www.youtube.com/watch?v=u1J1Kz1QWvQ&t=45s


# Description 
A fully containerized Counter-Strike 2 dedicated modded server with admin menu control.
This project provides a clean, reproducible environment using Docker, making it easy to deploy, update, and maintain a CS2 server on any machine.

# Features
Dockerized CS2 server : no manual installs or scattered files

Automatic updates : server pulls the latest CS2 build on start

Config persistence : store custom server configs outside the container

Port forwarding ready : works on local networks, cloud hosts, or home servers

Simple commands : start/stop/rebuild with one line


# Step 1: Enter SRCDS token
Go to the Steam community page: https://steamcommunity.com/dev/managegameservers

Enter 730 in slot 1 and any name you'd like in slot 2 for reference.
<img width="1081" height="355" alt="Screenshot 2026-05-27 195202" src="https://github.com/user-attachments/assets/b7b82b86-0675-40db-876f-3f16c15c7930" />

After that, you paste it in the SRCDS Token section in the Docker Compose file I had stored in my main CS2 data server file.

<img width="1895" height="1032" alt="image" src="https://github.com/user-attachments/assets/a6d1ab0c-5162-4b06-a01b-b2584cf4d581" />

# Step 2: Run the Docker Compose file in PowerShell Windows Terminal.
<img width="1815" height="560" alt="Screenshot 2026-05-27 211945" src="https://github.com/user-attachments/assets/918d5797-ffb6-40de-9359-0369af6da16e" />

Run the command 'ld' to make sure it's working, then you can do "docker compose up" to start and start the server. 

# Step 3: Installing Mods

First step is to install metamod, counterstrikeSharp, and SimpleAdmin as addon plugins to your CS2-data folder. It is best to follow the tutorial on YT for this step as trying to type it would just be confusing.
<img width="1122" height="300" alt="image" src="https://github.com/user-attachments/assets/4084e9ec-3e06-4153-817a-1131bda5517a" />

Next step was to install ARCOM and use css_addadmin command to get privileges to run the SimpleAdmin menu. 

<img width="1869" height="977" alt="canruncommands" src="https://github.com/user-attachments/assets/d4ab5266-ef15-4fde-96d0-a2a7acf37b46" />




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

# Links

Get SRCDS Token: https://steamcommunity.com/dev/manage...


Metamod: https://www.sourcemm.net/downloads.ph...

ARRCON: https://github.com/radj307/ARRCON

CounterStrikeSharp: https://github.com/roflmuffin/Counter...

SimpleAdmin: https://github.com/daffyyyy/CS2-Simpl...

Get your STEAMID64: https://steamid.io/lookup

SimpleAdmin Dependancies:
PlayerSettings: https://github.com/NickFox007/PlayerS...
AnyBase: https://github.com/NickFox007/AnyBase...
MenuManager: https://github.com/NickFox007/MenuMan...


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

Next step was to install ARCOM and use css_addadmin command to get privileges to run the SimpleAdmin menu. You needed a steamID64 key to get admin access and you can get that from this website: https://steamid.io/lookup
<img width="1853" height="898" alt="Screenshot 2026-05-27 221725" src="https://github.com/user-attachments/assets/315334db-0061-469c-9bb3-65de7ec1e52c" />


<img width="1869" height="977" alt="canruncommands" src="https://github.com/user-attachments/assets/d4ab5266-ef15-4fde-96d0-a2a7acf37b46" />

After copying the CS2-SimpleAdmin.json file and pasting it into my CS2 server folder, I was good to go. 

<img width="610" height="33" alt="image" src="https://github.com/user-attachments/assets/75bb3f4f-99f0-4069-8db6-bfbd8f563743" />

# Step 4: Testing the server 

Used the 'connect localhost' command to join, and it worked successfully. The only issues I had were not having admin privileges at first for SimpleAdmin, causing the menu not to load, but t his was fixed by making sure that my Steam64ID tag was right. This is an important step in the process, and I had it incorrect the first time. 

<img width="1919" height="1074" alt="Screenshot 2026-05-27 215708" src="https://github.com/user-attachments/assets/af4af596-4481-4e0c-9fd9-5c9ff03af62f" />

<img width="1909" height="1072" alt="Screenshot 2026-05-27 215755" src="https://github.com/user-attachments/assets/72511cba-bda3-4063-814d-758935e32634" />

<img width="1885" height="1034" alt="Screenshot 2026-05-27 221541" src="https://github.com/user-attachments/assets/1bf3ce76-bd79-46ab-ac02-6e5afd673dda" />

<img width="1903" height="343" alt="Screenshot 2026-05-27 215912" src="https://github.com/user-attachments/assets/43f31dbb-23c8-463a-9c6e-07b3142ccdf7" />

<img width="1848" height="1008" alt="final" src="https://github.com/user-attachments/assets/3136d3c6-1604-4687-a6dc-39ba14914555" />










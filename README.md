# RollerMadness

RollerMadness is a simple game which involves the player to collect the collectibles while trying to avoid collisions with the enemies at the same time. The game has two levels — Level1 and Level2 — both beatable.

## Components of the Game

1. __Player__ - The player is a sphere ball, namely RollerBall. It is destroyed either on collision with the enemy or on entering the DeathZone.<br>
<p align="center"><img src="https://github.com/pranshi112/RollerMadness/blob/main/images/rollerball.png" alt="rollerball" width="200"/></p>

2. __Enemy__ - The enemies are the cubes which spawn every 3 seconds and chase the player. They are destroyed on collision, either with the player or another enemy. <br>
<p align="center"><img src="https://github.com/pranshi112/RollerMadness/blob/main/images/enemy.png" alt="enemy" width="200"/></p>

3. __Collectibles__ - These include non-translating as well as bouncy coins. The bouncy coins spawn every second and are self-destructed after 10 seconds. For each coin collected, the player gets 1 point. <br>
<p align="center"><img src="https://github.com/pranshi112/RollerMadness/blob/main/images/coin.png" alt="coin" width="200"/></p>

4. __Obstacles__ - On collison with the obstacles, the GameObjects bounce off. <br>
<p align="center"><img src="https://github.com/pranshi112/RollerMadness/blob/main/images/bumper.png" alt="bumper" width="200"/></p>

5. __Floor__ - The entire area where the player is free to move. <br>
<p align="center"><img src="https://github.com/pranshi112/RollerMadness/blob/main/images/floor.png" alt="floor" width="200"/></p>

6. __DeathZone__ - The area around the floor, on entering which, the player dies. <br>
<p align="center"><img src="https://github.com/pranshi112/RollerMadness/blob/main/images/deathzone.png" alt="deathzone" width="200"/></p>

## How to Play

- Player movement can be controlled using either the arrow keys or the WSAD keys.
- The player must collect the minimum number of coins(either the non-translating or the bouncy ones) required to beat that level while trying to avoid any collision with the enemies or falling into the Death Zone simultaneously. If the latter happens, the player loses the level.
- Minimum score to beat:
  - Level1 = 5
  - Level2 = 10
- Beating Level1 takes the player to Level2. If not beated, the player gets an option to play Level1 again.
- In both cases - beating or losing Level2 - the player gets 2 options:
  - Play Level2 again.
  - Restart the game from Level1.

## Getting Started

The project is made on an Editor version 2019.4.16f1 and includes WebGL and Windows Build.

#### WebGL:
  
- In the project folder, navigate to Builds &#8594; WebGL &#8594; _index.html_. <br>
__Note__: Opening _index.html_ directly from the file system might not work in some browsers. This is due to security restrictions applied to local file URLs.
- In case none of your browsers support the first method, you may open the file by starting a local testing server. To start it:
  - Make sure you have __Python__ installed on your system.
  - Next, open the Command Prompt & navigate to the directory, WebGL where _index.html_ lies inside, using the `cd` command. 
  - Enter the command to start up the server in that directory:
  ```
  # If Python version is 3.X
  python -m http.server
  # If Python version is 2.X
  python -m SimpleHTTPServer
  ```
This will run the contents of the directory on a local web server, on port 8000. You can go to this server by going to the URL `localhost:8000` in any web browser. The HTML file would run now.

#### Windows:

In the project folder, navigate to Builds &#8594; Windows &#8594; _Roller Master.exe_.

#### Unity:

Open the project in Unity and navigate to File &#8594; Build And Run. This opens the application on your target platform specified in Unity.
__Note__: If your Editor version doesn't match with the project's, a warning message will be displayed asking you to download that version. Alternatively, download the required version in Unity Hub.


This is a short instruction to setup the littleServer to allow for connection of the littleBeast client.

1) Firstly clone both, the littleServer and littleBeast repo from these sources respectively.<br>
https://github.com/LittleBeasts/littleServer.git<br>
https://github.com/LittleBeasts/littleBeasts.git<br>

2) Then you can configure the server port in the littleServer in src.server.server
<p align="center">
  <img alt="ServerConfig" src="https://raw.githubusercontent.com/LittleBeasts/documentation/master/network/Images/serverConfig.png" width="600">
</p>


3) In the littleBeast game client you will need to input the correct IP-adress in src.main.java.client.client
<p align="center">
  <img alt="IP-config" src="https://raw.githubusercontent.com/LittleBeasts/documentation/master/network/Images/idadress.png" width="600">
</p>


4) Then start the server through running the server class in the littleServer project.

5) After that you can start up the client by running src.main.java.com.littleBeasts.Program.
In game you can start an online game.
<p align="center">
  <img alt="MainMenu" src="https://raw.githubusercontent.com/LittleBeasts/documentation/master/network/Images/mainMenu.png" width="800">
</p>


When the game can't connect to the server there will be an error in the console.<br>

6) To start a chat window just press the "return" key.

The project is built with a maven pom file. It could be that you will need to build the project before the first start up so all the needed libraries are installed.

For the project we used the openjdk-15 "15.0.1"


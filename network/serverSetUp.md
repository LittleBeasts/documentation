This is a short instruction to setup the littleServer to allow for connection of the littleBeast client.

1) Firstly clone both, the littleServer and littleBeast repo from these sources respectively.
https://github.com/LittleBeasts/littleServer.git
https://github.com/LittleBeasts/littleBeasts.git

2) Then you can configure the server port in the littleServer in src.server.server
IMAGE

3) In the littleBeast game client you will need to input the correct IP-adress in src.main.java.client.client
IMAGE

4) Then start the server through running the server class in the littleServer project.

5) After that you can start up the client by running src.main.java.com.littleBeasts.Program.
In game you can start an online game.
IMAGE

When the game can't connect to the server there will be an error in the console.

6) To start a chat window just press the "return" key.

The project is built with a maven pom file. I could be that you will need to build the project before the first start up so all the needed libraries are installed.

For the project wie used the openjdk-15 "15.0.1"


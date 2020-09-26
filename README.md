# Spark-websocket-chat

## About

Chat app created using the light-weight microservice framework "Spark Java". It internally uses Jetty and it's WebSocket capabilities.

This application can support more than concurrent 500 users, without data privacy concerns (as we don't log or store any message :D)

Set up a complete pipeline to deploy code to Heroku free tier VM's.

**Give a try with working demo of chat group** : https://websocket-spark-chat.herokuapp.com

## Want to run your own instance ?

_Prerequisite_ : Make sure you have Java 8+ and Maven installed. 

1. Clone this repo https://github.com/ayushwing/spark-websocket-chat.git
2. Open file websocket.js and change Websocket connection from wss to ws in Line 1 (If you do not have localhost https cert configured)
3. Open Terminal and build using Maven (mvn clean install Or mvn clean package)
4. After the build, you should have a target folder with a file as `websocketchat...-jar-with-dependencies.jar`
5. Navigate to this path and run `java -jar websocketchat-1.0.0-SNAPSHOT-jar-with-dependencies.jar`
6. The server will start default on `localhost:4567`. Open it in browser and Enjoy! :)  

## Screenshots of deployed app
Somehow (with google and stackoverflow) coded a decent responsive UI (not a FE guy)  

<div align="left">
    <img src="/doc/screenshot/welcome-screen.png" width="50%"</img> 
    <img src="/doc/screenshot/display-1.png" width="50%%"</img> 
    <img src="/doc/screenshot/display-2.png" width="50%"</img> 
    <img src="/doc/screenshot/display-3.png" width="50%"</img> 
    <img src="/doc/screenshot/display-3.png" width="50%"</img> 
    <img src="/doc/screenshot/inactivity.png" width="50%"</img> 
</div>
   

# Video Confrence App 
https://leetsmeet.herokuapp.com/ 

**How to use:**

* **As an End-user:**

     1- Firstly, register an account in the web app: https://leetsmeet.herokuapp.com/signup

     2- Login with the configration you signed up with in the app: https://leetsmeet.herokuapp.com/login

     3- After Logging you will have a choice to either join an on going meeting or Create a new Meeting.

     4- After creating a new meeting you will asked to allow mic and video to be able to interact with the others. 

     5- Then you will be in a the pre-viewing room and you will be asked to click on the green cell phone to enter the call room.
     
     6- Featuers() of the app 
 ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
* **As a Developer:**

    After downloading the zip file or clonning to the repository: 
    go to your terminal and run the following: 

    if you are using a Vscode go to server.js right click on the file -> open integrated terminal. 

    first thing copy the following to your terminal

    to install npm 
    `npm install` 

    to be able to use the database: Don't forget to add the .env  of mongo_URI in the same folder of server.js
    `MONGO_URI= mongodb+srv://DtaBaseName:DdPass@cluster0.njkga.mongodb.net/DtaBaseName?retryWrites=true&w=majority` 

    Finally, to run the app: 
    `npm run devStart` or ` node server.js`

    go to your borwser: at http://localhost:3000/ and now have a local hosted web app.
     
    To Deploy The app: we used Heroku & azure but you can use anyother like AWS,GCP up to you.
          - For heroku: Login and created an app in Heroku.com, then link the app with the github repo and Config Vars with th MONGO DB connection VAR
-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
**BASIC IDEA BEHIND A VIDEO CONFRENCE APP AND tHING YOU NEED TO DEVELOP THE APP:**

- Create your Express js server ->  Express is a minimalist web framework for Node.js — Express makes it very easy to create and run a web server with `Node.Js`.
- Show your Video-Audio to the app -> Using JavaScript `navigator.mediaDevices.getUserMedia`, etc.. 
- Then sett up rooms --> using uuid libary we were able to generate random unique RoomId(URL) for each room.
- Stream others Video & Audio -->  using Socket.io and PeerJs. In short, Socket.io allows us to commincaute between a client and a server. and peer js implements WebRTC. 
    - "https://socket.io/" & "https://peerjs.com/" & "https://webrtc.org/" 
- Sytling the page with CSS. 
- Added The user interfaces .ejs 
- decide what functions you want to use: mute, stop video, etc... 
- Extras
     - login-signup Interfaces dded 
     - Used Mongoose npm and passport Mongoes to provide a schema to our verifiacation, Mongoes provides a straight-forward, schema-based solution to model your application data.
     - Used Mongoose db to store data, 
- Publishing to Online Deployed our app to Heroku host services: we Tried differnt host servises like Azure, heroku and Vultr, it doesn't matter what host server you go with.  


**This app uses:**
- Node js - peer js - socket io - uuid - express - passport - mongoose - npm 

     
    **"Featuers of this WebApp:"**
     - Create a meeting
     - Join a meeting
     - Pre-Viewing before Joining
     - Invite others
     - mute aduio
     - stop video
     - chating
     - share screen
     - Record Screen
     - Login/register
     
-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
**Refrences:**

- Clever Programmer: https://www.youtube.com/watch?v=ZVznzY7EjuY

- w3Schools Node js: https://www.w3schools.com/nodejs/default.asp

- Academind: https://www.youtube.com/watch?v=2qDywOS7VAc 

- WebRTC ventures: https://webrtc.ventures/webrtc-services-new/?utm_source=WebRTCTrainingTutorialseCourseTutorial2

- WebRTC ventures: https://webrtc.ventures/2020/05/webrtc-security-and-privacy/?utm_source=WebRTCTrainingTutorialseCourseDisplacementEmail

- Also Some documents From WebRTC.ventures unfortunately, I can't share them due to security issues.




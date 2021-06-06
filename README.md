# Video Confrence App 
https://leetsmeet.herokuapp.com/ 

**How to use:**

* **As an End-user:**

     1- Firstly, register an account in the web app: https://leetsmeet.herokuapp.com/signup

     2- Login with the configuration you signed up with in the app: https://leetsmeet.herokuapp.com/login

     3- After Logging you will have a choice to either join an ongoing meeting or create a new meeting.

     4- After creating a new meeting you will asked to allow mic and video to be able to interact with the others. 

     5- Then you will be in the pre-viewing room and you will be asked to click on the green cell phone to enter the call room.
     
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
* **As a Developer:**

    After downloading the zip file or cloning to the repository: 
    1- go to your terminal and  install npm `npm install` 
        -if you are using a Vs code, go to server.js right click on the file -> open integrated terminal.  
    2-to be able to use the database: Don't forget to add the .env  of mongo_URI in the same folder of server.js
    `MONGO_URI= mongodb+srv://DtaBaseName:DdPass@cluster0.njkga.mongodb.net/DtaBaseName?retryWrites=true&w=majority` 

    3- Finally, to run the app: 
    `npm run devStart` or ` node server.js`

    4- go to your browser: at http://localhost:3000/ and now have a local hosted web app.
     
    5- To Deploy The app: we used Heroku & azure but you can use any other like AWS,GCP up to you.
          - For Heroku:
               - Login and create an app in Heroku.com.
               - Then link the app with the GitHub repo
               - Lastly, Config Vars with the MONGO DB connection VAR
-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
**BASIC IDEA BEHIND A VIDEO CONFRENCE APP AND THINGS YOU NEED TO DEVELOP THE APP:**

- Create your Express js server ->  Express is a minimalist web framework for Node.js — Express makes it very easy to create and run a web server with `Node.Js`.
- Show your Video-Audio to the app -> Using JavaScript `navigator.mediaDevices.getUserMedia`, etc.. 
- Then sett up rooms --> using uuid library we were able to generate random unique RoomId(URL) for each room.
- Stream others Video & Audio -->  using Socket.io and PeerJs. In short, Socket.io allows us to communicate between a client and a server. and peer.js implements WebRTC. 
    - "https://socket.io/" & "https://peerjs.com/" & "https://webrtc.org/" 
- Sytling the page with CSS. 
- Added The user interfaces .ejs 
- decide what functions you want to use: mute, stop video, etc... 
- Extras
     - login-signup Interfaces added 
     - Used Mongoose npm and passport Mongos to provide a schema to our verification, Mongos provides a straight-forward, schema-based solution to model your application data.
     - Used Mongoose dB to store data, 
- Publishing to Online Deployed our app to Heroku host services: we Tried different host services like Azure, Heroku and Vultr, it doesn't matter what host server you go with.  


**This app uses:**
- Node js - peer js - socket io - uuid - express - passport - mongoose - npm 

     
    **"Features of this WebApp:"**
     - Login/register
     - Create a meeting
     - Join a meeting
     - Pre-Viewing before Joining
     - Invite others
     - mute audio
     - stop video
     - chatting
     - share screen
     - Record Screen
     - Minimizing/ maximizing other video.     
     
-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
**References:**

- Clever Programmer: https://www.youtube.com/watch?v=ZVznzY7EjuY

- w3Schools Node js: https://www.w3schools.com/nodejs/default.asp

- Academind: https://www.youtube.com/watch?v=2qDywOS7VAc 

- WebRTC ventures: https://webrtc.ventures/webrtc-services-new/?utm_source=WebRTCTrainingTutorialseCourseTutorial2

- WebRTC ventures: https://webrtc.ventures/2020/05/webrtc-security-and-privacy/?utm_source=WebRTCTrainingTutorialseCourseDisplacementEmail

- Also, Some documents From WebRTC.ventures unfortunately, I can't share them due to security issues.




# PandemicPal 🤖

PandemicPal is a WhatsApp bot buit during COVID 19 Pandemic that can help you with many works  built on nodejs and Twilio

## Features of PandemicPal 🎆

- Can send you Vaccine Availability and their locations in your area by Pincode [Only in India]
- Can find the address of nearest areas based on your search keyword in the range of 2km
- Can send  nearest isolation centres
- Can provide information about symptoms, precautions during pandemic.
- Can grab the youtube video link based on your search word which keeps you concentrated on what you would like to see instead of getting to youtube and seeing some random recommended stuff
- Can get top 10 repositories from github based on the keyword
- Can get you news based on the location you wish to
- Can get you an image based on the keyword
- Can get you a geeky joke 

## Setup 🍧

- First fork and clone the repo to your system
    > git clone REPO-URL

- Install all the node dependencies
    > npm install

- Create a Twilio account(Free account is more than enough for building purposes)

- Create a .env file and add all the required API KEYS as mentioned in the `.env.example` file

- Now get into Programmable Messaging -> Tryit Out -> Try WhatsApp and configure your WhatsApp sandbox in Twilio console

    ![image](https://user-images.githubusercontent.com/73348574/128043675-f7421cb2-5e13-4da4-9b42-647d9f0a2922.png)

- Download [ngrok](https://dashboard.ngrok.com/get-started/setup) and unzip it in the project folder

- Start your server in the terminal `nodemon server.js` [If it gives any error try `npx nodemon seever.js`]

- Now open new terminal and run `./ngrok http <port>`. Copy the url next to forwarding in the terminal(Ex:http://d9086sssaa4db5.ngrok.io)

- Open WhatsApp sandbox in Twilio console and and paste the url along with `/message` (Ex:http://
d9086sssaa4db5.ngrok.io/message) in `WHEN A MESSAGE COMES IN` textbox

    ![image](https://user-images.githubusercontent.com/73348574/128043257-d57af8b1-d4be-4642-9229-562c6e892973.png)

- Now send a message to the Twilio number saying Hi/Start/Help and you should see an automated message from Twilio with the list of commands


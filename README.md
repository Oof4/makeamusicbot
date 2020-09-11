# Easy Music Bot

Hey Everyone! Today I'll Be Showing You How To Make A Music Bot, And It Should Work.

Hey Hey, No Need For Visual Studio Code And Python And Javascript. No No, We Won't Be Doing That. 
We'll Be Using: Glitch!

So Make A New Project. Make It A Static Site.
Delete Everything But The .env File,
So Make A  File Called Package.json,
And Write This Code Here: 

--------------------------------------------------------------------------------------------------------------------------------------------------------------------
{
  "name": "music-bot-example",
  "version": "1.1.0",
  "description": "ALL ME!",
  "main": "index.js",
  "scripts": {
    "test": "echo \"Error: no test specified\" && exit 1",
    "start": "node ."
  },
  "repository": {
    "type": "git",
    "url": "git+https://github.com/Oof4/makeamusicbot/edit/master/README.md"
  },
  "keywords": [
    "JavaScript",
    "NodeJS",
    "Npm",
    "meee"
  ],
  "author": "MEEEEE",
  "license": "by-nc-nd/4.0",
  "bugs": {
    "url": "https://github.com/Oof4/makeamusicbot"
  },
  "homepage": "https://github.com/Oof4/makeamusicbot/master/README.md",
  "engines": {
    "node": "12.x"
  },
  "dependencies": {
    "@discordjs/opus": "^0.3.2",
    "discord.js": "^12.3.1",
    "dotenv": "^8.2.0",
    "express": "^4.17.1",
    "node-opus": "^0.3.3",
    "opusscript": "0.0.7",
    "simple-youtube-api": "^5.2.1",
    "ytdl-core": "^3.2.2"
  },
  "optionalDependencies": {
    "@discordjs/uws": "^11.149.1"
  }
}


----------------------------------------------------------------------------------------------------------------------------------------------------------------------






Alright, That's Done..
This Is Not The End!
Make A File Called server.js
This makes a message in the terminal when you run it
K. Copy And Paste This Aswell


----------------------------------------------------------------------------------------------------------------------------------------------------------------------

var express = require("express");
var http = require("http");
var app = express();

// Ping the app
app.use(express.static("public"));
// http://expressjs.com/en/starter/basic-routing.html
app.get("/", function (request, response) {
    response.sendStatus(200);
});

// Request listener
var listener = app.listen(process.env.PORT || 3000, function () {
    console.log("Your app is listening on port " + listener.address().port);
});

setInterval(() => {
    http.get(`http://${process.env.PROJECT_DOMAIN}.glitch.me/`);
}, 280000);




------------------------------------------------------------------------------------------------------------------------------------------------------------------

Another One Off Our List! Yeah!


This One Has 19 Lines Of Code, Which Is Not Like Any Of The Above ^^


Make A File Called watch.json
And Copy And Paste This Code:


-------------------------------------------------------------------------------------------------------------------------------------------------------------------------


{
    "install": {
        "include": [
            "^package\\.json$",
            "^\\.env$"
        ]
    },
    "restart": {
        "exclude": [
            "^public/",
            "^dist/"
        ],
        "include": [
            "\\.js$",
            "\\.json"
        ]
    },
    "throttle": 8000000
}





------------------------------------------------------------------------------------------------------------------------------------------------------------------


Coming Soon For More


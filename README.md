Hello!
=========================

[![Deploy](https://www.herokucdn.com/deploy/button.png)](https://heroku.com/deploy)

An attempt to Peer-to-peer video chat that works. 

## Features
* Video chat with up to 15 people (limited only by user interface)
* Buttons to selectively mute audio and turn off video
* Client and server written in a single language: JavaScript
* Supported without client software by browsers with [WebRTC](http://caniuse.com/#feat=rtcpeerconnection)

## Anti-Features
* Does not require client software
* Does not require a Google+ account
* Does not send video stream through a 3rd party
* Does not spike your CPU at 100% utilization

## Requirements
* [EasyRTC](https://www.npmjs.org/package/easyrtc)
* [Express](https://www.npmjs.org/package/express)
* [Handlebars](http://handlebarsjs.com/)
* [nconf](https://www.npmjs.org/package/nconf)
* [socket.io](https://www.npmjs.org/package/socket.io)
* [NodeJS](https://nodejs.org/)

## Install to Heroku
Hello supports Heroku as a demonstration platform. Deployment can be done via the one-click [Deploy to Heroku](https://heroku.com/deploy?template=https://github.com/itss1ddhant/Hello) button or the commands below:

```
heroku login
git clone https://github.com/itss1ddhant/Hello.git
cd Hello
heroku create --http-git
git push heroku master
heroku ps:scale web=1
heroku open
heroku logs --tail
```

## Configuration
The server port, debug level, and SSL settings are configured via the `settings.json` file. tubertc uses port 8080, debug mode, and HTTP by default.


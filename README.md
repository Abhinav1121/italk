# iTalk

🚀 `A free WebRTC browser-based video call, chat and screen sharing` 🚀

<br>

[//]: https://img.shields.io/badge/<LABEL>-<MESSAGE>-<COLOR>

Powered by `WebRTC` using google Stun and [numb](http://numb.viagenie.ca/) Turn. `iTalk` provides video quality and latency not available with traditional technology.

Open the app with the following **supported browsers** & many more...

[//]: #![webrtc](www/images/webrtc.png)

[![Foo](https://mirotalk.herokuapp.com/)

## https://meet.sourcesytax.com/

<br>

[![italk](www/images/preview.png)](https://meet.sourcesytax.com/)

## Features

-   Is `100% Free` and `Open Source`
-   No download, plug-in or login required, entirely browser based
-   Unlimited number of conference rooms without call time limitation
-   Possibility to Lock/Unlock the Room for the meeting
-   Desktop and Mobile compatible
-   Optimized Room URL Sharing (share it to your participants, wait them to join)
-   Webcam Streaming (Front - Rear for mobile)
-   Audio Streaming crystal clear
-   Screen Sharing to present documents, slides, and more...
-   File Sharing, share any files to your participants in the room
-   Select Audio Input - Output && Video source
-   Ability to set video quality up to 4K and adapt the FPS
-   Recording your Screen, Audio and Video
-   Chat with Emoji Picker & Private messages & Save the conversations
-   Simple collaborative whiteboard for the teachers
-   Share any YouTube video in real time
-   Full Screen Mode on mouse click on the Video element
-   Possibility to Change UI Themes
-   Right-click on the Video elements for more options
-   Direct `peer-to-peer` connection ensures the lowest latency thanks to `WebRTC`
-   Supports [REST API](api/README.md) (Application Programming Interface)

## Demo

## Room join

## Quick start

```bash
# clone this repo
$ git clone https://github.com/miroslavpejic85/mirotalk.git
# go to mirotalk dir
$ cd mirotalk
# copy .env.template to .env
$ cp .env.template .env
# install dependencies
$ npm install
# start the server
$ npm start
```

-   Open http://localhost:3000 in browser

---

## Docker

-   Install https://docs.docker.com/compose/install/

```bash
# copy .env.template to .env
$ cp .env.template .env
# build or rebuild services
$ docker-compose build
# create and start containers
$ docker-compose up # -d
# stop and remove resources
$ docker-compose down
```

-   Open http://localhost:3000 in browser

---

## API

```bash
# The response will give you a entrypoint / Room URL for your meeting, where authorization: API_KEY_SECRET.
$ curl -X POST "http://localhost:3000/api/v1/meeting" -H "authorization: mirotalk_default_secret" -H "Content-Type: application/json"
$ curl -X POST "https://mirotalk.up.railway.app/api/v1/meeting" -H "authorization: mirotalk_default_secret" -H "Content-Type: application/json"
$ curl -X POST "https://mirotalk.herokuapp.com/api/v1/meeting" -H "authorization: mirotalk_default_secret" -H "Content-Type: application/json"
```




From where I took inspiration for this project. ❤️

## Contributing

-   Pull Requests are very welcome! :slightly_smiling_face:
-   Just run [prettier](https://prettier.io) on all of your PRs before submitting, this can be done with the following comand: `npm run lint`

-   For communication we use [gitter](https://gitter.im/) or [discord](https://discord.com/) chats which can be found here:

[![Gitter](https://badges.gitter.im/mirotalk/community.svg)](https://gitter.im/mirotalk/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge) [![Discord](https://img.shields.io/badge/chat-discord-green)](https://discord.gg/TAeWXJCvBr)

## License

[![AGPLv3](www/images/AGPLv3.png)](LICENSE)

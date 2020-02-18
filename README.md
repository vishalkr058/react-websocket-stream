# react-websocket-stream

## Description
This Project was built to display 4 iP Camera Stream in one Video on a WebApp
without any need of external plugins like flash or skylight.

You can access the video Stream via the WebApp and you are able to record your 
Video Stream
## Technique
ffmpeg convert our 4 ip RTSP streams into a MpegVideo Socket Stream an push it to
our Webrelay Service.
Our React App gets the Websocket Stream hosted on a specfic port.

### Config your RTSP Streams
Open `start-ffmpeg.bat` location is under jsmpeg

switch the inputs

from 
`rtsp://[User]:[Password]@[IP Adress]/h264Preview_01_sub`
to your rstp Stream

### Start ffmpeg receiver Service

+ `cd jsmpeg`
+ `npm run ffmpeg`

### Start Websocket Relay Server
+ `cd jsmpeg`
+ `npm start`

### Start React App
+ `cd WebApp`
+ `npm start`


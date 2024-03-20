# Spotify Controler
 a versatile spotify controler that uses the ESP8266 wifi features to comunicate with the spotify API, it also includes the capability to use a 20x4 LCD screen over I2C

## features
- pause/play
- skip/go back
- like song
- display song name, progress and duration
- IT SHOWS YOU THE TIME(about 50% of the time this doesn't work)

## how to make the code work
The procces to make this work for your own projects is quite long but worth it at the end, just follow this steps and you will have the code ready in no time:
- replace the WIFI_SSID and PASSWORD with your local house wifi name and password
- go to [spotify for developers](https://developer.spotify.com) and create an account
- with that account go to the dashboard and click on "create app"
- put literaly anything on name and description, put "http://localhost:8888" on redirect URI and click save
- go to the app setings for the app you just created and look for the "client ID" and the "client secret"
- replace the CLIENT_ID and the CLIENT_SECRET if the code with your apps "client ID" and "client secret"
- upload your code and wait until the message "spotify setup" shows up on the LCD
- now go back to the settings of your spotify app and replace the recirect URI you put before with the URL that appears on the LCD with the word "callback" at the end, it should look something like this: "http://131.154.0.11/callback"
- put that same ULR in the code where it says REDIRECT_URI
- uplad the coad again
- ENJOY YOUR CONTROLER :)

## the enclosure
the enclosure is 100% 3d printed with exception of some magnets so that it can stick to magnetic surfaces and some nylon screws and extensions that ussualy come with the LCD display
you can get the design on [OnShape](https://cad.onshape.com/documents/03c0f5b84e5dc7ce18a5b986/w/59c2b69761292aa5b35bee0f/e/642c8b87b2996676210efcd2)

## BROKEN THINGS:
- if your router gets disconected your local IP migth change breaking everything
- the time about 50% of the time shows it's 3:08AM

<br>
[![forthebadge](https://forthebadge.com/images/badges/works-on-my-machine.svg)](https://forthebadge.com)

<br>
[![forthebadge](https://forthebadge.com/images/badges/powered-by-coffee.svg)](https://forthebadge.com)

<br>
[![forthebadge](https://forthebadge.com/images/badges/open-source.svg)](https://forthebadge.com)

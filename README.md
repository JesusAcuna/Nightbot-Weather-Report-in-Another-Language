# Nightbot Weather Report in Another Language

<p align="center">
  <img src=https://cdn.dribbble.com/users/4323909/screenshots/14123163/media/06d26522e0dc02864bb5a6175f778194.png?compress=1&resize=400x300 width="400" height="300">
</p>

You can use the weather variable to create commands that display weather information for a specific location.

Nighbot docs:

> https://docs.nightbot.tv/variables/weather

This tutorial is to make a ninghbot command for weather report in a language other than English, whose default output is in English.

<p align="center">
  <img src="https://github.com/JesusAcuna/Nightbot-Weather-Report-in-Another-Language/blob/main/images/weather%20report%20command.png">
</p>

I'll make an example in Spanish for a command on Twitch, but you can do it in any language and on any platform that accepts Nightbot.

<b>Follow these next steps below:</b>

1. First we need to create a json URL to replace the English words to another, since the twitch chat is limited to 255 characters, and to do the translation we need more space.There's a web page, in which we can place the code to be able to make the translation, and make a request to obtain it.

> https://pastebin.com/

<p align="center">
  <img src="https://github.com/JesusAcuna/Nightbot-Weather-Report-in-Another-Language/blob/main/images/pastebin.png">
</p>

2. The translation in this code example is in Spanish, you just need to pass the translation of the first argument to the second argument in your language and that's it. Then copy that code, as in the image above.:

       w.replace('Weather for', 'El clima para').replace('Conditions are', 'Las condiciones meteorológicas son').replace('with a temperature of',
       'con una temperatura de').replace('The wind is blowing from the', 'La dirección del viento es').replace('and the current humidity is', 'y
       la humedad actual es del').replace('No location provided', 'Escribe tu ciudad/país en Inglés.').replace('Fair', 'buen
       tiempo').replace('Snow Shower', 'nevadas').replace('Mostly', 'mayormente').replace('Clear', 'cielo despejado').replace('Cloudy',
       'nublado').replace('Partly', 'parcialmente').replace('Sunny', 'soleado').replace('rain', 'lluvioso').replace('Wind', 'ventoso').replace(' 
       at ',' a ')

3. In `Optional Paste Settings`, the most important option is paste expiration, since it is the time in which the code will expire. I recommend you to create
an account, so you can then edit your pastebins. After configuring it, click on `Create New Paste`.

<p align="center">
  <img src="https://github.com/JesusAcuna/Nightbot-Weather-Report-in-Another-Language/blob/main/images/pastebin_settings.png">
</p>
  
4. After creating the pastebin, you click on raw to get the url that will help us to make the requests

<p align="center">
  <img src="https://github.com/JesusAcuna/Nightbot-Weather-Report-in-Another-Language/blob/main/images/pastebin_raw.png">
</p>


  

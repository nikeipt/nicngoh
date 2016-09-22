---
layout: post
title: Music to my Heart
tags: [Product Management]
---

There's an idea that's been rattling in the back of my head for a while. A few of us were at the gym and were talking about music and how it changes as we progress through our workout. During warmup its relatively slow and as we progress we require something faster or more energetic as we progress through our lifts.

So then the idea became:

> What if we can change the music automatically according to our heartrate?

Contextual music that changes according to the biofeedback that is fed into it. So how would we go about it? Well you would need API's with real time heartrate data and also a music source with tempo/BPM metadata that can be called upon.

### The heartrate side of things

As people exercise they will fluctuate between heartrate zones. Now these zones are a percentage of your max heart rate zone so they're not universal. Meaning that a baseline will have to be established but you can read more [here](https://www.wareable.com/running/how-to-use-garmin-polar-calculate-hrm-max-heart-rate-training).

![H7 heartrate](/post images/2016-09-22-music-to-my-heart/polar heart rate data.jpg)

The basic premise is that as you shift from one zone into the other, the heartrate monitor will initiate a call to the music player to play something more energetic or more motivational lyrics to match the heartrate.

###### Caveats:
Consider how often these API calls are made. Are they done at the end of the track? When the user chooses to change songs because it's not suitable. What if they shift zones and they want the song to continue till the end.


### The music side of things

I'll be a little biased here because I'm a Spotify user but also because they have an amazing amount of data available to all their music. If you click [here](https://developer.spotify.com/web-api/console/get-audio-features-several-tracks/#complete) you can access their web-API console and get the audio features for any track. Below is the metadata for fuckwithmeyouknowigotit and the field **tempo** shows the BPM of the track.

![fuckwithmeyouknowigotit](/post images/2016-09-22-music-to-my-heart/fuckwithmeyouknowigotit.PNG)

For a MVP I think something along the lines of matching the tempo's of a song to heartrate zone is possible.

* Songs are sorted between a floor and ceiling that equals the users heartrate zones
  * i.e Songs with a tempo between 65 - 85 are for Zone 1
* When real time heart rate crosses into a zone then the music is changed automatically or when the user presses NEXT

###### Caveats:

* Musical taste is deeply personal. While I might listen to trance or upbeat BND when I'm working out, someone else might wish to listen to RNB even at the high end of their heartrate. To take into account these things a tracker should be placed i.e how often is a song skipped in a particular zone and when is it allowed to play to tailor the playlist to the user
* Tempo is a good place to start measuring what songs to play when a user crosses into a heartrate zone but it's not the only metric to consider. Below is a song that I listen a lot to when I get ready for a big lift even though the BPM is significantly lower. Other metrics like **Energy** and **loudness** are both metrics I would consider as this feature progresses.

![Prisoner 1&2](/post images\2016-09-22-music-to-my-heart\Prison 1&2.PNG)

Currently this doesn't exist though RockMyRun is making an attempt at this. Part of this is dependent on the wearables market. While the H7 is designed specifically for enthusiasts, other products like the Fitbit Surge require people to pay a $50 p.a fee just to export their data. As wearables get more accurate hopefully something like this will come about. 

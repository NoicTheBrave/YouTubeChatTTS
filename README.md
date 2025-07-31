# YouTubeChatTTS

Just a simple script cobbled together with glue and ducktape to collect chat messages from any livestream and read them aloud - No filters. 

If you'd like to filter them, fill free to dig in and do that yourself - this is a simple demonstration script. 

#This actually works At the moment - this is the file you are looking for
## How it works: 
It takes chat messages, makes them into a buffer file, then plays the audio and automatically adds all chat messages into a queue to be converted then played as audio (means only 1 audio file will exist at a time for this and will be constantly written over, which is fine lol) 
#Needs Stream ID (aka the videoID of the stream) in order to pull the data it needs 

## Libraries and Requirements

---------WARNING: PERMISSIONS REQUIRED - WorkAround (just install this, its ez)---------
Needed to not only install pydub, but for permissions to get thru you also needed ``pip install simpleaudio``
otherwise it will throw an error with "Permissions denied"

Python: Ver. 3.10.11 (from Microsoft Store - probably not relavent)

### Libraries

* pytchat: verson 0.5.5
* gtts: verson 2.5.1
* pydub: verion 0.25.1
* simpleaudio: version 1.0.4 (the permissions one that works in the background, but not directly imported)
* os (UNKNOWN - doesnt have a __version__)
* time: (UNKNOWN - doesnt have a __version__)
* threading: : (UNKNOWN - doesnt have a __version__)

### Hardware Used
Not sure if this matters any, but I know different versions of OS's can screw with things sometimes and need work arounds that others dont, so here are those stats too 

Edition	Windows 11 Pro
Version	23H2


## How to use
Just install the libraries (versions specified just incase things do not work with the most recent versions of these things) and run ``main.py``. 

Please note you will need to enter in the Youtube video ID / Stream ID (ex. in the youtube video ``https://www.youtube.com/watch?v=dQw4w9WgXcQ``, the video ID is ``dQw4w9WgXcQ``). Yes, I know it's annoying to grab everytime for you streamers, but this was the minimal viable product and easiest to test in the ~2 hrs of "vibecoding" and bullshitting my way thru ripping apart other examples and code examples - so deal with it :P
 
Side note: 
(Ik there is a way to do it, probably just get the most recent "video" from a youtube channel in question, typically if they are live it should be the first recommended video, and rip that videos URL and isolate the end of the URL (I think) if you really wanted to truy - thats one idea idk 

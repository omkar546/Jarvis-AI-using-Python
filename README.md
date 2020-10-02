# Jarvis-AI-using-Python
reated and Tested on Linux with Python 2.7
An attempt to make a very simple, Personal Assistant that understands speech as well as text input and is capable of performing tasks other than conversing. This project is based on AIML 1.0 and uses pyaiml for using the AIML interpreter in python. AIML, is based on pattern matching and this project does not implement any sort of machine learning or language processing. Combined with a few python scripts, J.A.R.V.I.S now performs quite a few tasks:

Converses, barely.
Talk to J.A.R.V.I.S : hello
J.A.R.V.I.S : Well, hello

Talk to J.A.R.V.I.S : Who is iron man?
J.A.R.V.I.S : Iron man is the one who created me.

Talk to J.A.R.V.I.S : What does JARVIS stand for?
J.A.R.V.I.S : JARVIS stands for Just A Rather Very Intelligent System

All conversation is only for the hardcoded patterns, which are quite few. Can be easily extended to add AIML scripts of ALICE and other existing AIs.

Rhythmbox: Play, Pause, Open.
Uses shell commands to play and pause rhythmbox music.

Talk to J.A.R.V.I.S : play music
J.A.R.V.I.S : On it!
Talk to J.A.R.V.I.S : play music
J.A.R.V.I.S : On it!
Talk to J.A.R.V.I.S : please open rhythmbox jarvis
J.A.R.V.I.S : Right away, sir!

Tells time.
Talk to J.A.R.V.I.S : what time is it?
J.A.R.V.I.S : The time is 4 43 am

Gives a brief system status.
Talk to J.A.R.V.I.S : how are you? / System report / System Status
J.A.R.V.I.S : I am fine, sir. All systems are at 100 percent. Battery percentage: 100%. Battery state: discharging. 265 processes are currently running. Current volume is 30 percent

Suggests Googling for all unrecognized interrogative questions
Talk to J.A.R.V.I.S : What is IIT, Bombay?
J.A.R.V.I.S : Do you want me to google that for you?
Talk to J.A.R.V.I.S : yes
J.A.R.V.I.S : Right away, sir! Created new window in existing browser session.

Plays any song, first search result in youtube
Talk to J.A.R.V.I.S : play me a song
J.A.R.V.I.S : What song, sir?
Talk to J.A.R.V.I.S : Alter Bridge Isolation
J.A.R.V.I.S : On it! Created new window in existing browser session.

Uses youtube.py script to find the first search result for the last user input in above case, and opens it in chromium browser.

Searches internet.
Talk to J.A.R.V.I.S : Google what is the answer to life?
J.A.R.V.I.S : Right away, sir! Created new window in existing browser session.
Talk to J.A.R.V.I.S : Search youtube for Call of Duty
J.A.R.V.I.S : On it! Created new window in existing browser session.
Talk to J.A.R.V.I.S : Search for Navi Mumbai on google maps
J.A.R.V.I.S : On it! Created new window in existing browser session.

Changes Wallpaper.
Keep a set of wallpapers (and nothing else) in J.A.R.V.I.S/wallpapers directory. wallpaper.py randomly selects one and sets it as the desktop wallpaper by changing the key value using dconf-editor.

Talk to J.A.R.V.I.S : change wallpaper
J.A.R.V.I.S : On it!

Launches Programs.
Talk to J.A.R.V.I.S : open nautilus
J.A.R.V.I.S : Right away, sir!
Talk to J.A.R.V.I.S : take me to /etc
J.A.R.V.I.S : Sure thing! (Opens /etc in nautilus)
Talk to J.A.R.V.I.S : take me home
J.A.R.V.I.S : Sure thing! (Opens ~ in nautilus)
Talk to J.A.R.V.I.S : open chromium / open firefox / open calculator / open vlc
J.A.R.V.I.S : Sure thing!

Other:
Standard replies for unrecognized/unmatched inputs

Talk to J.A.R.V.I.S : you are dumb
J.A.R.V.I.S : I don't understand that yet. Maybe you could teach me.
Talk to J.A.R.V.I.S : no I won't
J.A.R.V.I.S : I don't know how to answer that. Maybe I could interest you in something else.

Talk to J.A.R.V.I.S : go to sleep / exit / quit / bye / goodbye

closes the python script.

Requirements:
Make sure you install these packages before moving forward to other python libraries-

sudo apt install libasound-dev portaudio19-dev libportaudio2 libportaudiocpp0 ffmpeg libav-tools

You can run pip install -r requirements.txt to install them all.

Individual packages listed as follows-

AIML (For Pattern Recognition)
pip install aiml

Speech Recognition
pip install SpeechRecognition

PyAudio is required for microphone input
pip install pyaudio

alsaaudio: (For Volume Control, Linux only)
pip install pyalsaaudio

ttsx: (Offline Text to Speech Service)
pip install pyttsx

Optional for Google Text to Speech :
gTTS: (Google Text to Speech service)
pip install gTTS

PyGame: (For audio playback with gTTS)
pip install pygame

argparse (For parsing arguments)
pip install argparse

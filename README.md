# Installation

## OS X
Installing youtube-dl - [(Official HowTo)](https://ytdl-org.github.io/youtube-dl/download.html)
```
sudo curl -L https://yt-dl.org/downloads/latest/youtube-dl -o /usr/local/bin/youtube-dl
```
```
sudo chmod a+rx /usr/local/bin/youtube-dl
```

Installing FFMPEG (used when downloading audio - to convert to mp3)
```
brew install ffmpeg
```

## Linux via Python (RPi included)
```
sudo pip install --upgrade youtube_dl
sudo pip install ffmpeg
sudo pip install ffprobe
```

# Scripts

## youtube-audio-dl
__Purpose:__ Call youtube-dl with a YouTube _single video link_, attempts to download the linked video as an audio mp3. File is saved in the shell's current working directory.

__Usage:__ Once installed, call from the directory you want the downloads in..
```
youtube-audio-dl "https://www.youtube.com/watch?v=dQw4w9WgXcQ"
```

__Install:__
```
sudo cp youtube-audio-dl /usr/local/bin/

sudo chmod a+rx /usr/local/bin/youtube-audio-dl
```

---

## youtube-audio-list-dl
__Purpose:__ Call youtube-dl with a YouTube _playlist link_, attempts to download the videos in the playlist as audio mp3 files. Files are saved in the shell's current working directory.

__Usage:__ Once installed, call from the directory you want the downloads in..
```
youtube-audio-list-dl "https://www.youtube.com/playlist?list=______________"
```

__Install:__
```
sudo cp youtube-audio-list-dl /usr/local/bin/

sudo chmod a+rx /usr/local/bin/youtube-audio-list-dl
```
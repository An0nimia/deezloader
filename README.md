# deezloader
The library lays [HERE](https://pypi.org/project/deezloader/) due DMCA takedown. IT IS A JUST FREE PROJECT, which help people poor like me to listen their favorite music. PLEASE DO NOT TAKE DOWN IT IS COMPLETLY NO PROFIT THANKS YOU A LOT

# deezloader

This project has been created to download songs, albums or playlists with Spotify or Deezer link from Deezer.

# Disclaimer

- I am not responsible for the usage of this program by other people.
- I do not recommend you doing this illegally or against Deezer's terms of service.
- This project is licensed under [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/)


* ### PYTHON VERSION SUPPORTED ###
	![Python >= 3.9](https://img.shields.io/badge/python-v%3E=3.9-blue)

* ### OS Supported ###
	![Linux Support](https://img.shields.io/badge/Linux-Support-brightgreen.svg)
	![macOS Support](https://img.shields.io/badge/macOS-Support-brightgreen.svg)
	![Windows Support](https://img.shields.io/badge/Windows-Support-brightgreen.svg)

* ### Installation ###
```bash
pip3 install deezloader
```

# SETTING
	[deez_login]
	mail = #YOUR DEEZER EMAIL
	password = #YOUR DEEZER PASSWORD
	token = #YOUR URL TOKEN GOT FROM DEEZER

### Setting disclaimer
- Write that content inside .deez_settings.ini file for using deez-dw.py

# API Avalaible

Finally **deez-web.py** avalaible ;)
```bash
deez-web.py
```

### API disclaimer
- Open your browser at http://127.0.0.1:8000/docs

# CLI interface

Finally **deez-dw.py** avalaible ;)
```bash
deez-dw.py -h
```
	usage: deez-dw.py [-h] [-l LINK] [-s SONG] [-a ARTIST] [-o OUTPUT]
	[-q {FLAC,MP3_320,MP3_128}] [-rq] [-rd]
	[-g] [-z] [-sa {0,1,2}]

## OPTIONS
	-h, --help            show this help message and exit
	-l LINK, --link LINK  Deezer or Spotify link for download
	-s SONG, --song SONG  song name
	-a ARTIST, --artist ARTIST
						artist song
	-o OUTPUT, --output OUTPUT
						Output folder
	-q {FLAC,MP3_320,MP3_128}, --quality {FLAC,MP3_320,MP3_128}
	-rq, --recursive_quality
						If choosen quality doesn't exist download with best possible
						quality (True or False)
	-rd, --recursive_download
						If the song has already downloaded skip (True or False)
	-g, --not_gui         Show the little not_gui (True or False)
	-z, --zip             If is an album or playlist link create a zip archive (True or
						False)
	-sa {0,1,2}, --save {0,1,2}

# Library

### Initialize

```python
from deezloader import Login

# if you want login with arl, IT EXPIRES
downloa = Login(arl = my_arl_token)
# if you want to login through your email and password, SHOULD LAST FOREVER
downloa = Login(
	email = my_deezer_email,
	password = my_deezer_password
)
```

### Download song

Download track by Spotify link

```python
downloa.download_trackspo(
	#YOUR SPOTIFY TRACK LINK,
	output_dir = #The output dir for the download,
	quality_download = #Choose between FLAC, MP3_320, MP3_128,
	recursive_quality = #True or False,
	recursive_download = #True or False,
	not_interface = #True or False,
	method_save = #choose between 0, 1 or 2
)
```

Download track by Deezer link
```python
downloa.download_trackdee(
	#YOUR DEEZER TRACK LINK,
	output_dir = #The output dir for the download,
	quality_download = #Choose between FLAC, MP3_320, MP3_128,
	recursive_quality = #True or False,
	recursive_download = #True or False,
	not_interface = #True or False,
	method_save = #choose between 0, 1 or 2
)
```

### Download album
Download album by Spotify link
```python
downloa.download_albumspo(
	#YOUR SPOTIFY ALBUM LINK,
	output_dir = #The output dir for the download,
	quality_download = #Choose between FLAC, MP3_320, MP3_128,
	recursive_quality = #True or False,
	recursive_download = #True or False,
	not_interface = #True or False,
	make_zip = #True or False,
	method_save = #choose between 0, 1 or 2
)
```

Download album from Deezer link
```python
downloa.download_albumdee(
	#YOUR DEEZER ALBUM LINK,
	output_dir = #The output dir for the download,
	quality_download = #Choose between FLAC, MP3_320, MP3_128,
	recursive_quality = #True or False,
	recursive_download = #True or False,
	not_interface = #True or False,
	make_zip = #True or False,
	method_save = #choose between 0, 1 or 2
)
```

### Download playlist

Download playlist by Spotify link
```python
downloa.download_playlistspo(
	#YOUR SPOTIFY PLAYLIST LINK,
	output_dir = #The output dir for the download,
	quality_download = #Choose between FLAC, MP3_320, MP3_128,
	recursive_quality = #True or False,
	recursive_download = #True or False,
	not_interface = #True or False,
	make_zip = #True or False,
	method_save = #choose between 0, 1 or 2
)
```

Download playlist from Deezer link
```python
downloa.download_playlistdee(
	#YOUR DEEZER PLAYLIST LINK,
	output_dir = #The output dir for the download,
	quality_download = #Choose between FLAC, MP3_320, MP3_128,
	recursive_quality = #True or False,
	recursive_download = #True or False,
	not_interface = #True or False,
	make_zip = #True or False,
	method_save = #choose between 0, 1 or 2
```

### Download name

Download by name
```python
downloa.download_name(
	artist = #ARTIST NAME,
	song = #ARTIST SONG NAME,
	output_dir = #The output dir for the download,
	quality_download = #Choose between FLAC, MP3_320, MP3_128,
	recursive_quality = #True or False,
	recursive_download = #True or False,
	not_interface = #True or False,
	method_save = #choose between 0, 1 or 2
)
```

# DONATION

IF YOU ARE POOR DON'T DONATE I AM ALSO POOR, IF YOU ARE RICH JUST PRESS [HERE](https://www.paypal.com/paypalme/an0nimia) THANKS YOU :)

# HEY YOUUUU

Too Lazy to finish the shitty documentation with VSCode you should be able discover the other params, methods and propieties I will try to do something more professional, MAYBE :)

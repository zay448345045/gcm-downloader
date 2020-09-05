# gcm-downloader
**Groove coaster mobile server downloader**

![Thumbnail](https://user-images.githubusercontent.com/33218378/92287708-d7f39e00-ef0a-11ea-9960-5b3a019a0542.PNG)

yes, to run this you need to have python 3 installed and 
install dependencies by putting these lines in your command prompt or shell:
```batch
pip install requests
pip install pycryptodome
pip install bs4
pip install lxml
```
after that you can do 
```batch
python start.py
``` 
and achieve server files yes.

**What does it download:**

- .pak files (contains filenames of server assets and game assets)
- .ogg music (Every song (BGM+SHOT) in the game including DLC and removed songs)
- .dat charts (They include filenames of the .ogg music so the program does parse them at util.getNamesFromChart())
- .m4a previews (Basically the preview songs you'd hear ingame before purchasing a song)

**What it can't download yet:**

- Ads (The ad banners you can see at login page and in store, i have working code for this but i'll implement it into this project cleanly later)
- Titles (The title-cards you can select as a player, again, i have working code, i'll implement soon)
- All .pak files (9.3 million possible urls, i'll add a list of valid urls in this program once i am done bruteforcing)

**Bro what is the password:**

All .zip files are encrypted by default with **`eiprblFFv69R83J5`**, i don't want to alter the data.

If you forget it somehow, you can find it again in util.ZIP_PASSWORD

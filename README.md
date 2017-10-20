# youtube-playlist-scraper
downloading playlist on channels from youtube, seperate directory. 

<h4>:))) => Already Exits from https://github.com/rg3/youtube-dl/blob/master/README.md#readme :</h4>

<p>Download YouTube playlist videos in separate directory indexed by video order in a playlist</p>

```shell
$ youtube-dl -o '%(playlist)s/%(playlist_index)s - %(title)s.%(ext)s' \
  https://www.youtube.com/playlist?list=PLwiyx1dc3P2JR9N8gQaQN_BCvlSlap7re
```

<p>Download all playlists of YouTube channel/user keeping each playlist in separate directory:</p>

```shell
$ youtube-dl -o '%(uploader)s/%(playlist)s/%(playlist_index)s - %(title)s.%(ext)s' \ 
  https://www.youtube.com/user/TheLinuxFoundation/playlists
```

# Installing

```shell
  $ git clone https://github.com/pleycpl/youtube-playlist-scraper  # First download repo
  $ cd youtube-playlist-scraper         # changed active directory to repo
  $ virtualenv -p python3 venv          # create virtual enviroment
  $ source venv/bin/active              # actived virtual environment
  $ pip install -r requirements.txt     # download requirement packages.
```

# Usage

```shell
  $ python3 main.py https://www.youtube.com/user/<channelName>/playlists requests   # Crawling with request package
  $ python3 main.py https://www.youtube.com/user/<channelName>/playlists selenium   # Crawling with selenium package, because js.
```

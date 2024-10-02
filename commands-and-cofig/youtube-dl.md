# Youtube-dl-Fu

### Download all playlists of YouTube channel/user keeping each playlist in separate directory: 

`youtube-dl -o '%(uploader)s/%(playlist)s/%(playlist_index)s - %(title)s.%(ext)s' https://www.youtube.com/user/TheLinuxFoundation/playlists`

`youtube-dl`

`youtube-dl -- -wNyEUrxzFU`

### Download best available:

`youtube-dl -f bestaudio+bestvideo "http://www.youtube.com/watch?v=VIEWCODE`

`youtube-dl -f 131+141 "http://www.youtube.com/watch?v=VIEWCODE`


### View available formats:

`youtube-dl -F "http://www.youtube.com/watch?v=VIEWCODE”`

### Download playlist

`https://www.youtube.com/playlist?list=PLAYLIST-CODE`

`youtube-dl -t https://www.youtube.com/playlist?list=PLAYLIST-CODE`

### Create URL list

`youtube-dl -cit -a file_name_in_which_you_paste_URL_list`

### Download to a folder

`-o “/users/USER/directory/%(title)s-%(id)s.%(ext)s"`

### Download playlist to a folder

`youtube-dl -o “/users/USER/directory/%(title)s-%(id)s.%(ext)s" https://www.youtube.com/playlist?list=PLAYLIST-CODE`

# musicAPI


This is a project made with .net to obtain the backend API of NetEase Cloud Music, developed with VS2013

The currently provided APIs are:

searching feature

Request address: /api/music/search?s={0}&limit={1}&offset={2}&type={3}
Request parameters:
s: search term
limit: used for paging, the number of returned items (default 30)
offset: offset, used for paging (default 0)
type: search type, (default 1) [1 single] [10 albums] [100 artists] [1000 songs] [1002 users]
Playlist (selected by netizens) hot

Request address: api/music/topPlaylist?cat=all&order=hot&offset=0&total=true&limit=3
Request parameters:
cat: category (default hot), other parameters, refer to: category name in http://music.163.com/#/discover/playlist
order: collation (default is hot)
offset: offset, used for paging (default 0)
total: the total number under the category
limit: used for paging, the number of returned items (default 50)
Song Details

Request address: api/music/detail?ids=29775505,300587
Request parameters:
ids: The ID corresponding to the song can also be multiple
get lyrics

Request address: api/music/lyric?id=29775505
Request parameters:
id: Get the song ID corresponding to the lyrics
Get playlist details

Request address: api/music/playlist?id=374755836
Request parameters:
id: the ID corresponding to the playlist
Get MV details

Request address: api/music/mv?id=333042
Request parameters:
id: corresponding MVID
thanks

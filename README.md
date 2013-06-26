spotifyripper
=============

small ripper script for spotify (rips playlists to mp3 and includes ID3 tags v1.1) 

note that stream ripping violates the ToC's of libspotify!

usage
-----
    ./jbripper.py [username] [password] [spotify_url]

example
-------
    "./jbripper.py user pass spotify:track:52xaypL0Kjzk0ngwv3oBPR" creates "Beat It.mp3" file
    "./jbripper.py user pass spotify:user:[user]:playlist:7HC9PMdSbwGBBn3EVTaCNx rips entire playlist

features
--------
* real-time VBR ripping from spotify PCM stream

* writes id3 tags v1.1 compatible with old mp3 players

* creates files and directories based on the following structure Artist/Album/01 - Artist - Song.mp3

prerequisites:
--------------
* libspotify (download at https://developer.spotify.com/technologies/libspotify/)

* pyspotify (sudo pip install -U pyspotify)

* spotify appkey (download at developer.spotify.com, requires premium!)

* lame

* eyeD3 (pip install eyeD3)

TODO
----
- [ ] skip exisiting track (avoid / completed tracks / completed = successful id3)
- [ ] detect if other spotify instance is interrupting
- [ ] add album supprt : spotify:album:1UnRYaeCev9JVKEHWBEgHe


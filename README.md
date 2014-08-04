spotifyripper
=============

small ripper script for spotify (rips playlists to mp3 and includes ID3 tags)

note that stream ripping violates the ToC's of libspotify!

usage
-----
    ./jbripper.py [username] [password] [spotify_url]

examples
--------
    "./jbripper.py user pass spotify:track:52xaypL0Kjzk0ngwv3oBPR" creates "Beat It.mp3" file
    "./jbripper.py user pass spotify:user:[user]:playlist:7HC9PMdSbwGBBn3EVTaCNx rips entire playlist

features
--------
* real-time VBR ripping from spotify PCM stream

* writes id3 tags (including album covers)

* creates files and directories based on the following structure artist/album/song.mp3

prerequisites:
--------------
* libspotify (download at https://developer.spotify.com/technologies/libspotify/)

* pyspotify (sudo pip install -U pyspotify, requires python-dev)

* spotify binary appkey (download at developer.spotify.com and copy to wd, requires premium!)

* lame (sudo apt-get install lame)

* eyeD3 (sudo pip install eyeD3 --allow-external eyeD3 --allow-unverified eyeD3)

TODO
----
- [ ] skip exisiting track (avoid / completed tracks / completed = successful id3)
- [ ] detect if other spotify instance is interrupting
- [ ] add album supprt : spotify:album:1UnRYaeCev9JVKEHWBEgHe

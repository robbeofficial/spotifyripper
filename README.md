spotifyripper
=============

small ripper script for spotify (rips playlists to mp3 and includes ID3 tags and album covers) 

note that stream ripping violates the ToC's of libspotify!

usage
    ./jbripper.py [username] [password] [spotify_url]

example
    "./jbripper.py user pass spotify:track:52xaypL0Kjzk0ngwv3oBPR" creates "Beat It.mp3" file
    "./jbripper.py user pass spotify:user:[user]:playlist:7HC9PMdSbwGBBn3EVTaCNx rips entire playlist

features
    - real-time VBR ripping from spotify PCM stream
    - writes id3 tags (including album cover)

prerequisites:
    - libspotify (download at https://developer.spotify.com/technologies/libspotify/)
    - pyspotify (sudo pip install -U pyspotify)
    - spotify appkey (download at developer.spotify.com, requires premium!)
    - jukebox.py (pyspotify example)
    - lame
    - eyeD3 (pip install eyeD3)

TODO
- album name subdir
- skip exisiting track (avoid / completed tracks / completed = successful id3)
- detect if other spotify instance is interrupting
. add album supprt : spotify:album:1UnRYaeCev9JVKEHWBEgHe

FIXME
..done!
Assertion 'pa_atomic_load(&(b)->_ref) > 0' failed at pulsecore/memblock.c:590, function pa_memblock_unref(). Aborting.
Aborted (core dumped)

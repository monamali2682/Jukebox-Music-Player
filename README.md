# Jukebox - Music Player
Functional Requirements
A user can create a playlist from a pool of available songs.
A user can delete a playlist.
A user can add / delete songs from the playlist.
A user can start playing songs by choosing a playlist. On choosing a playlist, the first song in the playlist will start playing.
A user can switch songs by using Next, Back command or by choosing another song from the playlist that has been chosen. 
On reaching the end, Next will switch to the first song in the current playlist.
On reaching the start, Back will switch to the last song in the playlist.
Only one song can be played at a time.
A user can choose to play the song from another playlist if and only if that playlist is selected. Basically two operations have to be done to successfully play the song of their choice. 
Select the playlist ( which will play the first song when selected )
Choose the song of your choice.
An album is a collection of songs owned by the original artist / artist group .
Artist Group Example:- One Direction. 
One Direction Group is the album owner and is considered as an artist.
Each song can feature multiple artists but it will be owned by the artist whose album this song belongs to.
Each song can only be a part of one album.


INPUT:-

LOAD-DATA songs.csv
CREATE-USER Kiran
CREATE-PLAYLIST 1 MY_PLAYLIST_1 1 4 5 6
CREATE-PLAYLIST 1 MY_PLAYLIST_2 1
DELETE-PLAYLIST 1 2
PLAY-PLAYLIST 1 1
MODIFY-PLAYLIST ADD-SONG 1 1 7
MODIFY-PLAYLIST DELETE-SONG 1 1 7
PLAY-SONG 1 5
PLAY-SONG 1 NEXT
PLAY-SONG 1 NEXT
PLAY-SONG 1 BACK
PLAY-SONG 1 BACK
PLAY-SONG 1 19

OUTPUT:-

Songs Loaded successfully
1 Kiran
Playlist ID - 1
Playlist ID - 2
Delete Successful
Current Song Playing
Song - South of the Border
Album - No.6 Collaborations Project
Artists - Ed Sheeran,Cardi.B,Camilla Cabello
Playlist ID - 1
Playlist Name - MY_PLAYLIST_1
Song IDs - 1 4 5 6 7
Playlist ID - 1
Playlist Name - MY_PLAYLIST_1
Song IDs - 1 4 5 6
Current Song Playing
Song - Cross Me
Album - No.6 Collaborations Project
Artists - Ed Sheeran,Chance The Rapper,PnB Rock
Current Song Playing
Song - Give Life Back To Music
Album - Random Access Memories
Artists - Daft Punk,Nile Rodgers
Current Song Playing
Song - South of the Border
Album - No.6 Collaborations Project
Artists - Ed Sheeran,Cardi.B,Camilla Cabello
Current Song Playing
Song - Give Life Back To Music
Album - Random Access Memories
Artists - Daft Punk,Nile Rodgers
Current Song Playing
Song - Cross Me
Album - No.6 Collaborations Project
Artists - Ed Sheeran,Chance The Rapper,PnB Rock
Given song id is not a part of the active playlist

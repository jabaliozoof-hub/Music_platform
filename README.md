# UML Design Lab: Music Streaming Platform
 
A UML design exercise for a system similar to a music streaming platform. Users explore music, organize content, and manage their personal collections of songs, albums, artists, and playlists.
 
## Problem Description
 
Users interact with music in different ways:
 
- Browse songs and albums
- Create playlists to organize songs
- Add albums or songs to their personal library
- Follow artists to keep track of their content
Music is structured hierarchically:
 
- An artist can create multiple albums
- An album contains multiple songs
User interactions must reflect this structure and keep data consistent.
 
## Key Constraints
 
- A song belongs to an album
- An album belongs to an artist
- A playlist is created and managed by a user
- A user can interact with multiple playlists, artists, and albums
## Use Cases
 
### 1. Add a song to a playlist
 
1. The user selects a playlist
2. The user selects a song
3. The system adds the song to the playlist
### 2. Follow an artist
 
1. The user selects an artist
2. The system records the relationship
### 3. Remove a song from a playlist
 
1. The user selects a playlist and a song
2. The system removes the song
## Modeling Notes
 
- Focus on modeling relationships clearly
- Make sure playlists behave consistently with songs and users
- Do not model streaming or playback behavior
## Main Classes
 
| Class      | Role                                                        |
| ---------- | ----------------------------------------------------------- |
| `User`     | Creates playlists, follows artists, owns a library          |
| `Artist`   | Creates albums                                              |
| `Album`    | Belongs to one artist, contains songs                       |
| `Song`     | Belongs to one album                                        |
| `Playlist` | Created and managed by one user, contains songs             |
| `Library`  | A user's personal collection of albums and songs            |

## Deliverables
 
- Class diagram with attributes, methods, relationships, and multiplicities
- Sequence diagrams for the three use cases

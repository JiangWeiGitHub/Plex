# How to use Plex

[**Official Site**](https://www.plex.tv/)<p>
[**Docker Site**](https://hub.docker.com/r/linuxserver/plex/)

### Usage for Docker
  1. host local tree
  ```

  .
  ├── libray
  │   └── Library
  │       ├── Application Support
  │       │   └── Plex Media Server
  │       │       ├── Cache
  │       │       ├── Codecs
  │       │       ├── Crash Reports
  │       │       ├── Logs
  │       │       ├── Media
  │       │       ├── Metadata
  │       │       ├── plexmediaserver.pid
  │       │       ├── Plug-ins
  │       │       ├── Plug-in Support
  │       │       ├── Preferences.xml
  │       │       └── Thumbnails
  │       └── linuxserver-chown.lock
  └── Media
      ├── Movies
      │   ├── a.avi
      │   └── video.mp4
      ├── Music
      │   ├── Beyond-iaserver.pid
      │   ├── Beyond-nces.xml
      │   ├── Beyond-nces.xml
      │   ├── Beyond-iaserver.pid
      │   ├── \13756665710罉\13756665710罉\12743354375
      │   ├──
      │   ├── G.E.M.-iaserver.pid
      │   ├── Smile.DK-Butterfly.mp3
      │   ├── Twins-Ī˹-Butterfly.mp3
      │   └── \13756671030罉\13756671030罉\25265431420噑\25265431420噑\16434467560\17777777400
      ├── Photo
      │   ├── 20120711494.jpg
      │   ├── 20120711495.jpg
      │   ├── 20120711497.jpg
      │   ├── 20120711498.jpg
      │   ├── 20120711499.jpg
      │   ├── 20120711500.jpg
      │   ├── 20120711501.jpg
      │   ├── 20120711502.jpg
      │   ├── 20120711503.jpg
      │   ├── 20120711504.jpg
      │   ├── 20120711505.jpg
      │   ├── 20120711506.jpg
      │   ├── 20120711507.jpg
      │   ├── 20120711508.jpg
      │   ├── 20120711509.jpg
      │   ├── 20120711510.jpg
      │   ├── 20120711511.jpg
      │   ├── 20120711512.jpg
      │   ├── test.jpg
      │   └── Thumbs.db
      └── TV Shows
          └── Grey's Anatomy
              └── Season 01
                  └── Grey's Anatomy - s01e01.avi
                      
  ```
  
  2. docker run --name=plex --net=host -e VERSION=latest -v /home/winsun/libray:/config -v /home/winsun/Media/Movies:/data/movies:ro -v /home/winsun/Media/Music:/data/music:ro -v
 /home/winsun/Media/Photo:/data/photo:ro -v /home/winsun/Media/TV\ Shows:/data/tvshows:ro linuxserver/plex
 
  3. register user
  ```
  
  wei.jiang
  1234qwer
  
  ```

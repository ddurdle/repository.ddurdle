XBMC-firedrive
==============

FireDrive / Putlocker Video add-on for XBMC

A video add-on for XBMC that enables playback of videos stored in a FireDrive account.

Supports [Tested on]:
All XBMC 12, 12.2, 13 including Linux, Windows, OS X, Android, Pivos, iOS (including ATV2), Raspberry Pi

Thoroughly tested on XBMC for Linux v13 & Raspberry Pi Raspbmc v12


Getting Started:
1) download the .zip file
2) transfer the .zip file to XBMC
3) in Video Add-on, select Install from .zip

Before starting the add-on for the first time, either "Configure" or right click and select "Add-on Settings".  Enter your Username and Password.

Features and limitations:
- will index videos in your FireDrive account, sorted by title name
- includes support for folders
- only indexes and playback videos and audio

Modes:
1) standard index (folderID=0)
- starting the plugin via video add-ons will display a directory containing all video/audio files and folders contained in the root folder of your FireDrive account
- click on a video/audio file to playback
- you can create favourites of the video/audio files or folders
2) mode=folder (folderID=0)
- create .strm or .m3u files containing the following: plugin://plugin.video.firedrive/?mode=folder&amp;folderID=unique_folder_id
- starting the plugin and display all video/audio files and folders within the folder specified
- click on a video/audio file to playback
- you can create favourites of the video/audio files or folders
3) mode=streamVideo
- playback via stream
- create .strm or .m3u files containing the following: plugin://plugin.video.firedrive/?mode=streamVideo&amp;filename=unique_file_id
- you can create a sample plugin call of this type and format by invoking the plugin normally, and right-clicking, add to favourites any video.  The video will be added to your favourites with the correct syntax and parameters needed to invoke the plugin using this method.
- if your video is composed of multiple clips, you can create a .m3u that makes the above plugin:// call, one line for each clip.  You can then create a .strm file that points to the .m3u.  XBMC can index movies and shows contained in your Google Drive account by either a .strm containing a single plugin:// call to the video, or a .strm that points to a local .m3u file that contains a list of plugin:// calls representing the video
4) mode=streamURL
- playback a specific FireDrive video/audio URL (format: http://www.firedrive.com/file/#####) via stream
- handy for playback of publicly shared videos stored in FireDrive
- create .strm or .m3u files containing the following: plugin://plugin.video.firedrive/?mode=streamURL&amp;url=http://www.firedrive.com/file/#####
- if your video is composed of multiple clips, you can create a .m3u that makes the above plugin:// call, one line for each clip.  You can then create a .strm file that points to the .m3u.  XBMC can index movies and shows contained in your Google Drive account by either a .strm containing a single plugin:// call to the video, or a .strm that points to a local .m3u file that contains a list of plugin:// calls representing the video


Roadmap to future releases:
- support for multiple Google Drive accounts
- support for pictures
- support for caching account contents

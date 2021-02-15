# panoptoDownloader
A bash script to download Panopto video files (tested only with UNIVR).
Using curl and pup, the script fetches the video link (screen shared and webcam) and the title, then using wget downloads the video (with the title as video name).
## Dependencies
1. pup (https://github.com/ericchiang/pup)
2. curl
3. wget
## How to install
1. Download this repo
2. Download and install all dependencies
3. Put the script file (panoptoDownloader) in one of the $PATH directories
4. Make a text file with one link (for UNIVR, it's the lesson link) per line, you can put as many links as you want
5. Use the script
## How to use the script
If the script is in $PATH
```bash
panoptoDownloader path/to/the/text/file where/to/save/videos
```
Otherwise
```bash
./panoptoDownloader path/to/the/text/file where/to/save/videos
```
Don't put another / after the video directory path

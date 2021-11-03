# FFbatchExtract

This is a pre-configured Windows batch file, along with FFmpeg binaries (gyan.dev build), that allow you to automate extracting video & audio streams/tracks from a folder of multi-track videos. The resulting files are invidiual videos of each stream/track and not re-encoded, simply copied.

# How To:
Extract the .rar (sorry, zip was too big for GitHub) to anywhere on the hard drive you like, then place the videos to be extracted in the "in" folder. Double click extract.bat to run the operation. When finished, the extracted videos will be in the "out" folder. Each file will be given a numbered suffix to denote the stream/channel that it was extracted from, i.e. _1, _2, _3 etc.

# Additional Notes:
Make sure the available space on the hard drive is at least double the size of all the multi-track videos to be processed, since FFMPEG will not delete the originals.

The batch operation is configured to extract up to 6 tracks/streams If more tracks are needed then you can simply add more lines to the .bat file, incrementing the stream and output suffix as so: 
![image](https://user-images.githubusercontent.com/7981637/140191022-fb0db160-6438-4a43-8143-6bc3bbcdd506.png)

You may see errors in the command prompt window when streams are not found in the original files, this is normal and expected as the batch operation is searching for up to 6 tracks to extract and most videos will not feature this many tracks, these errors/warnings will not affect the operation in any way.

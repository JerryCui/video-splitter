# video-splitter
A command line tool for automated video splitting. You can e.g. specify a file and an output directory and the script will use the `melt` command to search for scene changes and create a video file for the video part between each scene split (and the start and the end, of course). You might as well specify a directory to take input files from and let the script split thousands of file over night.

## Usage 
Invoke `python video_splitter.py -h` for usage information. Currently I didn't figure out `melt` yet, so there's no sound in the output. At a later point the `melt` parameters for clip creation should be configurable on the command line.

## Prerequisties
Make sure `pip` and the python templating engine `Cheetah` are installed (e.g. with `sudo apt-get install python-pip` on Ubuntu 14.10) and run `python setup.py build` (this will fetch all necessary dependencies) and install the aac codec (e.g. with `sudo apt-get install aac-enc` on Ubuntu 14.10).


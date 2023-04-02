# DPReview-Studio-Downloader
Originally created by [thatcherfreeman](https://github.com/thatcherfreeman/dpreview-studio-scraper). I've modified most of the code for my own purposes.

## Features:
- Preserves original file structure. Extremely important for metadata that is not logged such as E-Shutter and Pixel-Shift.

### New:
- Progress Bar.
- Skippable downloads. If image has already been downloaded, script will now automatically skip the download instead of redownloading all images from the beginning every time the script is run.
- Preserves original image file names and extensions.
- Script is now able to download multiple links per widget attribute. Previous script was only able to download one link per attribute, resulting in .acr.jpeg not downloading from the RAW drop down at all. In camera JPEG, RAW file, and .acr.jpeg all download correctly now.
- Check added for invalid characters **<>:"/\\|?***
- Removed .txt files containing metadata. Images already contain embeded EXIF and IPTC metadata.

## Requirements:
Progress bar requires [tqdm](https://pypi.org/project/tqdm/). To disable, comment out line 7 and 133 to 136.

## Optional:
I've included an optional .bat file to start the script in the current folder. Here is what it does.

- **This command points cmd/powershell to the current directory (folder the .bat is in). Files will download to this folder.**  
cd /D "%~dp0"

- **This command starts the python script automatically**  
python "DPReview Studio Downloader.py"

- **This command prevents cmd from exiting if their is an error or the download finishes. Users must manually close cmd. Very useful.**  
cmd /k

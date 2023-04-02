# DPReview-Studio-Downloader
Originally created by [thatcherfreeman](https://github.com/thatcherfreeman/dpreview-studio-scraper). I've modified most of the code for my own purposes.

## Features:
- Preserves original file structure. Extremely important for metadata that is not logged such as E-Shutter and Pixel-Shift.

### New:
- Progress Bar
- Skippable downloads. If image has already been downloaded, script will now automatically skip the download instead of redownloading all images from the beginning every time the script is run.
- Preserves original image file names and extensions.
- Script is now able to download multiple links per widget attribute. Previous script was only able to download one link per attribute, resulting in .acr.jpeg not downloading from the RAW drop down at all. In camera JPEG, RAW file, and .acr.jpeg all download correctly now.
- Check added for invalid characters **<>:"/\\|?***
- Removed .txt files containing metadata. Images already contain embeded EXIF and IPTC metadata.

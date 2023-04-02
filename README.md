# DPReview-Studio-Downloader
Originally created by [thatcherfreeman](https://github.com/thatcherfreeman/dpreview-studio-scraper). I've modified most of the code for my own purposes.

## Features:
- Preserves original image file names and extensions.
- Skippable downloads. If image has already been downloaded, script will now automatically skip the download instead of redownloading all images from the beginning every time the script is run.
- Script is now able to download multiple links per widget attribute. Previous script was only able to download one link per attribute, resulting in .acr.jpeg not downloading from the RAW drop down at all. In camera JPEG, RAW file, and .acr.jpeg all download correctly now.
- Check added for invalid characters **<>:"/\\|?***
- Preserves original file structure. Extremely important or metadata that is not logged such as E-Shutter and Pixel-Shift.
- Removed .txt files containing metadata. Images already contain embeded EXIF and IPTC metadata.

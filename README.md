# Only-Uploader

Forked from L4G Upload Assistant, thanks for all the work L4G on this tool and all the forks and updates. Shoutout Audionut and Uploarr

This fork is being maintained by OE.

A simple tool to take the work out of uploading.

## What It Can Do:
  - Generates and Parses MediaInfo/BDInfo.
  - Generates and Uploads screenshots.
  - Uses srrdb to fix scene filenames
  - Can grab descriptions from PTP (automatically on filename match or arg) / BLU (arg)
  - Obtains TMDb/IMDb/MAL identifiers.
  - Converts absolute to season episode numbering for Anime
  - Generates custom .torrents without useless top level folders/nfos.
  - Can re-use existing torrents instead of hashing new
  - Generates proper name for your upload using Mediainfo/BDInfo and TMDb/IMDb conforming to site rules
  - Checks for existing releases already on site
  - Uploads to OE/PTP/BLU/BHD/Aither/THR/R4E(limited)/HP/ACM/LCD/LST/NBL/ANT/FL/HUNO/RF/SN/RTF/OTW/FNP/CBR/UTP/AL/ULCX/HDB/YOINK/TVC/TIK/SPD/SHRI/PTT/PSS
  - Adds to your client with fast resume, seeding instantly (rtorrent/qbittorrent/deluge/watch folder)
  - ALL WITH MINIMAL INPUT!
  - Currently works with .mkv/.mp4/Blu-ray/DVD/HD-DVDs

  Built with updated BDInfoCLI from https://github.com/rokibhasansagar/BDInfoCLI-ng

  ## Image Hosts:
  - OnlyImage - oeimg
  - ImgBB - imgbb
  - PTPimg - ptpimg
  - ImageBox - imgbox
  - PixHost - pixhost
  - LensDump - lensdump
  - PTScreens - ptscreens

## Coming Soon:
  - Features
  - Rebase

## **Setup:**
   - **REQUIRES AT LEAST PYTHON 3.12 AND PIP3**
   - Needs [mono](https://www.mono-project.com/) on linux systems for BDInfo
   - Also needs MediaInfo and ffmpeg installed on your system
      - On Windows systems, ffmpeg must be added to PATH (https://windowsloop.com/install-ffmpeg-windows-10/)
      - On linux systems, get it from your favorite package manager
   - Clone the repo to your system `git clone https://github.com/edge20200/Only-Uploader.git`
   - Copy and Rename `data/example-config.py` to `data/config.py`
   - Edit `config.py` to use your information (more detailed information in the [wiki](https://github.com/edge20200/Only-Uploader/wiki))
      - tmdb_api (v3) key can be obtained from https://developers.themoviedb.org/3/getting-started/introduction
      - image host api keys can be obtained from their respective sites
   - Install necessary python modules `pip3 install --user -U -r requirements.txt`
     
   

   **Additional Resources are found in the [wiki](https://github.com/edge20200/Only-Uploader/wiki)**
   
   Feel free to contact me if you need help, I'm not that hard to find.

## **Updating:**
  - To update first navigate into the Upload-Assistant directory: `cd Only-Uploader`
  - Run a `git pull` to grab latest updates
  - Run `python3 -m pip install --user -U -r requirements.txt` to ensure dependencies are up to date
## **CLI Usage:**
  
  `python3 upload.py /downloads/path/to/content --args`
  
  Args are OPTIONAL, for a list of acceptable args, pass `--help`
## **Docker Usage:**
  Visit our wonderful [docker usage wiki page](https://github.com/edge20200/Only-Uploader/wiki/Docker)

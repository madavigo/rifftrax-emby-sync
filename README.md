# rifftrax-emby-sync
#### RiffTrax Emby Sync

#### About
RiffTrax.com produces comedic commentary tracks for a wide array of movies and other media. This Python script automates the process of adding newly downloaded RiffTrax commentaries to your Emby media server, ensuring they have the appropriate title and poster for easy navigation and playback.

### Features

Automatically renames MP4 files to match the EXIF Title metadata
Uploads the MP4 files to a designated NAS (Network-Attached Storage) via SCP (Secure Copy Protocol)
Refreshes the Emby library using Emby's API
Scrapes RiffTrax.com to fetch the appropriate poster for the commentary
Applies the fetched poster to the Emby library entry for the commentary

#### Prerequisites
Python 3.x
Perl Image ExifTool
Required Python libraries (requests, bs4, etc.)

##### Environment Variables

The following environment variables must be set:

EMBY_API_KEY: Your Emby API key

EMBY_BASE_URL: The base URL for your Emby servers api endpoint

#### Installation
Clone this repository: git clone https://github.com/madavigo/RiffTrax-Emby-Sync.git
Navigate to the directory: cd RiffTrax-Emby-Automator
Install the required Python packages: pip install -r requirements.txt

#### Usage
Open a terminal and navigate to the directory where the script is located.
Run the script: python script_name.py
When prompted, enter whether you want to delete the original files: Do you want to delete the original files? (yes/no):
The script will automatically process MP4 files found in the specified Downloads directory, rename them, upload them to your NAS, refresh the Emby library, and update the poster.

#### Contributing
If you would like to contribute or report issues, please feel free to open a GitHub issue or submit a pull request.
If you would like to contribute or report issues, please feel free to open a GitHub issue or submit a pull request.

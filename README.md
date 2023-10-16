# rifftrax-emby-sync
#### RiffTrax Emby Sync

#### About
RiffTrax.com produces comedic commentary tracks for a wide array of movies and other media. This Python script automates the process of adding newly downloaded RiffTrax commentaries to your Emby media server, ensuring they have the appropriate title and poster for easy navigation and playback.

### Features

1. Automatically renames MP4 files to match the EXIF Title metadata
2. Uploads the MP4 files to a designated NAS (Network-Attached Storage) via SCP (Secure Copy Protocol)
3. Refreshes the Emby library using Emby's API
4. Scrapes RiffTrax.com to fetch the appropriate poster for the commentary
5. Applies the fetched poster to the Emby library entry for the commentary

#### Prerequisites
Python 3.x
Perl Image ExifTool
Required Python libraries (requests, bs4, etc.)

##### Environment Variables

The following environment variables must be set:

EMBY_API_KEY: Your Emby API key

EMBY_BASE_URL: The base URL for your Emby servers api endpoint

#### Installation
1. Clone this repository: git clone https://github.com/madavigo/rifftrax-emby-sync.git
2. Navigate to the directory: cd rifftrax-emby-sync
3. Install the required Python packages: pip install -r requirements.txt

#### Usage
Open a terminal and navigate to the directory where the script is located.
Run the script: rifftrax or python rifftrax
When prompted, enter whether you want to delete the original files: Do you want to delete the original files? (yes/no):
The script will automatically process MP4 files found in the specified Downloads directory, rename them, upload them to your NAS, refresh the Emby library, and update the poster with the poster found at the RiffTrax website..

#### Contributing
If you would like to contribute or report issues, please feel free to open a GitHub issue or submit a pull request.

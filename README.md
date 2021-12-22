<h1 align="center">ytcd - YouTube channel downloader script</h1>
<p>
  <a href="#" target="_blank">
    <img alt="License: GPLv3" src="https://img.shields.io/badge/License-GPLv3-yellow.svg" />
  </a>
</p>

## Requirements

To use the script you must have [yt-dlp](https://github.com/yt-dlp/yt-dlp) installed.

## Usage

The channels to be downloaded and the download path must be edited in the `init()` function; the rest of the script can be left untouched. The test entries should be replaced with your own, this may look like this:
    
```sh
# Download folder
path="/home/sadirde/downloads"
    
# Channel URLs
channels[jawed]="https://www.youtube.com/user/jawed"
channels[youtube]="https://www.youtube.com/c/youtube"
channels[t-series]="https://www.youtube.com/aashiqui2"
```

There are two commands, firstly to download all channels:

```sh
./ytcd channels
```

and secondly to download a specific channel:

```sh
./ytcd channel name-of-channel
```

Replace `name-of-channel` with a name you specified in the `init()` function, for example `./ytcd channel t-series`.

In addition to the videos, JSON files containing the metadata about the videos and the channel are downloaded and stored in the "info" folder.

## License

ytcd is free and open-sourced software licensed under the [GNU General Public License v3.0](https://www.gnu.org/licenses/gpl.html).

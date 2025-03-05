# YouTube Media Downloader

## Overview

This script allows users to download and convert YouTube videos and playlists into MP3 or MP4 formats. It utilizes `yt-dlp` for downloading and `ffmpeg` for conversion, ensuring high-quality media processing.

## Features

- Download YouTube videos or entire playlists
- Convert downloaded videos to MP4 or MKV format
- Supports multiple quality options for both audio and video
- Uses `yt-dlp` for reliable downloads
- Uses `ffmpeg` for high-quality media conversion

## Prerequisites

Ensure you have the following installed on your system:

- **Python** (latest version recommended)
- **yt-dlp** (`pip install yt-dlp`)
- **ffmpeg** (install via package manager or download from [ffmpeg.org](https://ffmpeg.org))

## Installation

1. Clone or download the script.
2. Ensure `yt-dlp` and `ffmpeg` are installed and accessible from the command line.

## Usage

Run the script in a terminal:

```sh
python script.py
```

Follow the prompts:

1. Enter the YouTube video or playlist URL.
2. Choose whether to download an entire playlist or a single video.
3. Select the file type (`mp3` or `mp4`).
4. Select the quality level (`low`, `medium`, or `high`).
5. If downloading an MP4 file, you may choose to convert it to another format.

### Example Usage

**Download a single video in MP4 format with high quality:**

```
Enter YouTube URL: https://www.youtube.com/watch?v=example
Enter file type (mp3/mp4): mp4
Enter quality (default: medium): high
```

**Download an MP3 file with medium quality:**

```
Enter YouTube URL: https://www.youtube.com/watch?v=example
Enter file type (mp3/mp4): mp3
Enter quality (default: medium): medium
```

## Output

- All downloaded media will be stored in the `output/` directory.
- Converted video files will be stored in the same directory with the chosen format.

## Notes

- If a playlist URL is provided, the script will prompt you to download the full playlist or just a single video.
- MP4 files are downloaded in the best available format up to the selected resolution.
- MP3 files are extracted with the specified bitrate.
- Conversion only applies to MP4 files and supports MP4 and MKV formats.

## License

This script is open-source and available for use and modification under the MIT License.

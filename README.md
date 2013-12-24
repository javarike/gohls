# gohls

gohls - HTTP Live Streaming (HLS) downloader written in Golang


* Current version: **1.0.1**
* Author: Kevin Zhang
* License: [GNU GPL version 3](http://www.gnu.org/licenses/gpl-3.0.txt)

## [Download (source and binaries)](https://github.com/kz26/gohls/releases)

Download the source distribution for a tagged stable release, or download binaries for your platform.
Currently, binaries are available for the following platforms:

* Windows 64-bit

## Usage, options, and defaults

`gohls [-l=bool] [-t duration] [-ua user-agent] media-playlist-url output-file`

* -l=false: Use local time to track duration instead of supplied metadata
* -t=0: Recording duration (0 == infinite)
* -ua="Mozilla/5.0 (Windows NT 6.3; WOW64; rv:26.0) Gecko/20100101 Firefox/26.0": User-Agent for HTTP client

The recording duration should be specified as a Go-compatible [duration string](http://golang.org/pkg/time/#ParseDuration).

## TODO

* Encrypted streams support?
* Proper Ctrl-C handling

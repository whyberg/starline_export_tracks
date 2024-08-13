# starline_export_tracks
Console utility for export GPS/GLONAS tracks from starline.ru to json/GPX/kml.
OTP authentication is used for access Starline.ru, you need get OTP from your StarLine 2 app

##  Prerequisites
This project requires Python3

## Installation

**BEFORE YOU INSTALL:** please read the [prerequisites](#prerequisites)

Start with cloning this repo on your local machine:

```sh
$ git clone https://github.com/whyberg/starline_export_tracks.git
$ cd PROJECT
```

Create virtual environment for python3

```sh
python3 -m venv ./dist/python3
./dist/python3/bin/pip install -r requirements.txt
```

Start utility

```sh
starline_export_tracks -h
```

Authentication by OTP

```sh
starline_export_tracks -p 13461959
```

Get connected devices

```sh
starline_export_tracks -l
```

Export tracks to stdout json fomrat

```sh
starline_export_tracks -w [device_id from the previous request] -f [Start Date/Time] -t [Stop date/time]
```

Export tracks to file json format

```sh
starline_export_tracks -w [device_id from the previous request] -f [Start Date/Time] -t [Stop date/time] -n [filename]
```

Export tracks to file gpx format

```sh
starline_export_tracks -w [device_id from the previous request] -f [Start Date/Time] -t [Stop date/time] -g -n [filename]
```

Export tracks to file kml format

```sh
starline_export_tracks -w [device_id from the previous request] -f [Start Date/Time] -t [Stop date/time] -k -n [filename]
```

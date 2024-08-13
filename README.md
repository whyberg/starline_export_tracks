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

[![pypi-total-downloads](https://img.shields.io/pypi/dm/mangadex-downloader?label=DOWNLOADS&style=for-the-badge)](https://pypi.org/project/mangadex-downloader)
[![python-ver](https://img.shields.io/pypi/pyversions/mangadex-downloader?style=for-the-badge)](https://pypi.org/project/mangadex-downloader)
[![pypi-release-ver](https://img.shields.io/pypi/v/mangadex-downloader?style=for-the-badge)](https://pypi.org/project/mangadex-downloader)


# mangadex-downloader

Download manga from Mangadex through Python

## Key Features

- Download manga directly with python from mangadex
- [Tachiyomi](https://github.com/tachiyomiorg/tachiyomi) support (Local files support)

## Installation

### From PyPI

```shell
# For Windows
py -3 -m install mangadex-downloader

# For Linux / Mac OS
python3 -m pip install mangadex-downloader
```

### From Git 

**NOTE:** You must have git installed. If you don't have it, install it from here https://git-scm.com/.

```shell
# For Windows
py -3 -m pip install git+https://github.com/mansuf/mangadex-downloader.git@v0.1.0

# For Linux / Mac OS
python3 -m pip install git+https://github.com/mansuf/mangadex-downloader.git@v0.1.0
```

## Usage

**NOTE:** This app will download manga in english language only. Other languages are implemented soon.

### Command Line Interface (CLI)

Options

```
positional arguments:
  URL                   MangaDex URL

options:
  -h, --help            show this help message and exit
  --folder FOLDER       Store manga in given folder
  --proxy SOCKS / HTTP Proxy
                        Set http/socks proxy
  --proxy-env           use http/proxy from environments
  --verbose             Enable verbose output
```

Usage

```shell

mangadex-dl "insert MangaDex URL here" 
# or
mangadex-downloader "insert MangaDex URL here" 

# Use this if "mangadex-dl" or "mangadex-downloader" didn't work

# For Windows
py -3 -m mangadex-downloader "insert MangaDex URL here" 

# For Linux / Mac OS
python3 -m mangadex-downloader "insert MangaDex URL here" 
```

### Embedding (API)

```python
from mangadex_downloader import download

# The parameters are:
# - url: str
# - folder: str (default: None)

download("insert MangaDex URL here")
```

## Minimum Python version
```
Python 3.5.x
```

## Issues

You can open a issue [here](https://github.com/mansuf/mangadex-downloader/issues), if its related to Mangadex.
<br>
For more information, click [here](https://github.com/mansuf/mangadex-downloader/blob/main/CONTRIBUTING.md#Issues)

## Contributing

You can check the guidelines [here](https://github.com/mansuf/mangadex-downloader/blob/main/CONTRIBUTING.md)

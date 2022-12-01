## Installation:
- Python 3.6 or later is required.
- First, please make sure that the latest pip version is installed in your working environment.
```
python -m pip install -U pip
```
- Run the following command given below to install the package:
```
python -m pip install -U YouTubeMusicAPI
```

## Get Started
- Here is an example program.
```py
import YouTubeMusicAPI

query: str = "alan walker faded"

result = YouTubeMusicAPI.Search(query)

if result:
    print(result)
else:
    print("No Result Found")
```
- If a result for your search query is found while running the above program, it will return an **dict object**; otherwise, it will return **None**. 
```json
{
    "trackName": "...",
    "trackId": "...",
    "trackUrl": "...",
    "artworkUrl": "...",
    "artistName": "...",
    "artistUrl": "..."
}
```

## Building from source code:
- Clone the repository
```
git clone https://github.com/cj-praveen/YouTube-Music-API.git
```
- cd into the directory
```
cd YouTube-Music-API
```
- Install dependencies
```
python -m pip install -U build setuptools
```
- on Linux / macOS:
```
sudo apt-get install python3-venv
```

- Run the following command given below to build:
```
python -m build
```

# ***Zingmp3***
Zingmp3 - A tool crawl data from [`zingmp3.vn`](https://zingmp3.vn/).

[![Capture.png](https://i.postimg.cc/5tm0NNkk/Capture.png)](https://postimg.cc/Ny5YdYt1)

## ***Installation***
 - **Language**: Python3.x
 
 - **Module**: requests, colorama
    ```
    pip install -r requirements.txt
    ``` 

## ***exe version***
- [`driver`](https://drive.google.com/file/d/1BMbwAjXJP_VB-M6N81OVgat3w79lCLyU/view) or [`mediafire`](https://www.mediafire.com/file/l51hoj6n4qy2baw/zingmp3.rar/file)

[![Capture.png](https://i.postimg.cc/0y138xD6/Capture.png)](https://postimg.cc/D855g9CF)


## ***Options***
  - `-c` or `--cookie`: Add cookies to auth
  - `-j` or `json` : Show json of info media. 
  - `-s` or `--save` : Path to save file downloaded.
  - `-l` or `--lyric` : Download with lyric.
  - Default will download all media and lyric.
  - All the example in Usage.
 
## ***All URL Supported***
- **url media**
    ```
    https://zingmp3.vn/video-clip/.../<id>.html
    https://zingmp3.vn/bai-hat/.../<id>.html
    https://zingmp3.vn/playlist/.../<id>.html
    https://zingmp3.vn/album/.../<id>.html
    https://zingmp3.vn/embed/.../<id>.html
    ```
- **url artist's profile type 1**
    ```
    https://zingmp3.vn/nghe-si/<name_artist>/video
    https://zingmp3.vn/nghe-si/<name_artist>/playlist
    https://zingmp3.vn/nghe-si/<name_artist>/bai-hat
    https://zingmp3.vn/nghe-si/<name_artist>/album
    ```
- **url artist's profile type 2**
    ```
    https://zingmp3.vn/<name_artist>/bai-hat
    https://zingmp3.vn/<name_artist>/playlist
    https://zingmp3.vn/<name_artist>/video
    https://zingmp3.vn/<name_artist>/album
    ```
- **url #ZINGCHART**
    ```
    https://zingmp3.vn/zing-chart/bai-hat.html
    https://zingmp3.vn/zing-chart/video.html
    https://zingmp3.vn/zing-chart-tuan/bai-hat-Viet-Nam/<id>.html
    https://zingmp3.vn/zing-chart-tuan/video-US-UK/<id>.html
    ```
- **url new release**
    ```
    https://zingmp3.vn/top-new-release/index.html
    ```
 
## ***How to get cookies.txt for login***
 If you want to use your account VIP to download quality list 320 or lossless
 
 1. Download extension from chrome store [`cookies.txt`](https://chrome.google.com/webstore/detail/cookiestxt/njabckikapfpffapmjgojcnbfjonfjfg)
 2. Go to page [`zingmp3`](https://zingmp3.vn/)
 3. Click to icon cookies.txt just download
 4. Click to `click here` and save file cookies.txt
 5. Get cookies.txt then put it to them same path with tool, then run
 
 Sometime cookies will die, Pls follow the steps above to update the new cookies.
  
 If you don't set cookies, tool will download default quality like 128 ...
## ***Usage***
```
$ python zingmp3.py -h
usage: zingmp3.py [-h] [-c] [-s] [-j] [-l] url

Zingmp3 - A tool crawl data from zingmp3.vn .

positional arguments:
  url             Url.

optional arguments:
  -h, --help      show this help message and exit

Authentication:
  -c , --cookie   Cookies for authenticate with.

Options:
  -s , --save     Path to save
  -j, --json      Show json of info media.
  -l, --lyric     Download only lyric.
```
 - **Install module**
    ```
    pip install -r requirements.txt
    ```
 - **Run**
    ```
    python zingmp3.py https://zingmp3.vn/bai-hat/Khoc-Cung-Em-Mr-Siro-Gray-Wind/ZWBI0DFI.html
    ``` 
 - **Download with cookies**
  
    ```
    python zingmp3.py -c cookies.txt https://zingmp3.vn/bai-hat/Khoc-Cung-Em-Mr-Siro-Gray-Wind/ZWBI0DFI.html
    ```
 - **Set quality want download**
 
    No cookies
    ```
    python zingmp3.py -q lossless https://zingmp3.vn/bai-hat/Khoc-Cung-Em-Mr-Siro-Gray-Wind/ZWBI0DFI.html
    ```
    
    with cookies
    ```
    python zingmp3.py -c cookies.txt -q lossless https://zingmp3.vn/bai-hat/Khoc-Cung-Em-Mr-Siro-Gray-Wind/ZWBI0DFI.html
    ```
    
    Video
    ```
    python zingmp3.py -q 1080 https://zingmp3.vn/video-clip/Em-Gi-Oi-Jack-K-ICM/ZWAEFWIF.html
    ```
    
 - **Show json of info media**
     ```
     python zingmp3.py -j https://zingmp3.vn/bai-hat/Khoc-Cung-Em-Mr-Siro-Gray-Wind/ZWBI0DFI.html
     ```

## ***Note***
- All file downloaded in folder DOWNLOAD at the same path
- If there's an error or problem, please write issue out here
 [`zingmp3 issues`](https://github.com/hatienl0i261299/Zingmp3_api/issues)
- FB: 100011734236090

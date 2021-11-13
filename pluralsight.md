# Download Pluralsight Videos

- Login into Pluralsight.com using your Username and Password.
- Install following `Get cookies.txt` Chrome extension (https://chrome.google.com/webstore/detail/get-cookiestxt/bgaddhkoddajcdgocldbbfleckgcbcid)
- Now go to Pluralsight page and export the cookie using `Get cookies.txt` Chrome extension

<img src="./get-cookie.jpg" style="width:100%">

- Next create cookies.txt file and paste export cookie content in it.
- Now use following `youtube-dl` command to download videos


### Download with subtitle

```bash
youtube-dl --cookies "./cookies.txt" --user-agent "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/95.0.4638.69 Safari/537.36" --sleep-interval 35 --max-sleep-interval 120 --all-subs --sub-format srt --write-sub --verbose https://app.pluralsight.com/library/courses/docker-networking-managing
```

### Download without subtitle

```bash
youtube-dl --cookies "./cookies.txt" --user-agent "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/95.0.4638.69 Safari/537.36" --sleep-interval 35 --max-sleep-interval 120  --verbose https://app.pluralsight.com/library/courses/docker-networking-managing
```

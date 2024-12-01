# M3U8-Proxy
Proxies m3u8 files.

## Usage
To proxy m3u8 files, use the `/m3u8-proxy` route. All you have to do is input the URL and headers. For example:
```
http://localhost:3030/m3u8-proxy?url=https%3A%2F%2Fojkx.vizcloud.co%2Fsimple%2FEqPFJvsQWADtjDlGha7rC8UurFwHuLiwTk17rqk%2BwYMnU94US2El_Po4w12gXe6GptOSQtc%2Fbr%2Flist.m3u8%23.mp4&headers=%7B%22referer%22%3A%22https%3A%2F%2F9anime.pl%22%7D
```
The URL in this case is `https://ojkx.vizcloud.co/simple/EqPFJvsQWADtjDlGha7rC8UurFwHuLiwTk17rqk+wYMnU94US2El_Po4w12gXe6GptOSQtc/br/list.m3u8#.mp4` and the headers are `{"Referer": "https://9anime.pl"}`. This will then send a request to the m3u8 using the headers, modify the content to use the ts proxy, then proxy each ts file using a CORS proxy.

## Installation
1. Run `npm i`.
2. Run `npm run build`.
3. Run `npm start`.

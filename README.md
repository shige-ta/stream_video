## video.js AWSでストリーミング配信サイト作成メモ



参考サイト
https://dev.classmethod.jp/articles/video-js-play-hls-streaming-s3-cloudfront-cors/

https://akiyoko.hatenablog.jp/entry/2015/08/24/192618

https://kimbio.info/video-js-autoplay/

https://akiyoko.hatenablog.jp/entry/2015/08/11/015852

https://youtu.be/3ykzi358sK8


## CORS ポリシー

```json
[
    {
        "AllowedHeaders": [
            "*"
        ],
        "AllowedMethods": [
            "GET"
        ],
        "AllowedOrigins": [
            "*"
        ],
        "ExposeHeaders": [],
        "MaxAgeSeconds": 3000
    }
]
```

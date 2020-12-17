## video.js AWSでストリーミング配信サイト作成メモ



参考サイト
https://dev.classmethod.jp/articles/video-js-play-hls-streaming-s3-cloudfront-cors/

https://akiyoko.hatenablog.jp/entry/2015/08/24/192618

https://kimbio.info/video-js-autoplay/

https://akiyoko.hatenablog.jp/entry/2015/08/11/015852

https://youtu.be/3ykzi358sK8


## バケットポリシー

```json
{
  "Id": "Policy1434989802960",
  "Version": "2012-10-17",
  "Statement": [
    {
      "Sid": "Stmt1434989800735",
      "Action": [
        "s3:GetObject"
      ],
      "Effect": "Allow",
      "Resource": "arn:aws:s3:::xxxxx/*",
      "Principal": "*"
    }
  ]
}
```


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

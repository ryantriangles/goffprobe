# go-ffprobe

Go wrapper around ffprobe, providing a simplified breakdown of video and audio
file attributes.

```
>> info := NewVideoInfo("foo.mp4")
>> info.SimpleDescription
"h264+av1@2700000/aac@256000"
>> info.Pixels // Pixel count of highest-resolution video stream
414720
>> info.Duration // Seconds
618
>> info.HasMultipleVideo
true
>> info.AudioBitrate
256000
>> info.VideoBitrates
1800000, 900000
```

# License (MIT)

© 2022 Ryan Plant

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

# BadApple-LCD1602

## Usage

Use your favorite C compiler to compile `pic-encoder.c`, then run:
```
ffmpeg -i "*FileIn*" -vf colorchannelmixer=.299:.587:.114:0:.299:.587:.114:0:.299:.587:.114,scale=23:17:flags=lanczos -pix_fmt gray -f rawvideo - | pic-encoder
```
(replace `*FileIn*` with your video file) to generate binary file (`out.bin`).

Then, copy the binary file to a SD Card, connect SD card to an Arduino, download the sketch and enjoy!

## Lyrics?

Lyrics generator is working in progress, please wait a moment...

# Create gif from video
```sh
ffmpeg -ss 3 -t 3 -i test.avi \
    -vf "fps=10,scale=720:-1:flags=lanczos,split[s0][s1];[s0]palettegen[p];[s1][p]paletteuse" \
    -loop 0 output.gif
```
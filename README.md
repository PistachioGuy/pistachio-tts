# tts
My python text to speech project
<br>
Requirements:
 - python3
 - ffmpeg
 - pydub

options:
```  -h, --help            show this help message and exit
  -i INPUT, --input INPUT
  --decompress          Decompress recordings to raw uncompressed wavs instead of mp3s. This takes up a bit more storage but makes generation of long
                        texts multiple times faster. Use this arguement every time you want to use uncompressed training data, otherwise it will default to
                        compressed.
  --del-uncompressed    Delete uncompressed training data generated by --decompress to save space.
  --debug               Long debug output
```
<br>
Example usage:
```
python3 tts.py --decompress -i "The quick brown fox jumped over the lazy dog"
```
<br><br>
It's reccomended that you always use --decompress, it only takes an extra 16 megabytes (instead of 3) for the recordings, and makes it many times faster.

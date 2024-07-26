# Watermark

A Python script that recursively adds a logo or watermark to all of the photos
in a given directory and all of its subdirectories.

## Output

<p align="center">
   <img src="output.gif">
</p>

### Requirements

Pillow:

```
pip install pillow
```

[Pillow Docs](https://python-pillow.github.io/)

### Installation

```
git clone https://github.com/NjauSamuel/Python_Watermark.git
```

### Application

Using this script, you should assign images in a certain folder and its
subdirectories a watermark or a logo. The script accepts the following
arguments:

1. The folder with the images you want to watermark
2. The path of the logo to add
3. The position you want to place the logo (optional)
4. The directory where you want to save the watermarked images (optional; if not
   provided, the watermarked images will overwrite the original images)
5. Padding (in pixels) around the watermark logo (optional; default is 0)

These are the valid positions:

-  topleft
-  topright
-  bottomleft
-  bottomright
-  center (if no position is specified, this will be the default)

Any other position will result in an error.

To start using watermark.py, specify your original images folder, the watermark
location, a position to place the watermark, a destination directory, and scale
the watermark to 30% of the image width (optional):

```
python watermark.py './images' 'logo.png' --pos bottomright --new_dir './watermarked_images' --scale 30
```

To add padding around the watermark:

```
python watermark.py './images' 'logo.png' --pos topleft --padding 20


```

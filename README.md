# image-convert

**image-convert** tool allows you to convert images to different formats on GNU/Linux, macOS and Windows systems.



## Contents
- [Supported OS](#supported-os)
- [Prerequisites](#prerequisites)
- [Supported formats](#supported-formats)
- [Installation](#installation)
- [Available options](#available-options)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)



## Supported OS
- GNU/Linux
- Windows
- macOS



## Prerequisites
- [Python3](https://www.python.org/downloads/)
- [Pillow](https://pypi.org/project/Pillow/): Install using `pip install Pillow`



## Supported formats
- JPEG
- PNG
- WEBP
- TIFF
- BMP
- ICO
- ICNS
- PBM
- PGM
- PPM



## Installation
**1. Clone this repo:**
```
git clone https://github.com/the-weird-aquarian/image-convert.git
```

**2. Move into the project directory:**
```
cd image-convert
```

**3. Give executable permissions to the script (Not required for Windows):**
```
chmod +x image-convert
```



## Available options:
```
-h, --help              Show this help message and exit
-f, --formats           Show a list of supported output formats
-i, --input-files       Path to the input image files
-o, --output-format     Output format (e.g.: png, jpeg, etc.)
-d, --directory         Output directory for converted images
-l, --lossy             Perform lossy conversion (default: lossless, except for JPEG)
-p, --parallel          Convert images in parallel
```

**NOTE**:
If -p/--parallel option is used, multiple images will be read in parallel.
This will be faster, however, it might use a lot of system resources if too many images are provided.



## Usage
```
python3 image-convert -i <image> -o <output format>
```

```
python3 image-convert -i <image1> <image2> <image3> -o <output format>
```

**Examples:**
```
python3 image-convert -i icon.png -o jpeg
```

```
python3 image-convert -i icon1.png icon2.jpg icon3.webp -o tiff -d /home/user/Downloads
```

```
python3 image-convert -i icon1.png icon2.jpg -o webp -l -p
```



## Contributing
Pull requests can be submitted [here](https://github.com/the-weird-aquarian/image-convert/pulls).



## License
This project is licensed under the terms of [GPLv3 license](https://github.com/the-weird-aquarian/image-convert/blob/main/LICENSE).

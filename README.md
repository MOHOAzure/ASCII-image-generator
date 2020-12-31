# ASCII-image-generator
A generator, which accept an image file, for example jpg, and convert it to an ASCII image art.

## Dependency
- numpy
- Pillow

## How to use
- prepare a image

- command
    - format : python .\ascii_image_generator.py --file {input image}
    - example: python .\ascii_image_generator.py --file input/image.jpg --cols 200
    - required args:
        - file:         Input file name, for example, input/img.jpg
    - optional args:
        - out:          Output file name, for example, ascii_art.txt
        - cols:         Width of tile. The larger the cols is, the more clearer the output art is.
        - scale:        Scaled height
        - morelevels:   Look up ascii char for detailed presentation. No value should be provided for this arg.
        
- check the generated ascii art in the output file
        
## Demo

### Input image
- input/image.jpg

### Command & ASCII art
python .\ascii_image_generator.py --file input/image.jpg --out output/ascii_art.txt --cols 200

- output/ascii_art.txt

python .\ascii_image_generator.py --file input/image.jpg --out output/ascii_art_detailed.txt --morelevels --cols 200

- output/ascii_art_detailed.txt
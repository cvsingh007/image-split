# image-split

**Quickly split an image into rows and columns (tiles).**

[split-image](https://pypi.org/project/split-image/) is a Python package that you can use from the command line to split an image into tiles.

![alt text](https://drive.google.com/uc?id=1cdbBrS675gj5aDm5zM7ZuPB1M_qv8Hvk)

**Installation**

`pip install split-image`

**Usage**
```
from split_image import split_image

split_image(image_path, rows, cols, should_square, should_cleanup, [output_dir])
# e.g. split_image("bridge.jpg", 2, 2, True, False)
```

**Basic examples**

`split_image("/content/cat.png", 15, 8, False, False,"/content/")`

This splits the cat.png image in 4 tiles (2 rows and 2 columns).
![alt text](https://drive.google.com/uc?id=1l3xu6QyrUPF_WpFwR3PYTGkd2p5EFEMa)

`split_image("/content/bridge.png", 3, 4, True, False,"/content/")`

This splits the `bridge.png` image in 12 tiles (3 rows and 4 columns). The square arguments `True` resizes the image into a square before splitting it. The background color used to fill the square is determined from the image automatically.

![alt text](https://drive.google.com/uc?id=1bCZ0_bK9PixrhVdAAn1h5b-2wQD17hQP)

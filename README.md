# Style-My-Pic

A simple, modular implementation of Neural Style Transfer (NST) designed for research purposes. This project provides a pipeline for transferring artistic style from one image (style image) to another (content image), inspired by the paper "A Neural Algorithm of Artistic Style" by Gatys et al.

## Directory Structure
```
samanton-j-style-my-pic/
├── README.md
├── NST.py
├── requirements.txt
├── requirements_macos.txt
├── data/
│   ├── .DS_Store
│   ├── content-images/
│   └── style-images/
└── models/
    └── definitions/
        ├── vgg19.py
        └── __pycache__/
```

## Features
- Uses VGG19 as the base feature extractor.
- Clean separation of style and content representation.
- Easily extensible with different model backbones.
- Compatible with macOS and other platforms.

## Installation
```bash
pip install -r requirements.txt  # For general systems
pip install -r requirements_macos.txt  # For macOS
```

## Usage
To perform style transfer:
```bash
python NST.py --content data/content-images/your_image.jpg --style data/style-images/your_style.jpg
```

## Output
The output will be a stylized image saved in the project directory with a default name like `output.jpg`.

## Models
The `models/definitions/` folder includes the VGG19 architecture adapted for NST.

## Dataset
Place your own images in the `content-images/` and `style-images/` folders respectively.

## TODO
- Add support for real-time webcam-based NST
- Support for batch processing of multiple images
- Add perceptual loss variants for style enhancement

## License
MIT License

---

For academic or personal research use only. Feel free to modify and expand.


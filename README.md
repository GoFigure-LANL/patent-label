# GoFigure/patent-label
Read figure labels from patent drawings.

## Installation

Packages needed:
- PIL or pillow
- scipy
- skimage
- pytesseract


## Usage

Write an output.csv file with the name of the input image, bounding box, and OCR text result; with one entry line per bounding box:
```bash
python label_extraction.py --image_path [path_to_images]
```

Full help message with options:
```bash
python label_extraction.py -h
```

## Evaluating results

The regular expression parser and the python script to calculate the precision and recall is in find_only_label.py.
All the .txt files in east_png_results_new.zip is used together with find_only_label.py.


## Acknowledgements

If you find this code useful, please cite:
- Ming Gong, Xin Wei, Diane Oyen, Jian Wu, Martin Gryder, and Liping Yang. Recognizing Figure Labels in Patents. In *AAAI Workshop on Scientific Document Understanding*. 2021.


## License
BSD-3. See [LICENSE](LICENSE).

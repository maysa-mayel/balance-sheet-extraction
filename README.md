# Table Extraction and Text Recognition from Balance Sheets

## Overview
This project focuses on extracting tabular data from balance sheets (bilan) using a combination of advanced machine learning techniques. The pipeline involves detecting tables and their structures, recognizing text within each cell, and saving the extracted data into a CSV file for further analysis.

## Features
- **Table Detection**: Utilizes the Table Transformer model to detect tables and their structures within balance sheets.
- **Text Extraction**: Uses PaddleOCR for extracting text from each cell of the detected tables.
- **CSV Output**: Saves the extracted data into a CSV file for easy review and analysis.

## Requirements
To run this project, you need the following Python packages:

- `transformers`
- `timm`
- `pdf2image`
- `pandas`
- `paddlepaddle-gpu`
- `paddleocr`
- `torch`
- `numpy`
- `matplotlib`
- `opencv-python`
- `Pillow`

You can install these dependencies using pip:

```bash
pip install git+https://github.com/huggingface/transformers.git
pip install timm pandas pdf2image transformers matplotlib numpy paddlepaddle-gpu==2.5.1.post112 -f https://www.paddlepaddle.org.cn/whl/stable.html
pip install paddleocr torch opencv-python Pillow
```
Using the Table Transformer model for table detection and structure recognition.
Applying PaddleOCR to extract text from detected cells.
Saving the results to a CSV file for easy review and analysis.

**Contributing**
If you'd like to contribute to this project, please fork the repository, make your changes, and submit a pull request. We appreciate your help in improving this tool!

**License**
This project is licensed under the MIT License. See the LICENSE file for detail

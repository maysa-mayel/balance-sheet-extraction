#Table Extraction and Text Recognition from Balance Sheet
**Overview**
This project extracts tabular data from balance sheets (bilan) using a combination of advanced machine learning techniques. The process involves:

Detecting tables and their structure using the Table Transformer model.
Recognizing text within each cell using PaddleOCR.
Saving the extracted data into a CSV file for further analysis.
Features
Table Detection: Utilizes the Table Transformer model to detect tables and their structure.
Text Extraction: Uses PaddleOCR for extracting text from individual table cells.
CSV Output: Saves the extracted text in a CSV file for easy analysis.
Requirements
To run this project, you need the following Python packages:

transformers
timm
pdf2image
pandas
paddlepaddle-gpu
paddleocr
torch
numpy
matplotlib
opencv-python
Pillow
You can install these dependencies using pip:

bash
Copy code
pip install git+https://github.com/huggingface/transformers.git
pip install timm pandas pdf2image transformers matplotlib numpy paddlepaddle-gpu==2.5.1.post112 -f https://www.paddlepaddle.org.cn/whl/stable.html paddleocr
Setup
Clone the Repository

bash
Copy code
git clone https://github.com/yourusername/your-repository.git
cd your-repository
Install Dependencies

Follow the instructions in the Requirements section to install necessary Python packages.

Prepare Your Data

Place your balance sheet PDF (exp bilan.pdf) in the project directory.

Usage
Run the Notebook

Open the Jupyter Notebook file (table_extraction_on_bilan.ipynb) and execute each cell sequentially. The notebook performs the following steps:

Converts the PDF to an image.
Applies the Table Transformer model to detect and recognize table structures.
Uses PaddleOCR to extract text from each cell within the detected tables.
Saves the extracted text into a CSV file.
Review Results

After running the notebook, the extracted data will be saved in bilan.csv. You can open this file to view the extracted text in a tabular format.

Example
The notebook demonstrates:

Using the Table Transformer model for table detection and structure recognition.
Applying PaddleOCR to extract text from detected cells.
Saving the results to a CSV file for easy review and analysis.
**Contributing**
If you'd like to contribute to this project, please fork the repository, make your changes, and submit a pull request. We appreciate your help in improving this tool!

**License**
This project is licensed under the MIT License. See the LICENSE file for detail

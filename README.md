# Document Scanner & OCR Text Extractor

A Computer Vision-based project that transforms document images into clean, scanned documents and extracts their text using OCR.

**Author:** ARYAN
**Registration No.:** 24BAI10586
**Course:** Computer Vision

## Features

* Detects documents in images using OpenCV.
* Performs perspective correction and improves the scanned document.
* Extracts text from documents using EasyOCR.
* Filters OCR results based on confidence scores.
* Saves the generated results in PNG, TXT, JSON, and PDF formats.
* Supports both single-image and batch image processing.

## Technologies Used

Python, OpenCV, NumPy, EasyOCR, FPDF2, Pytest

## Project Structure

```text
Document_scanner_using_ocr/
├── diagrams/
├── input/
├── output/
├── src/
├── tests/
├── README.md
├── requirements.txt
└── statement.md
```

## Setup

Clone the repository and install the required dependencies:

```bash
git clone https://github.com/mohitpoonia21/Document_scanner_using_ocr.git
cd Document_scanner_using_ocr
pip install -r requirements.txt
```

## Run

Place a document image in the `input` folder and run:

```bash
python -m src.cli --input input/your_document.jpg --output output
```

For processing multiple images at once:

```bash
python -m src.cli --input-dir input --output output
```

## Testing

Run the test suite using:

```bash
pytest -q
```

**Result:** 13 tests passed

## Output

The application can generate the following files:

* `document_scan.png`
* `document.txt`
* `document.json`
* `document.pdf`

## Note

The complete OCR process requires EasyOCR along with its model files. During development, the OCR wrapper was tested with mocks because the required package and model download were not available in the testing environment.

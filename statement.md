# Project Statement

## Document Scanner Using OCR

**Name:** ARYAN
**Registration No.:** 24BAI10586
**Domain:** Computer Vision

## Problem Statement

Images of documents can often have problems such as tilted pages, unnecessary backgrounds, uneven illumination, and other distortions. These problems can reduce the quality of the document image and may also interfere with accurate text recognition.

The objective of this project is to create a simple document scanner that can identify a document in an image, correct its perspective, enhance the scanned output, and extract the text using OCR technology.

## Proposed Solution

The project is developed in Python using OpenCV and EasyOCR. The complete system is organized into three primary modules.

### Module 1 — Preprocessing

The system first validates the input image, identifies the document's edges and boundaries, detects its four corners, performs perspective correction, and enhances the final scanned image.

### Module 2 — OCR

The enhanced document image is provided to EasyOCR for text recognition. The extracted OCR data is stored along with confidence scores, allowing results with low confidence to be removed based on a specified threshold.

### Module 3 — Export

The processed document and extracted OCR information can be saved in PNG, TXT, JSON, and PDF formats. The system also keeps a log of important pipeline activities.

## Functional Requirements

1. The system must accept and validate supported image formats.
2. It must detect the document and correct its orientation using Computer Vision methods.
3. It must extract document text through EasyOCR.
4. It must provide an option to filter OCR results according to confidence scores.
5. It must support exporting results in multiple file formats.
6. It must provide clear handling of common input and processing errors.

## Non-Functional Requirements

* **Performance:** Process standard document images within a reasonable amount of time.
* **Reliability:** Properly handle invalid inputs and processing errors.
* **Usability:** Provide straightforward command-line options along with understandable messages.
* **Maintainability:** Organize preprocessing, OCR, exporting, and utility functions into separate modules.
* **Testing:** Use automated tests to verify important project functionality.
* **Logging:** Maintain records of significant events during the processing pipeline.

## Technology Stack

* Python
* OpenCV
* NumPy
* EasyOCR
* FPDF2
* pytest

## Testing

The project includes automated tests covering preprocessing and OCR-related functionality. The current test suite consists of **13 tests**, with the development test run producing:

```text
13 passed
```

A synthetic document image was additionally used to verify the preprocessing pipeline.

## Scope

This project demonstrates a basic Computer Vision workflow involving document detection, perspective transformation, image enhancement, OCR integration, and exporting of processed results.

## Future Scope

The system can be further improved by adding a graphical user interface, camera-based document capture, automatic orientation detection, more advanced document detection methods, support for additional OCR engines, and enhanced PDF creation.

## Conclusion

Document Scanner Using OCR demonstrates the integration of image processing and OCR techniques to transform a photograph of a document into a cleaner digital scan while also extracting its text. The modular design makes the system easier to test, maintain, and expand in the future.

## Declaration

I, ARYAN, Registration No. 24BAI10586, submit this project as an academic Computer Vision project titled **Document Scanner Using OCR**.

**Name:** ARYAN
**Registration No.:** 24BAI10586

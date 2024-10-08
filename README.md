## Project Directory Structure

```plaintext
PDF-OCR-Table-Extractor/
│
├── pdf_images/            # Folder to store images extracted from the PDF.
│   ├── page_1.png
│   ├── page_2.png
│   └── ...
│
├── pdf_texts/             # Folder to store text extracted from each PDF page.
│   ├── page_1_text.txt
│   ├── page_2_text.txt
│   └── ...
│
├── output/                # Folder for annotated images and extracted table content.
│   ├── annotations/       # Annotated images showing detected text regions.
│   │   ├── page_1_annotation.png
│   │   ├── page_2_annotation.png
│   │   └── ...
│   │
│   ├── json/              # JSON files containing table structure data.
│   │   ├── page_1.json
│   │   ├── page_2.json
│   │   └── ...
│   │
│   ├── page_1_result.jpg  # Annotated result images for detected structures.
│   ├── page_2_result.jpg
│   └── ...
│   
│   ├── page_1/            # Folder containing individual detected structures from the first page.
│   │   ├── [39, 215, 553, 332]_0.jpg
│   │   ├── [132, 44, 621, 222]_1.jpg
│   │   └── ...
│   │
│   ├── page_2/            # Folder containing individual detected structures from the second page.
│   │   ├── [51, 198, 537, 345]_0.jpg
│   │   └── ...
│
├── UnrealText.pdf         # The input PDF file used in the project.
└── README.md              # Project documentation (this file).

```
## Requirements
- Python 3.x
- PaddleOCR
- PyMuPDF
- OpenCV
- PIL

You can install the required libraries using:

```bash
pip install pymupdf opencv-python Pillow paddlepaddle paddleocr

# PDF OCR Converter to TXT LLM Ready Dataset Pipeline
This project converts scanned or image-based PDF documents into plain text files using Optical Character Recognition (OCR). It is designed to produce raw text suitable for training or fine-tuning Large Language Models. The pipeline extracts images from PDFs, applies Tesseract OCR to each page, and compiles the results into a structured format

# Key Features:
📄 Image-based PDF Support: Handles scanned PDFs using high-resolution conversion and OCR.

🧠 Tesseract OCR Integration: Extracts text with good accuracy using pytesseract.

🗂️ Page-wise Structure: Inserts page breaks (--- Page N ---) for easier dataset navigation.

💾 Clean TXT Output: Outputs a raw .txt file for each PDF, ready for tokenization or ingestion in RAG pipelines.

🛠️ Technologies Used:
pdf2image — Converts PDF pages into high-resolution images.

pytesseract + Tesseract-OCR — Performs OCR on each page image.

PIL, os — Image processing and file handling.

📂 Pipeline Overview:
Convert PDF to PNGs using pdf2image at 300 DPI.

OCR Each Page using Tesseract and compile the text.

Save as .txt file with structured page markers.

# Automated PDF to Structured CSV Data Extraction

## Description: <br>
A Python tool for extracting and structuring text data from PDF files using OCR and regex, then exporting it to CSV. This project is particularly suited for converting scanned PDFs containing structured forms or invoices into usable, tabulated data. By leveraging pdf2image and pytesseract, it handles each page of a PDF as an image, allowing reliable OCR text extraction. Regex patterns are used to extract specific data fields, enabling customizable and targeted text capture for complex data layouts.

## Features: <br>
<ul>
  <li>
    PDF-to-Image Conversion: Converts each PDF page to an image using pdf2image for high-fidelity OCR, making it suitable for scanned or image-heavy PDFs.
  </li>
  <li>
    OCR with Pytesseract: Extracts text from images using pytesseract, enabling multi-language support and high accuracy for complex documents.
  </li>
  <li>
    Regex-Based Data Extraction: Uses Python’s re module to apply regular expressions for capturing specific data fields from extracted text, such as dates, ticket numbers, customer information, weights, prices, and other structured details.
  </li>
  <li>
    Automated CSV Generation: Outputs structured data into a CSV file, with customizable headers, making it easy to analyze or integrate the data with other applications.
  </li>
</ul>

### Technical Details: <br>
**Dependencies:** <br>
<ul>
  <li>
    pdf2image: Converts each page of the PDF into high-resolution images for improved OCR accuracy.
  </li>
  <li>
    pytesseract: Provides OCR capabilities to recognize and extract text from images.
  </li>
  <li>
    re (Regex): Extracts targeted fields from the OCR output text.
  </li>
  <li>
    csv: Saves extracted data to CSV, ensuring structured and organized output.
  </li>
</ul>

**Data Extraction Example:** <br>
<ul>
  <li>
    Extracted fields include Ticket, Date, Time, Customer, Transporter, Gross Weight, and others using regex to capture patterns for each field.
  </li>
  <li>
    Supports missing data by returning "N/A" for fields not found, ensuring consistent CSV formatting.
  </li>
</ul>

**Setup and Usage:** <br>
<ol>
  <li>
    Install dependencies: pip install pdf2image pytesseract.
  </li>
  <li>
    Install poppler-utils for compatibility with pdf2image.
  </li>
  <li>
    Run the script by specifying your PDF file, and view results in the generated CSV.
  </li>
  <li>
    This tool is ideal for analysts, developers, or organizations needing a reliable way to extract and organize structured data from PDF documents, such as invoices, logs, or records.
  </li>
</ol>

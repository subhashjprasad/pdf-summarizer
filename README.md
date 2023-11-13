# pdf-summarizer
A program that summarizes (page-by-page) a PDF with multiple pages. 
Runtime depends on length of PDF.

Created using PyTorch, facebook/nougat-base for OCR, and pszemraj/led-large-book-summary for text summarization.

## Usage
For detailed implementation/modification, refer to PDFSummarizer.ipynb.

### Ready-To-Use Instructions (with PDFSummarizerEasyUse.ipynb):
- Run first cell
- Upload pdf to Files
- Replace `pdf_path` variable with appropriate pdf file path:
```
%%capture
pdf_path = 'coontz.pdf' # replace with pdf path
images = convert_from_bytes(open(pdf_path, 'rb').read(), size=800)
```
- Run second cell
- Run third cell to print summarized output

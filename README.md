# How to automatically search certain keywords in historical source editions and how to highlight them for Historical Matrix Online or any other projects



## What you will need:

- A digitized version of the historical source edition / collection in PDF format

- Download [matrix_thesaurus.sh](matrix_thesaurus.sh)

  In case you want to search for other keywords, you can exchange the keywords in the shell script according to your needs.

- [ocrmypdf](https://ocrmypdf.readthedocs.io/en/latest/index.html), [tesseract and language data packs](https://github.com/tesseract-ocr)

- [PyMuPDF](https://pypi.org/project/PyMuPDF/) and pdf_highlighter.py ([github](https://github.com/x4nth055/pythoncode-tutorials/tree/master/handling-pdf-files/highlight-redact-text) or [website](https://www.thepythoncode.com/code/redact-and-highlight-text-in-pdf-with-python))

Everything listed above is open source and freely accessible. Everything was tested using Arch- and Debian-based Linux machines.



## Workflow

### Step 1:

Install and setup ocrmypdf, tesseract, language data packs, PyMuPDF and pdf_highlighter.py on your PC.

### Step 2:

OCR the digitized source edition according to your needs. 

### Step 3:

For highlighting the words with pdf_highlighter.py, go to your folder where the PDFs are stored, open the terminal and type in:

1.) Make matrix_thesaurus.sh executable:

`chmod +x matrix_thesaurus.sh`

2.) Run matrix_thesaurus.sh for all PDFs in the folder (Note: this will add the highlights to the existing files):

`bash matrix_thesaurus.sh`

### Step 4:

By using any PDF reader, look for the pages with highlights.

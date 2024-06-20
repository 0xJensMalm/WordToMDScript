# Epikrise script

This script extracts sections from a Word document and generates separate Markdown files based on specific markers. The content should be formatted using these markers within the Word document.

## Markers

- **T:** Title of a new document.
- **S:** Section title.
- **C:** New paragraph within the section.
- **P:** List item.

### Example Formatting

Here is how to format your Word document using the markers:

T: Document Title
S: Section Title 1
C: This is the first paragraph of section 1.
P: This is a point under section 1.
S: Section Title 2
C: This is the first paragraph of section 2.
C: This is the second paragraph of section 2.



## How to Use the Script

1. **Prepare Your Word Document**
    - Ensure your document is formatted using the markers `T:`, `S:`, `C:`, and `P:` as described above.
    - Save the document as `epikriser.docx` in the same directory as the script.

2. **Set Up the Environment**
    - Install the `python-docx` library if you haven't already:
      ```bash
      pip install python-docx
      ```

3. **Run the Script**
    - Place the script and the `epikriser.docx` file in the same directory.
    - Execute the script:
      ```bash
      python epikrisescript.py
      ```

4. **Output**
    - The script will generate Markdown files in the `output_md_files` directory within the same folder as the script.
    - Each Markdown file will be named based on the title specified by the `T:` marker.

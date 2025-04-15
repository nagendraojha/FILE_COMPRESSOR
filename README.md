# FILE_COMPRESSOR


1. **Import Libraries**:
   - **os**: Handles file system operations.
   - **gzip**: Compresses files using the GZIP format.
   - **tkinter**: Provides a graphical user interface (GUI) for file upload.
   - **PIL (Python Imaging Library)**: Handles image compression.
   - **shutil**: A file handling library (not used directly in the script).

2. **Function `compress_file()`**:
   - Compresses files based on their type.
   - **Images** (PNG, JPG, etc.) are compressed by reducing quality to 50% using the `PIL` library.
   - **Text files** (TXT, CSV, etc.) are compressed using the GZIP format.
   - **Other binary files** (PDFs, EXE, etc.) are also compressed using GZIP.

3. **Function `upload_and_compress()`**:
   - Opens a file dialog for the user to select a file.
   - If a file is selected, it generates an output path in the **Downloads** folder and compresses the file using the `compress_file()` function.

4. **GUI Setup**:
   - A Tkinter window is created with a label and a button.
   - The button lets the user upload a file and automatically compress it.

5. **Execution**:
   - The program waits for the user to upload a file and then compresses it based on the file type.
   - The compressed file is saved in the **Downloads** folder.

---

This script allows users to upload a file, and it will automatically compress the file (image, text, or binary) and save it in the Downloads folder.

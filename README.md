# Ales Light Sensor

This project was built to help a **CISCO electrical engineering employee** streamline their workflow by extracting product-specific information from a large Word document and automatically generating a new, clean document with only the relevant product data.

I developed this tool **entirely on my own** by watching YouTube tutorials, exploring Python libraries, and applying what I learned to solve a real-world need. This is a self-taught project that demonstrates both initiative and practical problem-solving.

---

## What It Does

Given a master `.docx` file with information about multiple products, the script:

- Prompts the user to input a product number
- Parses the Word document to isolate only the relevant product content
- Generates a new Word document with just that product’s information
- Saves the output in a clean format inside the `output/` folder

This solution is especially helpful for engineers or teams who frequently need to extract and send product-specific documentation.

---

## How to Run This in VS Code

Follow these steps to set up and run the script locally.

### 1. Clone the Repository

Open your terminal or VS Code, then run:

```bash
git clone https://github.com/jangel19/aleslightsensor.git
cd aleslightsensor
```

Alternatively, in VS Code:
- Press `Cmd+Shift+P` (Mac) / `Ctrl+Shift+P` (Windows)
- Type **"Git: Clone"**
- Paste the repo URL above
- Choose a folder and open it in a new window

---

### 2. (Optional) Create a Virtual Environment

Creating a virtual environment is best practice to isolate dependencies.

**Mac/Linux:**
```bash
python3 -m venv .venv
source .venv/bin/activate
```

**Windows:**
```bash
python -m venv .venv
.venv\Scripts\activate
```

---

### 3. Install Required Packages

Make sure you're in the project directory, then run:

```bash
pip install -r requirements.txt
```

This installs all the Python libraries the script depends on (like `python-docx`).

---

### 4. Run the Script

Use this command to run the main program:

```bash
python product_doc_filter/clean_master.py
```

You’ll be asked to input a product number (e.g. `2`).  
The script will then generate a new document with only that product’s information and save it to:

```
product_doc_filter/output/product_2_cleaned.docx
```

---

## Project Structure

```
aleslightsensor/
│
├── product_doc_filter/
│   ├── master.docx                # The original document containing all products
│   ├── clean_master.py            # Python script to extract product-specific content
│   └── output/                    # Folder where new cleaned docs are saved
│       └── product_X_cleaned.docx
│
├── requirements.txt               # Python dependencies
├── README.md                      # You're reading it!
```

---


## 👤 Author

**Jordi Lopez**  
[GitHub – @jangel19](https://github.com/jangel19)  
Self-taught developer, CS + Math student, and builder of helpful tools.  
I created this project after a Cisco engineer described a tedious documentation problem. I saw a way to automate it — and learned everything needed by diving into Python, the `python-docx` library, and YouTube resources.

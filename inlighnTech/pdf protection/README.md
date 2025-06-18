# 🔐 PDF Password Protector

This script allows you to add password protection to an existing PDF file using Python's `PyPDF2` library.

## ✅ Features

- Add password to any PDF file
- Lightweight and easy to use from the command line
- Handles common errors (missing file, invalid PDF, etc.)

---

## 🛠 Requirements

Install the required Python package:

```bash
pip install PyPDF2
```

---

## 📄 Usage

```bash
python3 script.py <input_pdf> <output_pdf> <password>
```

### 📌 Arguments

| Argument       | Description                             |
|----------------|-----------------------------------------|
| `input_pdf`    | Path to the original PDF file           |
| `output_pdf`   | Name/path for the new protected PDF     |
| `password`     | Password to apply to the new PDF file   |

---

## 💡 Example

```bash
python3 script.py document.pdf protected_document.pdf secret123
```

If successful, you’ll see:

```
Password-protected PDF saved as protected_document.pdf
```


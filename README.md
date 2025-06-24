# Assyrian Keyboard & PDF Workbench

## Project Overview

The **Assyrian Keyboard & PDF Workbench** is a web-based application designed to facilitate interaction with the Eastern (**Maḏnḥāyā**) Syriac script. It combines:

- A virtual Assyrian keyboard for easy text input.
- A PDF viewer for displaying historical texts (like the American Bible Society Peshitta).
- OCR (Optical Character Recognition) to extract and transliterate text directly from PDF documents.

This tool is ideal for scholars, students, and anyone engaging with Syriac texts—especially those in the Eastern dialect.

## 🌐 Live Demo

Try it here: [https://ai-assyria.github.io/assyrian-bible-workbench/](https://ai-assyria.github.io/assyrian-bible-workbench/)

---

## Features

### 🔤 Virtual Assyrian Keyboard

- Supports **Eastern (Maḏnḥāyā)** and **Estrangelā** scripts.
- **Two Layouts:**
  - **Assyrian Letters** – Buttons display Syriac characters.
  - **QWERTY (Latin Mapped)** – Buttons display Latin keys mapped to Syriac.
- Accurate diacritic support (e.g., `ܶ` rḇāṣā ʾărīḵā, `ܹ` rḇāṣā karyā).
- Real-time **transliteration** to Latin script.
- Save typed text as a **PNG image**.

### 📄 PDF Viewer

- Renders PDF documents in-browser.
- Pre-loaded with the **1886 ABS Peshitta**.
- Upload your own PDFs.
- Simple navigation controls.

### 🔍 Optical Character Recognition (OCR)

- Uses **Tesseract.js** to extract Syriac text.
- Falls back to **image-based OCR** if no text layer is found.
- Displays both **original Syriac** and **transliteration**.
- Uses the **`syr` trained data model** for optimal Syriac recognition.

---

## 🛠️ Technologies Used

- **HTML5** – Structure.
- **Tailwind CSS** – Styling.
- **JavaScript** – Core logic.
- **PDF.js** – PDF rendering.
- **Tesseract.js** – OCR engine.
- **Google Fonts** – `Noto Sans Syriac Eastern` & `Estrangela`.

---

## 🚀 How to Use

1. **Open the App**: Visit the [live demo](https://ai-assyria.github.io/assyrian-bible-workbench/).
2. **Browse PDFs**: Use the nav buttons to flip through the default Peshitta.
3. **Upload Your Own**: Click _"Upload another Assyrian PDF"_.
4. **OCR Output**: Extracted Syriac text + transliteration appear below the viewer.
5. **Use the Keyboard**:
   - Select script: _Estrangelā_ or _Maḏnḥāyā_.
   - Choose layout: _Assyrian Letters_ or _QWERTY (Latin Mapped)_.
   - Type using the buttons or keyboard.
   - View transliteration in real time.
6. **Save as PNG**: Click _"Save Text as Image"_ after typing.

---

## 🧑‍💻 Local Installation (Development)

### 1. Clone the Repository

```bash
git clone https://github.com/AI-Assyria/assyrian-bible-workbench.git
cd assyrian-bible-workbench
````

### 2. Download Tesseract Language Data

Make sure your browser can fetch:

```
https://cdn.jsdelivr.net/npm/@tesseract.js-data/syr@1.0.0/4.0.0_best_int/syr.traineddata.gz
```

*Note: JSDelivr CDN is used for best browser compatibility.*

### 3. Serve Locally

#### Option A – Python (recommended)

```bash
python -m http.server 8000
```

Then open: [http://localhost:8000/assyrian-keyboard-app.html](http://localhost:8000/assyrian-keyboard-app.html)

#### Option B – Node.js

```bash
npm install -g http-server
http-server . -p 8000
```

Then open: [http://localhost:8000/assyrian-keyboard-app.html](http://localhost:8000/assyrian-keyboard-app.html)

---

## 📝 Important Notes on Syriac Script

* **Eastern Vowel Accuracy**: Diacritic rendering is tailored to the **Eastern Syriac (Maḏnḥāyā)** tradition.
* **OCR Limitations**: The `syr` model is mainly trained on **Estrangelā**. OCR accuracy may vary with Eastern fonts. A future goal is training a custom Tesseract model on Peshitta glyphs.

---

## 🤝 Contributing

Contributions welcome!

1. Fork the repo.
2. Create a new branch: `git checkout -b feature/your-feature`
3. Make your changes.
4. Commit: `git commit -m "Add feature"`
5. Push: `git push origin feature/your-feature`
6. Submit a **Pull Request**.

---

## 📄 License

Licensed under **GNU GPL v3.0**. See the `LICENSE` file for details.

---

## 🙏 Acknowledgements

* [PDF.js](https://mozilla.github.io/pdf.js/)
* [Tesseract.js](https://github.com/naptha/tesseract.js)
* [Tailwind CSS](https://tailwindcss.com/)
* [Google Fonts – Noto Syriac](https://fonts.google.com/)

```

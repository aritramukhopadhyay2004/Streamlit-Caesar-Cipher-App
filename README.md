# Streamlit-Caesar-Cipher-App

A simple, interactive Streamlit web app that demonstrates the classic Caesar cipher. Use this app to encrypt and decrypt text by shifting letters by a fixed number of positions in the alphabet. It's intended as an educational tool to show how substitution ciphers work and to provide a lightweight demo of a Streamlit application.

---

## Features

- Encrypt plain text using the Caesar cipher.
- Decrypt cipher text back to plain text (using the same shift value).
- Adjustable shift (rotation) value.
- Preserves letter case and leaves non-alphabetic characters (punctuation, digits, spaces) unchanged.
- Easy to run locally with Streamlit or deploy to Streamlit Cloud.

---

## How the Caesar Cipher Works (short)

The Caesar cipher is a substitution cipher where each letter in the plaintext is shifted a fixed number of places down (or up) the alphabet. For example, with a shift of 3:
- `A -> D`, `B -> E`, `C -> F`, ...
- `Z -> C` (wraps around)

When decrypting, you shift in the opposite direction by the same amount.

Example:
- Plain: `Hello, World!`
- Shift: `3`
- Cipher: `Khoor, Zruog!`

---

## Prerequisites

- Python 3.8+ recommended
- Git (to clone the repo)
- Internet access for installing dependencies

The repository includes a `requirements.txt` file listing required packages (Streamlit is required).

---

## Installation & Running Locally

1. Clone the repository:
   git clone https://github.com/aritramukhopadhyay2004/Streamlit-Caesar-Cipher-App.git
   cd Streamlit-Caesar-Cipher-App

2. (Optional) Create and activate a virtual environment:
   python -m venv .venv
   - On macOS/Linux: source .venv/bin/activate
   - On Windows (PowerShell): .venv\Scripts\Activate.ps1

3. Install dependencies:
   pip install -r requirements.txt

4. Run the Streamlit app:
   streamlit run app.py

5. The app will open in your browser (usually at http://localhost:8501).

---

## Usage (UI Overview)

- Enter the text you want to encrypt or decrypt in the provided input area.
- Choose the operation: Encrypt or Decrypt.
- Set the shift (an integer). Positive values rotate forward; negative values rotate backward.
- The app displays the resulting transformed text and typically provides a copy/download option (if implemented).
- Non-letter characters are left unchanged, and uppercase/lowercase are preserved.

---

## Example

Encrypting the text:
- Input: `Hello, World!`
- Shift: `3`
- Output: `Khoor, Zruog!`

Decrypting:
- Input: `Khoor, Zruog!`
- Shift: `3`
- Output: `Hello, World!`

---

## Code Structure

- `app.py` — Main Streamlit application. Contains the UI and the Caesar cipher logic (encryption/decryption, shift handling, input/output).
- `requirements.txt` — Python dependencies for the app.
- `LICENSE` — License file for the project.
- `.gitignore` — Files and directories excluded from the repository.

(If you want, I can open and review `app.py` and produce a precise function-level summary or docstrings for each function.)

---

## Deployment

To deploy on Streamlit Cloud:
1. Create a new app on [Streamlit Cloud](https://streamlit.io/cloud).
2. Connect the GitHub repo `aritramukhopadhyay2004/Streamlit-Caesar-Cipher-App`.
3. Set the main file to `app.py`.
4. Deploy — Streamlit Cloud will install dependencies from `requirements.txt` and run the app.

Alternatively, you can deploy the app on other platforms that support Python web apps (Heroku, Docker, etc.).

---

## Contributing

Contributions are welcome. To contribute:
1. Fork the repository.
2. Create a feature branch: `git checkout -b feature/my-change`
3. Make changes and commit them.
4. Push to your fork and open a Pull Request against the main repository.

Suggestions:
- Add unit tests for the cipher functions.
- Improve UI/UX (copy-to-clipboard, download output, preset shifts).
- Add support for other alphabets or character encodings.

---

## License

See the `LICENSE` file in this repository for license details.

---

## Contact

For questions or suggestions, open an issue or contact the repository owner via GitHub:
https://github.com/aritramukhopadhyay2004

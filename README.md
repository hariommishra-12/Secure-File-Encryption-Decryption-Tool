# Secure-File-Encryption-Decryption-Tool
A Python GUI application to securely encrypt and decrypt files using Fernet symmetric encryption, with support for key generation, clipboard copy, and activity logging.
# Features
- Generate a secure encryption key with a single click <br>
- Encrypt files and save the output to any location<br>
- Decrypt files using the correct key<br>
- Automatically copy the generated key to the clipboard<br>
- View or delete activity logs<br>
- Clean and simple GUI built with tkinter<br>
# Requirements
- Python 3.7 or higher<br>
- Required Python packages: pip install cryptography, pip install pyperclip, pip install tk<br>
- Note: tkinter is usually included with Python by default<br>
# How to Use
- Run the application: python MAIN.py<br>
- Generate a Key: Click Generate Key to create a secure Fernet key. The key is automatically copied to your clipboard<br>
- Select Input and Output Files: Click Select Input File to choose the file to encrypt or decrypt. Click Select Output File to choose where to save the result<br>
- Encrypt a File: Enter the key in the Key field (or use the generated key) and click Encrypt<br>
- Decrypt a File: Enter the key used for encryption and click Decrypt<br>
- Manage Logs: Click Show Logs to view the activity log, click Delete Logs to clear the log file<br>
# Usage Example
Suppose you have a file named example.txt that you want to encrypt:

- Launch the application: python your_script_name.py<br>
- Generate a key by clicking Generate Key. Copy it from the key field<br>
- Select example.txt as the input file<br>
- Choose a location and filename for the output, e.g., example_encrypted.txt<br>
- Click Encrypt. The file is now encrypted<br>

**To decrypt:**

- Open the app again<br>
- Select example_encrypted.txt as the input file<br>
- Choose an output filename like example_decrypted.txt<br>
- Enter the key used during encryption<br>
- Click Decrypt. The original file will be restored<br>
# Security Notes
- Keep your key safe: Without it, encrypted files cannot be restored<br>
- Logs contain file paths and keys; handle them securely<br>
- Uses Fernet symmetric encryption — strong and reliable for file security<br>
# File Structure

SecureFileEncryption/<br>
├── MAIN.py # Main Python script<br>
├── logs.log # Activity logs (auto-created)<br>
└── README.md # Documentation<br>


# License

This project is licensed under the MIT License.

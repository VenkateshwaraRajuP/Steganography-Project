A secure web application for hiding secret messages within images using advanced steganography techniques combined with AES encryption. Built with Streamlit for an intuitive user interface.

✨ Features
🔒 AES Encryption: Messages are encrypted before being hidden in images
🖼️ Image Steganography: Hide encrypted messages in PNG images
🔑 Dual Key System: Separate encryption and stego keys for enhanced security
📱 User-Friendly Interface: Clean, responsive web interface built with Streamlit
📥 Download Support: Easy download of encoded images
🔍 Message Extraction: Retrieve hidden messages with correct keys
🚀 Quick Start
Local Development
Clone the repository

git clone https://github.com/YOUR_USERNAME/steganography-project.git
cd steganography-project
Install dependencies

pip install -r requirements.txt
Run the application

streamlit run app.py
Open your browser Navigate to http://localhost:8501

📖 Usage
Encoding a Message
Upload Image: Select a PNG, JPG, or JPEG image
Enter Message: Type the secret message you want to hide
Set Keys:
AES Encryption Key: For encrypting the message
Stego Key: For hiding the encrypted message
Encode: Click to process and download the encoded image
Decoding a Message
Upload Encoded Image: Select the PNG file containing the hidden message
Enter Keys: Provide the same stego key and AES decryption key
Decode: Extract and view the hidden message
🔧 Technical Details
Steganography Method: LSB (Least Significant Bit) substitution
Encryption: AES-256 in CBC mode with random IV
Image Format: PNG (lossless compression preserves hidden data)
Key Derivation: SHA-256 hashing for encryption keys
🌐 Deployment
Streamlit Cloud (Recommended)
Push your code to GitHub
Visit share.streamlit.io
Connect your GitHub repository
Deploy automatically
Other Platforms
The project includes a Procfile for Heroku and other platforms that support it.

📋 Requirements
Python 3.7+
Streamlit 1.32.0
OpenCV 4.9.0.80
NumPy 1.26.4
Pillow 10.0.1
PyCryptodome 3.19.0
⚠️ Important Notes
PNG Format Only: Decoding only works with PNG files as JPG/JPEG compression destroys hidden data
Key Security: Keep your encryption and stego keys safe - they're required for decoding
Image Size: Larger images can hide longer messages
Data Integrity: Don't edit or compress encoded images
🔒 Security Features
AES-256 Encryption: Military-grade encryption for message security
Random IV: Each encryption uses a unique initialization vector
Key Separation: Different keys for encryption and steganography
Hash-based Keys: SHA-256 derivation for consistent key handling
🤝 Contributing
Fork the repository
Create a feature branch (git checkout -b feature/amazing-feature)
Commit your changes (git commit -m 'Add amazing feature')
Push to the branch (git push origin feature/amazing-feature)
Open a Pull Request
📄 License
This project is licensed under the MIT License - see the LICENSE file for details.

🙏 Acknowledgments
Built with Streamlit
Encryption powered by PyCryptodome
Image processing with OpenCV and Pillow

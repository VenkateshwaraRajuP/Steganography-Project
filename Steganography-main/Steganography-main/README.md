# 🔐 Image Steganography with AES Encryption

A secure web application for hiding secret messages within images using advanced steganography techniques combined with AES encryption. Built with Streamlit for an intuitive user interface.

## ✨ Features

- **🔒 AES Encryption**: Messages are encrypted before being hidden in images
- **🖼️ Image Steganography**: Hide encrypted messages in PNG images
- **🔑 Dual Key System**: Separate encryption and stego keys for enhanced security
- **📱 User-Friendly Interface**: Clean, responsive web interface built with Streamlit
- **📥 Download Support**: Easy download of encoded images
- **🔍 Message Extraction**: Retrieve hidden messages with correct keys

## 🚀 Quick Start

### Local Development

1. **Clone the repository**
   ```bash
   git clone https://github.com/YOUR_USERNAME/steganography-project.git
   cd steganography-project
   ```

2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the application**
   ```bash
   streamlit run app.py
   ```

4. **Open your browser**
   Navigate to `http://localhost:8501`

## 📖 Usage

### Encoding a Message

1. **Upload Image**: Select a PNG, JPG, or JPEG image
2. **Enter Message**: Type the secret message you want to hide
3. **Set Keys**: 
   - **AES Encryption Key**: For encrypting the message
   - **Stego Key**: For hiding the encrypted message
4. **Encode**: Click to process and download the encoded image

### Decoding a Message

1. **Upload Encoded Image**: Select the PNG file containing the hidden message
2. **Enter Keys**: Provide the same stego key and AES decryption key
3. **Decode**: Extract and view the hidden message

## 🔧 Technical Details

- **Steganography Method**: LSB (Least Significant Bit) substitution
- **Encryption**: AES-256 in CBC mode with random IV
- **Image Format**: PNG (lossless compression preserves hidden data)
- **Key Derivation**: SHA-256 hashing for encryption keys

## 🌐 Deployment

### Streamlit Cloud (Recommended)

1. Push your code to GitHub
2. Visit [share.streamlit.io](https://share.streamlit.io)
3. Connect your GitHub repository
4. Deploy automatically

### Other Platforms

The project includes a `Procfile` for Heroku and other platforms that support it.

## 📋 Requirements

- Python 3.7+
- Streamlit 1.32.0
- OpenCV 4.9.0.80
- NumPy 1.26.4
- Pillow 10.0.1
- PyCryptodome 3.19.0

## ⚠️ Important Notes

- **PNG Format Only**: Decoding only works with PNG files as JPG/JPEG compression destroys hidden data
- **Key Security**: Keep your encryption and stego keys safe - they're required for decoding
- **Image Size**: Larger images can hide longer messages
- **Data Integrity**: Don't edit or compress encoded images

## 🔒 Security Features

- **AES-256 Encryption**: Military-grade encryption for message security
- **Random IV**: Each encryption uses a unique initialization vector
- **Key Separation**: Different keys for encryption and steganography
- **Hash-based Keys**: SHA-256 derivation for consistent key handling

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Built with [Streamlit](https://streamlit.io/)
- Encryption powered by [PyCryptodome](https://pycryptodome.readthedocs.io/)
- Image processing with [OpenCV](https://opencv.org/) and [Pillow](https://python-pillow.org/)

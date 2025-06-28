# CampusKey

CampusKey is a robust digital identity verification system that securely embeds user-specific QR codes into ID card images using advanced LSB steganography and 5D Quantum Logistic Map encryption. Designed primarily for educational institutions, it ensures tamper-resistant and invisible ID encoding, with real-time database verification support.

## 🧠 Overview
This project aims to enhance the security of digital ID cards using a multi-layered approach:
Invisible QR code embedding via LSB Steganography in the Y channel of YCbCr color space
Chaotic encryption using a 5D Quantum Logistic Map
Real-time verification of extracted QR codes against a database

## 🔧 Technologies Used
Technology	Purpose
Python	Core programming language
OpenCV	Image manipulation & QR scanning
Pillow	Image I/O operations
NumPy, SciPy	Data processing and transformations
QR Code Libraries	QR code generation & decoding
Flask/Django (optional)	For web-based verification interface
SQL/NoSQL DB	User and ID record storage
Git	Version control

## 🚀 Features
🔒 Encrypted QR Embedding using chaotic maps (5D QLM)
🖼️ Imperceptible Steganography in the Y channel of YCbCr
🗃️ Database Verification of extracted IDs
📉 Compression via RLE before encryption
⚙️ Robust Extraction despite compression/noise
📲 Future Mobile App & Blockchain Support

## 🛠️ Installation & Setup

```bash
# Clone the repository
git clone https://github.com/Samyakjain2004/CampusKey.git
cd CampusKey

# Install dependencies
pip install -r requirements.txt

```

Dependencies include:
- opencv-python
- pyzbar
- pillow
- numpy
- flask or django (optional for web support)

## 📌 How It Works

### 🔐 Embedding Flow:
- Generate unique QR Code from user ID.
- Convert QR to binary → compress using Run Length Encoding.
- Encrypt with 5D Quantum Logistic Map.
- Convert target image to YCbCr → Embed into LSBs of Y channel.
- Reconstruct and save the final stego image.

### 🔓 Extraction Flow:
- Convert stego image to YCbCr.
- Extract LSBs from Y → Decrypt using QLM → Decompress.
- Reconstruct QR Code → Scan → Verify against database.

## 🌱 Future Scope
- 🔍 AI-based tamper detection
- 🔗 Blockchain-based ID verification
- 📱 Cross-platform mobile app
- 🧠 Biometric fusion (face/fingerprint)
- 🚪 IoT integration for access control

## 📜 License

This project is licensed under the MIT License.

## 👨‍💻 Author

Samyak Jain
🔗 LinkedIn - https://www.linkedin.com/in/samyak-jain-470b7b255

🔗 GitHub - https://github.com/Samyakjain2004

## 🤝 Contributing
Pull requests and suggestions are welcome! For major changes, please open an issue first to discuss.



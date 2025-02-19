Secure Data Hiding in Image Using Steganography

📌 Project Description

This project implements image steganography to securely hide a secret message inside an image. The message is embedded by modifying pixel values, and access to decryption is protected by a passcode. The approach ensures minimal image distortion while keeping the hidden data discreet and secure.

🚀 Features

Passcode-Protected Decryption – Ensures only authorized users can retrieve the hidden message.

Minimal Image Distortion – Direct pixel value modifications reduce visible changes to the image.

Lightweight & Simple Implementation – Uses only OpenCV and standard Python libraries.

Fully Reversible Encoding – No external metadata is required for decryption.

🛠️ Technologies Used

Python 3.x

OpenCV (cv2) – Image processing for reading, modifying, and saving images.

OS Module – To open the modified image automatically after encryption.

📂 Project Structure

📁 SecureSteganography
│── 📄 steganography.py   # Main script for encoding and decoding messages
│── 🖼️ twitter.png       # Sample image for testing (replace with your own)
│── 📄 README.md         # Project documentation

🔧 Installation & Setup

Install Python (if not installed) from Python Official Site

Install OpenCV using pip:

pip install opencv-python

Run the script:

python steganography.py

Enter a secret message and a passcode to encrypt the message inside an image.

Provide the correct passcode to decrypt the message successfully.

🎯 How It Works

Encryption Process:

Reads an image using OpenCV.

Converts the message characters into ASCII values.

Modifies pixel values to store the message.

Saves the new image as encryptedImage.jpg.

Decryption Process:

Reads the modified image.

Uses the passcode to extract the original message from pixel values.

Displays the decrypted message.

🔐 Security Considerations

The passcode prevents unauthorized decryption.

The approach avoids noticeable image distortions.

Can be improved by adding encryption before embedding the message.

🎯 Future Enhancements

Implement AES encryption before embedding the message for added security.

Support larger message sizes using optimized encoding techniques.

Develop a GUI-based version for user-friendly interaction.

📜 License

This project is open-source under the MIT License.

💡 Contributions are welcome! Feel free to improve the security features or add new functionalities.


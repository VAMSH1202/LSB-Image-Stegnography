# Image Steganography System 🔐

## 📌 Project Overview

This project implements Least Significant Bit (LSB) based Image Steganography, which is the technique of hiding secret data within an image file by modifying the least significant bits of pixel values. The process ensures that the image remains visually unchanged while carrying embedded information.

Both sender and receiver share a secret key to encode/decode the hidden data, enhancing security. This project also serves as a hands-on introduction to basic image processing techniques and low-level bit manipulation in C.

## 🔧 Features

- Hide text data inside image files (e.g., `.bmp`)
- Extract hidden data using a shared secret key
- Preserve image integrity with minimal visual distortion
- Hands-on practice with bitwise operations and file manipulation in C
- Understand how data is represented and manipulated at the byte/bit level

## 🧠 Pre-requisites

Before diving in, ensure you're comfortable with:

- Function pointers
- File I/O operations
- Bitwise operations

## 🚀 How It Works

### Encoding
1. Take a source image and the secret message to hide
2. Modify the LSBs of pixel data based on the message bits
3. Save the modified image as a stego-image

### Decoding
1. Read the stego-image using the shared secret key
2. Extract and reconstruct the original hidden message from LSBs

## 🛠️ Tech Stack

- **Language:** C
- **Image Format:** .bmp (Bitmap)
- **Tools:** GCC compiler, Makefile

## 📁 Project Structure

- `encode.c` — Logic for embedding secret message into image
- `decode.c` — Logic for extracting hidden message from image
- `common.h` — Shared structures and function prototypes
- `Makefile` — Build instructions

## ⚙️ How to Compile & Run
```bash
# Compile
make

# Encode (hide message)
./stego encode input.bmp secret.txt output.bmp

# Decode (extract message)
./stego decode output.bmp extracted.txt
```

## What I Learned

- Bitwise operations and bit-level data manipulation in C
- BMP file format structure and pixel data handling
- File I/O using file pointers in C
- Modular programming with Makefiles
- Basics of image steganography and data security

## Author

**Miryala Vamshi**  
Embedded Systems Engineer  
📧 vamshimiryala2@gmail.com  
🔗 [LinkedIn](https://linkedin.com/in/vamshi-miryala-a7b71a347)

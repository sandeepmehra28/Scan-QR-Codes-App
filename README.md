# Barcode & QR Code Scanner App

This Android application scans **barcodes** and **QR codes** using **CameraX** and **Google ML Kit Barcode Scanning API**. It detects and displays the barcode's content, and automatically opens URLs when scanned.

## ✨ Features

- Real-time barcode and QR code scanning
- Supports multiple formats: `QR_CODE`, `EAN_13`, `CODE_128`
- Automatically opens URLs in browser
- Uses `CameraX` for camera integration
- Minimal and user-friendly interface

## 📸 Screenshots

*(Add your screenshots here if available)*

## 🔧 Tech Stack

- **Kotlin**
- **CameraX**
- **ML Kit Barcode Scanning**
- **AndroidX Libraries**

## 📂 Project Structure

- `MainActivity.kt`: Core logic for camera and barcode processing
- `activity_main.xml`: UI layout with `PreviewView` and `TextView` for scan results

## 📱 UI Layout

```xml
<LinearLayout>
 ├── TextView (Header)
 ├── PreviewView (CameraX Preview)
 └── TextView (Scan result)
</LinearLayout>

✅ Barcode Formats Supported

QR_CODE

EAN_13

CODE_128

⚙️ How It Works

Requests camera permission at runtime

Initializes the back camera using CameraX

Analyzes camera frames to detect barcodes

Displays the scanned value in a TextView

Automatically opens links if the scanned value is a URL

🔒 Permissions

CAMERA – Required for real-time scanning

🛠️ How to Run

Clone this repository or copy the source code

Open the project in Android Studio

Connect a physical device (CameraX doesn't work well on some emulators)

Run the app and grant the camera permission

Scan a barcode or QR code

📦 Dependencies
Add these to your build.gradle:
// CameraX
implementation "androidx.camera:camera-core:1.3.0"
implementation "androidx.camera:camera-camera2:1.3.0"
implementation "androidx.camera:camera-lifecycle:1.3.0"
implementation "androidx.camera:camera-view:1.3.0"

// ML Kit Barcode Scanner
implementation 'com.google.mlkit:barcode-scanning:17.2.0'
( Make sure to use the latest versions as needed. )

🚀 Future Improvements

Support scanning multiple barcodes at once

Add flashlight toggle

Improve UI/UX with animations and transitions

Save scanned history locally




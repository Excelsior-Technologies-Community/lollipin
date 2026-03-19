# 🍭 Flutter LolliPin

A lightweight Flutter package for implementing **PIN-based and Biometric (Fingerprint / Face ID)** authentication — just like a device lock screen 🔐

---

## ✨ Features

- 🔢 Secure PIN (Passcode) unlock
- 👆 Fingerprint
- 🔐 Local PIN storage using SharedPreferences
- ⚡ Smooth and minimal UI
- 🔁 Auto biometric prompt
- ❌ Error handling (no biometrics / wrong PIN)

---

### preview

https://github.com/user-attachments/assets/559cc760-9122-40d6-bd84-53a61a3697dc

## 📦 Installation

### 🔗 From GitHub

```yaml
dependencies:
  flutter_lollipin:
    git:
      url: https://github.com/jaypanchal1014/flutter_lollipin.git
```

---

### 📥 Get Packages

```bash
flutter pub get
```

---

## 🚀 Getting Started

### 1. Import

```dart
import 'package:flutter_lollipin/flutter_lollipin.dart';
```

---

### 2. Use in App

```dart
MaterialApp(
  home: LockScreen(),
);
```

---

## 📱 How It Works

- App opens → Lock screen appears
- User can:
  - Enter PIN 🔢
  - Use Fingerprint 👆

- On success → Navigate to next screen

---

## ⚙️ Android Setup

### ✅ MainActivity

```kotlin
import io.flutter.embedding.android.FlutterFragmentActivity

class MainActivity: FlutterFragmentActivity() {
}
```

---

### ✅ Permissions

```xml
<uses-permission android:name="android.permission.USE_BIOMETRIC"/>
<uses-permission android:name="android.permission.USE_FINGERPRINT"/>
```

---

## ⚠️ Requirements

- Device must have:
  - Fingerprint
  - Screen lock enabled

---

## 🧪 Error Handling

Handled cases:

- ❌ No biometrics enrolled
- ❌ Wrong PIN
- ❌ Biometric not available

---

## 📄 License

MIT License

Copyright (c) 2026 Excelsior Technologies

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

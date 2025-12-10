# KampusApp2

Project aplikasi kampus berbasis React Native.

## Prasyarat

Pastikan Anda telah menginstal:
- [Node.js](https://nodejs.org/)
- [Java Development Kit (JDK)](https://www.oracle.com/java/technologies/downloads/)
- [Android Studio](https://developer.android.com/studio) (untuk Android)
- [Xcode](https://developer.apple.com/xcode/) (untuk iOS, hanya macOS)

## Instalasi

1. Clone repository ini:
   ```bash
   git clone https://github.com/username/KampusApp2.git
   cd KampusApp2
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

## Konfigurasi Firebase (PENTING)

Project ini menggunakan Firebase. Agar aplikasi dapat berjalan, Anda harus menggunakan konfigurasi Firebase Anda sendiri.

1. Buka [Firebase Console](https://console.firebase.google.com/).
2. Buat project baru atau gunakan project yang sudah ada.

### Untuk Android
1. Di Firebase Console, tambahkan aplikasi Android dengan package name: `com.kampusapp2` (atau sesuaikan `applicationId` di `android/app/build.gradle` jika Anda ingin mengubahnya).
2. Download file `google-services.json`.
3. Letakkan file `google-services.json` tersebut di dalam folder `android/app/`.

### Untuk iOS
1. Di Firebase Console, tambahkan aplikasi iOS dengan Bundle ID yang sesuai (default: `org.reactjs.native.example.KampusApp2` atau cek di Xcode).
2. Download file `GoogleService-Info.plist`.
3. Buka project `ios/KampusApp2.xcworkspace` menggunakan Xcode.
4. Klik kanan pada folder `KampusApp2` di sidebar kiri, pilih "Add Files to 'KampusApp2'..." dan pilih file `GoogleService-Info.plist` yang sudah didownload. Pastikan "Copy items if needed" tercentang.

## Menjalankan Aplikasi

### Android
Pastikan emulator Android sudah berjalan atau device fisik terhubung.
```bash
npm run android
```

### iOS (Hanya macOS)
```bash
cd ios
pod install
cd ..
npm run ios
```

## Lisensi

[MIT](LICENSE)

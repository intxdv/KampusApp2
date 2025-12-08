# **JADI CERITANYA GINI**
## Step 0 : Setup Framwork dan Package
### Setup Framerowk
Inisialisasi framework lewat CLI pake ```npx @react-native-community/cli init KampusApp2```, jangan lupa waktu cuma muncul 1 line downloading templates itu enter aja terus, tadi aku stuck di situ woilah T^T
### Install Package
```npm install @react-navigation/native```          : navigasi native
```npm install @react-navigation/native-stack```    : stack navigasi
```npm install @react-native-firebase/app```        : jembatan utama ke Firebase
```npm install @react-native-firebase/auth```       : auth Firebase
```npm install @react-native-firebase/firestore```  : firestore Firebase

## Step 1 : Buat Firebase Project dan Setup Konfigurasi
### Buat Firebase Project Android
1. Add Android App di project KampusApp2
2. Ada note:
> Your package name is generally the applicationId in your app-level build.gradle file
    Android package name : com.kampusapp2
    App nickname gausa gapapa
3. Download file ```google-servces.json```
4. Taroh di folder ```android/app/```

### Konfigurasi Firebase di Project
File ```google-servces.json``` ngga work secara sendirinya, kita perlu otak-atik konfigurasi Gradle nya dulu
1. Ke ```android/build.gradle```
2. Tambahkan ```classpath("com.google.gms:google-services:{versinya, liat dari instruksi}")``` di bagian dependencies
3. Lanjut ke ```android/app/build.gradle``` ambahkan ```apply plugin: "com.google.gms.google-services"``` di deretan apply2 plugin atas

## Step 2 : Mulai Mengoding
### 
# startup_namer

## Tugas 6 - Mobile Programming
### Oleh: Arbi Syarifudin (12181630)

___

## Soal dan Ketentuan

1. Mengikuti Panduan Dasar pembuatan Mobile App dengan Flutter melalui tautan berikut: 
   * [Write your first Flutter app, Part 1](https://flutter.dev/docs/get-started/codelab)
   * [Write your first Flutter app, Part 2](https://codelabs.developers.google.com/codelabs/first-flutter-app-pt2)

2. Menjelaskan Materi yang terdapat pada 2 (dua) panduan diatas.

## Penjelasan

### Bagian 1 : [Write your first Flutter app, Part 1](https://flutter.dev/docs/get-started/codelab)

   - Disini kita diajarkan untuk memulai membuat aplikasi flutter bernama 'Startup Name Generator' dengan nama project nya 'startup_namer'
   - Aplikasi tersebut berupa aplikasi sederhana yang akan menampilkan daftar nama-nama yang dibuat acak membentuk suatu nama dan frasa baru, dan bisa dipakai sebagai referensi penamaan startup
   - Caranya:
      1. Install Android Studio dan Flutter SDK dengan mengikuti panduan yang ada [disini](https://flutter.dev/docs/get-started/install).
      2. Buka **Visual Studio Code** (VS Code), lalu install Ektensi **Dart** dan **Flutter** di **Extension Marketplace**-nya VS Code.
      3. Setelah install berhasil, tekan tombol ```CTRL + SHIFT + P``` pada keyboard yang akan membuka *Command Pallete*
      4. Buka *Command Pallete*, ketik "```Flutter: New Project```", pilih ```Application```, dan cari folder untuk menyimpan project Flutter ini
      \
      \
      ![](SS/ss1-rfd.png)
      
      1. Pada *Commad Pallete* ketik "```Flutter: Run Flutter Doctor```", lalu klik atau enter untuk menjalankan pengecekan apakah semua persyaratan yang dibutuhkan oleh Flutter sudah terpenuhi. Tandanya adalah akan muncul suatu daftar *tool/library/dsb* yang diperlukan untuk menjalakan Flutter dan mereka akan **tercentang** semua. Jika ada yang bertanda **silang**, silakan install dia terlebih dahulu.
      \
      \
      ![](SS/ss2-rfd-term.png) 
      1. Buka *Command Pallete* dan ketik "```Flutter: Launch Emulator```", lalu pilih ```Create Emulator```, maka VS Code akan secara otomatis membuatkan kita sebuah emulator Android dan menjalankannya. Proses ini cukup memakan waktu, jadi tunggu saja.
      2.  Setelah selesai maka Emulator akan dijalankan dan aplikasi Flutter kita akan memunculkan tulisan "Hello World" jika kita mengikut panduannya dengan benar.
      \
      \
      ![](SS/ss3-run-emu.png) 
      1.  Tidak harus menggunakan Emulator, kita juga bisa menggunakan Smartphone yang kita miliki, dengan cara mengaktifkan ```USB Debugging``` pada Smartphone lalu menghubungkannya dengan Laptop kita.
      2.  Pada panduan tersebut, kita juga diajarkan bagaimana cara menginstall package / dependecy, misalnya package ```english_words```. Caranya:
      Buka file ```pubspec.yaml```, lalu pada bagian **dependencies:**, tambahkan 1 baris baru yaitu: \
          ```english_words: ^4.0.0```
      ```
      dependencies:
         flutter:
            sdk: flutter
         cupertino_icons: ^1.0.2
         english_words: ^4.0.0
      ```
      1.  Saat kita melakukan perubahan pada file ```pubspec.yaml```, VS Code akans secara otomatis menjalankan perintah ```flutter pub get``` untuk memasang dependency yang baru kita tambahkan. Namun jika tidak berjalan, cukup jalankan secara manual via terminal.
      2.  Dimateri tersebut juga diajarkan cara membuat fungsi custom bernama ```randomWords()``` untuk generate kata-kata secara acak.
      3.  Diajarkan juga cara buat infinite scrolling ListView untuk menampilkan halaman listView berupa daftar **nama startup** acak yang digenerate secara otomatis tadi
      4.  List tersebut bisa kita berikan tombol **love** untuk menyimpannya ke dalam **list tersimpan** agar user bisa melihat lagi nanti
      5.  Diajarkan juga tentang Navigation Route untuk pindah halaman 
      6.  Selesai
          
# Dokumentasi Refactoring - Week 03 (Factory & Singleton)

## Perubahan yang Dilakukan
1. **Implementasi Singleton**: Mengubah `PaymentFactory` menjadi Singleton untuk memastikan pengelolaan strategi pembayaran terpusat dan hemat memori.
2. **Implementasi Factory**: Memindahkan logika pembuatan objek `PaymentStrategy` dari `Main` ke dalam `PaymentFactory`.

## Alasan Refactoring
* **Efisiensi**: Dengan Singleton, kita tidak membuat objek Factory baru setiap kali ada transaksi.
* **Fleksibilitas**: Mengikuti prinsip Spring, kode utama kini cukup meminta objek ke Factory tanpa perlu tahu cara instansiasinya.

## Cara Menjalankan
1. Jalankan `javac index.java`
2. Jalankan `java index`
3. Masukkan harga dan pilih metode pembayaran (Factory akan menyediakan objeknya).

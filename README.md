Class Produk (Abstraksi):
Kelas ini adalah kelas abstrak yang mewakili produk umum. Setiap produk memiliki kode dan harga.
Kelas ini menyediakan metode untuk mendapatkan dan mengubah harga, serta metode abstrak tampilkanInfo() yang harus diimplementasikan oleh subclass.

Class Koper (Inheritance dari Produk):
Koper adalah subclass dari Produk, yang mewakili produk koper. Selain kode dan harga, koper juga memiliki atribut merk.
Kelas ini mengimplementasikan metode tampilkanInfo() untuk menampilkan detail koper.

Interface CRUDOperations:
Interface ini mendefinisikan metode dasar untuk operasi CRUD (Create, Read, Update, Delete), yang nantinya diimplementasikan oleh kelas manajer koper.

Class KoperManager (Implementasi CRUD):
Kelas ini bertanggung jawab untuk mengelola daftar koper.
Kelas ini menggunakan ArrayList<Koper> untuk menyimpan daftar koper.
Koper default (5 koper) sudah ditambahkan di konstruktor.
Metode tambah(), lihat(), update(), dan hapus() diimplementasikan untuk menambah, melihat, memperbarui, dan menghapus koper dalam daftar.
Metode menuUtama() menyediakan antarmuka berbasis teks untuk pengguna, memungkinkan mereka berinteraksi dengan daftar koper (memilih menu CRUD).

Class Main:
Kelas ini adalah titik awal program. Di sini, objek KoperManager dibuat, dan metode menuUtama() dipanggil untuk memulai interaksi dengan pengguna.

Cara Kerja:
Program menampilkan menu utama kepada pengguna:
Tambah koper baru.
Lihat daftar koper.
Update koper yang ada.
Hapus koper berdasarkan kode.
Keluar dari aplikasi.
Pengguna dapat memilih opsi dari menu, dan program akan menjalankan fungsi sesuai dengan pilihan pengguna (misalnya, menambahkan koper baru atau melihat daftar koper).
Daftar koper diinisialisasi dengan 5 koper default saat KoperManager dibuat.

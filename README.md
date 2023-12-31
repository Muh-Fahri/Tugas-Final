# database Data Barang

## Menjalankan Aplikasi
1. Pastikan anda telah menjalankan MySQL Server.
2. Kompilasi serta jalankan kelas `App.java` untuk memulai aplikasi.
3. Pada menu utama, Anda dapat memilih opsi yang tersedia:
   - Opsi 1 untuk membaca data barang dari sebuah database.
   - Opsi 2 untuk menambahkan data barang baru ke dalam database.
   - Opsi 3 untuk mengubah suatu data barang yang ada di database.
   - Opsi 4 untuk menghapus data barang dari database.
   - Opsi 0 untuk keluar dari aplikasi.

## Struktur Proyek

- Folder `com.config` berisi kelas `DbConnect` yang berfungsi mengatur koneksi ke database.
- Folder `com.controller` berisi kelas `DBController` yang berfungsi sebagai pengontrol data barang di database.
- Folder `com.layout` berisi berbagai kelas yang berfungsi mengatur tampilan dan interaksi dengan pengguna.
- Folder `com.models` berisi kelas `Produk` yang berfungsi mewakili model data barang.

## com.layout
Menu:berfungsi sebagai menu utama aplikasi. Metode showMenu() digunakan untuk menampilkan opsi menu kepada pengguna dan mengarahkan ke opsi yang dipilih.
ReadData:untuk membaca serta menampilkan data barang dari database kepada pengguna. Metode getDatabase() digunakan untuk mengambil data dari database dan menampilkannya di layar.
InsertData:untuk menambahkan data barang baru ke database. Metode insertData() meminta pengguna memasukkan detail barang baru seperti nama, harga, dan jumlah, kemudian data tersebut akan disimpan di database.
EditData:untuk mengubah jumlah barang yang ada di database. Metode editData() meminta pengguna memasukkan ID barang yang ingin diubah dan jumlah baru, kemudian data akan diperbarui di database.
DeleteData:menghapus data barang dari database. Metode deleteData() meminta pengguna memasukkan ID barang yang ingin dihapus, kemudian data tersebut akan dihapus dari database.
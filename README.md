#tugas pertemuan 

##profil
| Variable       |    DATA DIRI         |
| ---------------| ----------------     |
| Nama           | Lutpiah Ainus Shiddik|                                     
| NIM            | 312310474            |
| Kelas          | TI.23.A.5            |
| Mata Kuliah    |Basis data            |
 
 # Soal Latihan Praktikum
## 1. Tulis semua perintah-perintah SQL percobaan di atas beserta outputnya!

*1. Buat sebuah database dengan nama latihan2*

Untuk membuat database gunakan perintah sebagai berikut :

`CREATE DATABASE [nama_database]`

`CREATE DATABASE latihan2;`

lalu, setelah kita membuat database. kita masuk kedalam database tersebut dengan perintah sebagai berikut :

`USE latihan2;`

![Alt text](<gambar ss/nomor ss 1.png>)

*2. Buat sebuah tabel dengan nama biodata (nama, alamat) didalam database latihan2!*

Untuk membuat Tabel gunakan perintah sebagai berikut :

`CREATE TABLE nama_tabel (
    nama_field1 tipe _data(ukuran), nama_field2 tipe_data(ukuran), ..., nama_fieldn tipe_data(ukuran)
    );`

`CREATE TABLE biodata (
    nama varchar (100),
    alamat text
    );`

![Alt text](<gambar ss/nomor ss 2.png>)

*3. Tambahkan sebuah kolom keterangan (varchar 15), sebagai kolom terakhir!*

Contoh :

`ALTER TABLE biodata ADD COLUMN keterangan VARCHAR (15);`

![Alt text](<gambar ss/nomor ss 3.png>)

*4.Tambahkan kolom id(int 11) di awal (sebagai kolom pertama)!*

Untuk menambahkan kolom pertama yaitu dengan perintah sebagai berikut :

`ALTER TABLE biodata ADD COLUMN id int FIRST; `

![Alt text](<gambar ss/nomor ss 4.png>)

*5. Sisipkan sebuah kolom dengan nama phone (varchar 15) setelah kolom alamat!*

Untuk menambahkan kolom setelah kolom lain yaitu dengan perintah `AFTER`

![Alt text](<gambar ss/nomor ss 5.png>)

*6. Ubah tipe data kolom id menjadi char(11)!*

Untuk mengubah type data yaitu dengan perintah sebagai berikut :

`ALTER TABLE [nama_tabel] MODIFY nama_field tipe_data_baru(ukuran);`

![Alt text](<gambar ss/nomor ss 6.png>)

*7. Ubah nama kolom phone menjadi hp (char 20)!*

Untuk mengubah kolom yaitu dengan perintah sebgai berikut :

`ALTER TABLE [nama_tabel] CHANGE nama_field_lama nama_field_baru tipe_data(ukuran);`

![Alt text](<gambar ss/nomor ss 7.png>)

*8. Tambahkan kolom email setelah kolom hp*

![Alt text](<gambar ss/nomor ss 8.png>)

*9. Hapus kolom keterangan dari tabel!*

Untuk menghapus kolom dari tabel yaitu dengan perintah sebagai berikut :

`ALTER TABLE [nama_tabel] DROP nama_field;`

![Alt text](<gambar ss/nomor ss 9.png>)

*10. Ganti nama tabel menjadi data_mahasiswa!*

Untuk mengganti nama tabel yaitu dengan perintah sebagai berikut :

`ALTER TABLE [nama_tabel] RENAME [nama_tabel_baru];`

![Alt text](<gambar ss/nomor ss 10.png>)

*11. Ganti nama field id menjadi nim!*

![Alt text](<gambar ss/nomor ss 11.png>)

*12. Jadikan nim sebagai PRIMARY KEY!*

Untuk menambahkan index atau key, gunakan perintah sebagai berikut :

tipe index :

- PRIMARY KEY
- UNIQUE KEY
- FULLTEXT

`ALTER TABLE [nama_tabel] ADD [INDEX|PRIMARY KEY] (nama_field);`

![Alt text](<gambar ss/nomor ss 12.png>)

*13. Jadikan kolom email sebagai UNIQUE KEY!*

Perintah nya sama seperti diatas, hanya saja diganti menjadi UNIQUE KEY

![Alt text](<gambar ss/nomor ss 13.png>)

## 2. Apa Maksud Dari INT(11) ?

Pada konteks basis data, INT(11) merujuk pada jenis data integer dengan panjang 11 digit

## 3. Ketika Kita Melihat Struktur Tabel Dengan Perintah DESC , Ada Kolom Null yang Berisi Yes dan No. Apa Maksudnya ?

Yes: Menandakan bahwa nilai dalam kolom tersebut boleh kosong. Artinya, tidak wajib mengisi setiap baris dengan data pada kolom tersebut.

No: Menandakan bahwa nilai dalam kolom tersebut tidak boleh kosong. Setiap baris harus memiliki nilai untuk kolom tersebut.

##terimakasih pak


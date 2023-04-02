# Tugas-Basis-Data

1. Buat sebuah database dengan nama latihan2!
``` 
CREATE DATABASE latihan1;
```
![bdata 1](https://user-images.githubusercontent.com/115356128/229334957-bac06184-b49b-4fd3-b0c4-f241e0881d68.png)


2. Buat sebuah tabel dengan nama biodata (nama, alamat) didalam
database latihan1!
```
CREATE TABLE siswa (nama VARCHAR(100), alamat TEXT);
```
![bdata 2](https://user-images.githubusercontent.com/115356128/229334988-a9ac6897-3f66-46ef-a831-d19ce13d1b34.png)


3. Tambahkan sebuah kolom keterangan (varchar 15), sebagai kolom
terakhir!
```
ALTER TABLE siswa ADD COLUMN keterangan varchar(15) TEXT AFTER alamat;
```
![bdata 3](https://user-images.githubusercontent.com/115356128/229334996-3b8ed532-96ae-487f-a753-c6bfe61ae9bb.png)


4. Tambahkan kolom id (int 11) di awal (sebagai kolom pertama)!
```
ALTER TABLE siswa ADD COLUMN id int(11) TEXT First;
```
![bdata 4](https://user-images.githubusercontent.com/115356128/229335001-339d3972-e0ec-41a1-8b07-419fc6adc5cd.png)


5. Sisipkan sebuah kolom dengan nama phone (varchar 15) setelah
kolom alamat!
```
ALTER TABLE siswa ADD COLUMN phone varchar(10) after alamat;
```
![bdata 5](https://user-images.githubusercontent.com/115356128/229335004-06620cf0-2fc1-4f9c-a69b-0c527071307c.png)


6. Ubah tipe data kolom id menjadi char(11)!
```
ALTER TABLE siswa MODIFY COLUMN id VARCHAR(11);
```
![bdata 6](https://user-images.githubusercontent.com/115356128/229335014-14aa7f4f-87bb-49c1-8cd6-100d4082bca0.png)


7. Ubah nama kolom phone menjadi hp (varchar 20)!
```
ALTER TABLE siswa CHANGE COLUMN phone hp varchar(20);
```
![bdata 7](https://user-images.githubusercontent.com/115356128/229335021-30d15d7f-64e3-4939-8923-369f1b1e7802.png)


8. Tambahkan kolom email setelah kolom hp
```
ALTER TABLE siswa ADD COLUMN email text after hp;
```
![bdata 8](https://user-images.githubusercontent.com/115356128/229335037-bcf5a062-5d3c-4a25-a586-8b657acc9d7b.png)


9. Hapus kolom keterangan dari tabel!
```
alter table siswa drop keterangan;
```
![bdata 9](https://user-images.githubusercontent.com/115356128/229335044-7a78c3fb-76e4-4c99-bdb7-8d6c4e0e71e0.png)


10. Ganti nama tabel menjadi data_mahasiswa!
```
alter table siswa rename data_mahasiswa;
```
![bdata 10](https://user-images.githubusercontent.com/115356128/229335046-b7547cd1-98e1-4627-b209-19b33cc21ed4.png)


11. Ganti nama field id menjadi nim!
```
ALTER TABLE data_mahasiswa CHANGE COLUMN id nim varchar(11);
```
![bdata 11](https://user-images.githubusercontent.com/115356128/229335050-1590d861-4af9-4a19-aac0-adb34e40135e.png)


12. Jadikan nim sebagai PRIMARY KEY!
```
ALTER TABLE data_mahasiswa ADD PRIMARY KEY(nim);
```
![bdata 12](https://user-images.githubusercontent.com/115356128/229335054-583270b2-e5ad-4ce9-b54a-c6f89f0b44a2.png)


13. Jadikan kolom email sebagai UNIQUE KEY
```
ALTER TABLE data_mahasiswa ADD CONSTRAINT email unique KEY(email);
```
![bdata 13](https://user-images.githubusercontent.com/115356128/229335058-3e334837-dd2c-4efa-aab4-62b766f35f06.png)


14. Hasil akhir

![bdata 14](https://user-images.githubusercontent.com/115356128/229335067-6f9423e3-aa30-4d59-8326-7fe6d6739f6e.png)


# Evaluasi dan pertanyaan
1. Apa maksud dari int (11)?
```
int (11) nunjukkan bahwa kolom memiliki tipe data bilangan bulat (integer) dengan ukuran 11 digit 
```

2. Ketika kita melihat struktur tabel dengan perintah desc, ada kolom Null yang
berisi Yes dan No. Apa maksudnya ?
```
Jika kolom "Null" adalah "YES", itu berarti kolom tersebut diizinkan untuk memiliki nilai NULL.

Jika kolom "Null" adalah "NO", maka kolom tersebut tidak diizinkan untuk memiliki nilai NULL
```

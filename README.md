# Tugas-Basis-Data

1. Buat sebuah database dengan nama latihan2!
``` 
CREATE DATABASE latihan1;
```

2. Buat sebuah tabel dengan nama biodata (nama, alamat) didalam
database latihan1!
```
CREATE TABLE siswa (nama VARCHAR(100), alamat TEXT);
```

3. Tambahkan sebuah kolom keterangan (varchar 15), sebagai kolom
terakhir!
```
ALTER TABLE siswa ADD COLUMN keterangan varchar(15) TEXT AFTER alamat;
```

4. Tambahkan kolom id (int 11) di awal (sebagai kolom pertama)!
```
ALTER TABLE siswa ADD COLUMN id int(11) TEXT First;
```

5. Sisipkan sebuah kolom dengan nama phone (varchar 15) setelah
kolom alamat!
```
ALTER TABLE siswa ADD COLUMN phone varchar(10) after alamat;
```

6. Ubah tipe data kolom id menjadi char(11)!
```
ALTER TABLE siswa MODIFY COLUMN id VARCHAR(11);
```

7. Ubah nama kolom phone menjadi hp (varchar 20)!
```
ALTER TABLE siswa CHANGE COLUMN phone hp varchar(20);
```

8. Tambahkan kolom email setelah kolom hp
```
ALTER TABLE siswa ADD COLUMN email text after hp;
```

9. Hapus kolom keterangan dari tabel!
```
alter table siswa drop keterangan;
```

10. Ganti nama tabel menjadi data_mahasiswa!
```
alter table siswa rename data_mahasiswa;
```

11. Ganti nama field id menjadi nim!
```
ALTER TABLE data_mahasiswa CHANGE COLUMN id nim varchar(11);
```

12. Jadikan nim sebagai PRIMARY KEY!
```
ALTER TABLE data_mahasiswa ADD PRIMARY KEY(nim);
```

13. Jadikan kolom email sebagai UNIQUE KEY
```
ALTER TABLE data_mahasiswa ADD CONSTRAINT email unique KEY(email);
```

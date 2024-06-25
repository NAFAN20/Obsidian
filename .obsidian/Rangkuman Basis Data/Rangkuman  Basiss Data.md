# penggunaan awal MySQL

### Query

```mysql
<mysql -u root -p>
```
### Hasil
![gambar](Asset/Asset1BD.png)

## membuat data base

- `CREATE DATABASE` adalah perintah untuk membuat database baru.
- `[XI_RPL_1]` adalah nama yang Anda pilih untuk database baru Anda. Tanda kurung siku `<("[]")>` digunakan di sini untuk menghindari kesalahan jika nama database mengandung karakter spesial atau spasi. Namun, perlu dicatat bahwa tidak semua DBMS mengizinkan penggunaan tanda kurung siku dalam nama database, jadi pastikan untuk menyesuaikan sintaksdengan DBMS yang Anda gunakan.
### Query

```mysql
create database xi_rpl_1;
```
### Hasil:
![gambar](Asset/Asset2BD.png)

## Tampilkan data base

`SHOW DATABASE` digunakan untuk menampilkan daftar database yang ada dalam sistem manejemen basis data (DBMS). Perintah ini dapat digunakan di beberapa DBMS seperti MYSQL, PostgreSQL, dan beberapa DBMS lainnya. Namun, perintahnya dapat sedikit berbeda tergantung

### Query

```mysql
show databases;
```
### Hasil:
![gambar](Asset/Asset3BD.png)
## Hapus database

`<DROP DATABASE [nama_database]>` digunakan dalam sistem manajemen basis data (DBMS) untuk menghapus sebuah database beserta semua objek yang terkait dengan database tersebut, seperti tabel, indeks, tampilan, prosedur tersimpan, dan lain-lain.

### Query

```mysql
drop database xi_rpl_1;
```
### Hasil:
![gambar](Asset/Asset4BD.png)

## gunakan data base

`USE [nama_database]` digunakan dalam sistem manajemen basis data (DBMS) untuk beralih atau memilih database yang akan digunakan. Ketika Anda menggunakan perintah `<USE>` diikuti dengan nama database, DBMS akan mengarahkan semua perintah dan operasi selanjutnya pada database yang ditentukan.

### Query
```mysql
use rental_nafan;
```
### Hasil:
![gambar](Asset/Asset5BD.png)

## Membuat Tabel 

- Membuat tabel bernama `nafan_tables`.
- Tabel memiliki tiga kolom: `nama`, `alamat`, dan `catatan`.
- `nama` menyimpan teks maksimal 50 karakter.
- `alamat` menyimpan teks maksimal 100 karakter.
- `catatan` menyimpan teks panjang.

### Query
```mysql
CREATE TABLE nafan_tables (
    nama CHAR(50),
    alamat VARCHAR(100),
    catatan TEXT,
);
```
### Hasil : 

![gambar](Asset/42.png)

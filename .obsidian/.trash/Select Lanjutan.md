# AND
## Struktur Query
mysql
SELECT kolom1,kolom2 FROM [nama_tabel] WHERE kolom1="nilai1" AND kolom2="nilai2";

## Contoh Query
MYSQL
SELECT warna,pemilik FROM mobil WHERE warna="HITAM" AND pemilik="NAFAN";

## Hasil
![[Screenshot 2024-02-20 141411.png|500]]

## Analisis

## Kesimpulan


# OR
## Struktur Query
MYSQL
 SELECT kolom1,kolom2 FROM [nama_tabel] WHERE kolom1="nilai1" OR kolom2="nilai2";

## Contoh Query
MYSQL
 SELECT warna,pemilik FROM mobil WHERE warna="HITAM" OR pemilik="NAFAN";

## Hasil
![[lanjutan (2).png|500]]

## Analisis

## Kesimpulan

# BETWEEN
## Struktur Query
MYSQL
 SELECT * FROM [nama_tabel] WHERE kolom1 BETWEEN nilai1 AND nilai2;

## Contoh Query
mysql
 SELECT * FROM mobil WHERE harga_rental BETWEEN 50000 AND 100000;

## Hasil
![[lanjutan (3).png|500]]

## Analisis
## Kesimpulan
# NOT BETWEEN
## Struktur Query
MYSQL
 SELECT * FROM [nama_tabel] WHERE kolom1 NOT BETWEEN nilai1 AND nilai2;

## Contoh Query
MYSQL
 SELECT * FROM mobil WHERE harga_rental NOT BETWEEN 100000 AND 150000;
## Hasil
![[not between.png|500]]

Analisis
Kesimpulan
# <=
## Struktur Query
mysql
 SELECT * FROM [nama_tabel] WHERE kolom1 <= nilai1;

 ## Contoh Query
mysql
 SELECT * FROM mobil WHERE harga_rental <= 100000;

## Hasil
![[lebih kecil.png|500]]

## Analisis

 ## Kesimpulan

# >=
 ## Struktur Query
mysql
SELECT * FROM [nama_tabel] WHERE kolom1 >= nilai1;

## Contoh Query
mysql
SELECT * FROM mobil WHERE harga_rental >= 100000;

## Hasil
![[lebih besar.png|500]]

## Analisis

## Kesimpulan
# <> atau !=
## Struktur Query
mysql
SELECT * FROM [nama_tabel] WHERE kolom1 <> nilai1;

SELECT * FROM [nama_tabel] WHERE kolom1 != nilai1;

## Contoh Query
````mysql
SELECT * FROM mobil WHERE harga_rental <> 100000;

SELECT * FROM mobil WHERE harga_rental != 50000; ````

## Hasil
![[tidak sama dengan.png|500]]

![[tdk sma dgn.png|500]]

## Analisis

## Kesimpulan

# Tantangan Login
# IN
## IN + AND
## IN + OR
## IN + AND OPERATOR
## Table Virtual
# AGREGASI
## Select AVG
### Analisis:
Perintah SQL `SELECT AVG` digunakan untuk menghitung rata-rata dari nilai-nilai dalam satu kolom tertentu dalam tabel database. Ini sangat berguna saat Anda ingin mendapatkan nilai rata-rata dari data numerik dalam database Anda.
### Contoh Query
```
SELECT AVG(Harga_Rental) AS Rata_Rata From Mobil;
```
### Hasil:

## Select Min
### Analisis:
Perintah SQL `SELECT MIN()` digunakan untuk mengambil nilai minimum dari kolom tertentu dalam tabel database. Ini sangat berguna ketika Anda perlu menemukan nilai terkecil dalam satu kolom.
### Contoh Query
```
SELECT MIN (Harga_rental) AS Minimal From Mobil;
```
### Hasil:

## Select Count
### Analisis:
Dalam SQL, perintah `SELECT COUNT()` digunakan untuk menghitung jumlah baris yang cocok dengan kriteria tertentu dalam sebuah tabel. Analisis program `SELECT COUNT()` dapat meliputi beberapa aspek, termasuk kinerja, fungsionalitas, dan optimasi 
1. **Kinerja**: Perintah `SELECT COUNT()` bisa menjadi mahal dari segi kinerja, terutama jika tabelnya sangat besar. Hal ini karena database harus memindai seluruh tabel untuk menghitung jumlah baris yang cocok dengan kriteria. Dalam situasi di mana kinerja menjadi perhatian, pertimbangkan untuk menggunakan indeks pada kolom yang relevan untuk meningkatkan kinerja operasi pencarian.
    
2. **Fungsionalitas**: `SELECT COUNT()` memungkinkan Anda untuk menghitung jumlah baris yang memenuhi kriteria tertentu. Misalnya, Anda bisa menghitung jumlah baris dengan kondisi tertentu, seperti jumlah pengguna dengan usia di atas 18 tahun. Kombinasikan dengan klausul WHERE untuk menentukan kriteria pencarian.
    
3. **Optimasi**: Dalam beberapa kasus, Anda mungkin dapat mengoptimalkan perintah `SELECT COUNT()` dengan menggunakan strategi tertentu. Misalnya, jika Anda hanya tertarik pada jumlah baris yang sesuai dengan kriteria tertentu dan tidak memerlukan nilai yang sesuai, Anda bisa menggunakan `SELECT COUNT(*)` daripada `SELECT COUNT(column_name)`, karena yang pertama lebih efisien. Selain itu, Anda bisa mempertimbangkan penggunaan `HAVING` daripada `WHERE` jika Anda ingin memfilter hasil setelah penghitungan dilakukan.
### Contoh Query
```
SELECT COUNT (Pemilik) From Mobil;
```
### Hasil:


## Select Sum 
### Analisis:
Program SELECT SUM dalam SQL digunakan untuk menghitung total jumlah nilai dalam kolom numerik dari tabel yang sesuai dengan kondisi yang diberikan. Misalnya, jika Anda memiliki tabel "penjualan" dengan kolom "jumlah" yang berisi jumlah penjualan, Anda dapat menggunakan SELECT SUM untuk mengetahui total penjualan.
### Contoh Query
```
SELECT SUM (harga_rental) From Mobil;
```
### Hasil: 


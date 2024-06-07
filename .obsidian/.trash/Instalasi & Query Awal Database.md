 # Instalasi MySQL
* 1. Berikan akses termux ke memori internal
	 termux-setup-storage
* 2. Muncul pop-up untuk meminta izin akses ke memori internal
	klik izinkan/allow acces
* 3. Lakukan uptade dan sekaligus upgrade paket
	pkg upgrade && upgrade -y
* 4. jika ada konfirmasi untuk melanjutkan instalasi. silahkan klik
	y dan enter
* 5. instal aplikasi MariaDB
	pkg install mariadb
* 6. Memberikan Akses aman ke MySQL
	mysqld_Safe
* 7.  Hentikan Proses
	CTRL+Z
* 8. Masuk Kedalam admin
	mysql -u root
### Menggunakan XAMPP
* 1. Buka Xampp 
* 2. Klik `start` di MySQL  
* 3.  Klik `Shell`
* 4. Masuk Kedatabase dengan akun administrator `mysql -u root -p 
	Passwordny Kosong Jadi silahkan langsung enter
* 5. Buat Database
* Create Database `[nama_database];`
* 6.Tampilkan Database
* Contoh
* `Show databases`
* 7.Hentikan Proses
* Contoh
*  `Drop Database xi_rpl_1;`
* 8. Menggunakan Da\tabase;
* use`[nama_database];`
* contoh
* `Use_kelas;`

### Referensi Video youtube
https://www.youtube.com/watch?v=0HHtGx0cDAg
### Penggunaan Awal MySQL
* 1. Buka Xampp 
* 2. Klik `start` di MySQL  
* 3.  Klik `Shell`
* 4. Masuk Kedatabase dengan akun administrator `mysql -u root -p`
	Passwordny Kosong Jadi silahkan langsung enter
* 5. Buat Database
* Create Database [nama_database];
* 6.Tampilkan Database
* Contoh
* Show databases
* 7.Hentikan Proses
* Contoh
*  Drop Database xi_rpl_1;
* 8. Menggunakan Da\tabase;
* use [nama_database];
* contoh
* Use_kelas;

 Analisis :
* ==`MySQL`== Ini adalah klien baris perintah untuk MySQL.
* ==`-u root` ==Ini menentukan pengguna MySQL yang ingin Anda login sebagai, dalam hal ini, 'root'..
* ==`-p`== Opsi ini memberitahu MySQL untuk meminta kata sandi. Setelah memasukkan perintah ini, Anda akan diminta memasukkan kata sandi untuk pengguna 'root'.
Jadi, saat Anda menjalankan perintah mysql -u root -p, pada dasarnya perintah tersebut berbunyi, "Masuk ke MySQL sebagai pengguna 'root' dan minta kata sandi."

Contoh Query Mysql :
```mysql
mysql -u root -p
```

Hasil : 
![[termux.png]]

 Kesimpulan:
Jalankan perintah untuk masuk ke MySQL: `mysql -u root -p`. Anda mungkin diminta memasukkan kata sandi; biarkan kosong jika Anda belum mengaturnya
### Create Database

Analisis:
 Dalam rangka membuat database dalam XAMPP, Anda dapat menggunakan antarmuka grafis phpMyAdmin melalui peramban web atau antarmuka baris perintah MySQL menggunakan perintah SQL `CREATE DATABASE`. Pastikan selalu mempertimbangkan praktik terbaik untuk pengelolaan dan keamanan basis data dalam lingkungan pengembangan Anda.
 
 Query Create Database:
```mysql
Create Databases;
```

 Hasil

![[Pasted image 20240426063728.png]]
Kesimpulan : 
Di sini, `nama_database` adalah nama yang Anda pilih untuk database baru yang akan dibuat. Setelah menjalankan query ini, sistem akan membuat database baru dengan nama yang Anda tentukan.
### Show Databases
Analisis: 
SHOW DATABASES digunakan untuk menampilkan daftar semua database yang ada dalam sistem manajemen basis data (DBMS) yang sedang digunakan. Ini adalah perintah standar yang sering digunakan di banyak DBMS, meskipun sintaksisnya mungkin sedikit berbeda tergantung pada sistem yang digunakan.

Query show databases:
```mysql
Show Databases;
```

Hasil : 
![[Pasted image 20240426082831.png]]

Kesimpulan :
Dengan demikian, untuk menampilkan database dalam XAMPP, Anda dapat menggunakan phpMyAdmin melalui peramban web atau antarmuka baris perintah MySQL. Di phpMyAdmin, navigasikan ke tab "Databases", dan di antarmuka baris perintah, gunakan perintah SQL `SHOW DATABASES;`.
### Drop Database
Analisis:
1. **DROP DATABASE:** Ini adalah perintah SQL untuk menghapus sebuah database.
2. **XI_RPL_1:** Nama database yang akan dihapus. Pastikan bahwa Anda telah memverifikasi dengan benar bahwa database yang dimaksud adalah yang dimaksudkan untuk dihapus.

Query Drop Database
```mysql
	DROP DATABASE senapan_rpl1;
```

Hasil:
![[Pasted image 20240426082906.png]]

Kesimpulan:

### Use Database
Analisis:
Perintah `USE DATABASE` digunakan dalam SQL untuk beralih ke database tertentu.
Misalkan Anda memiliki beberapa database dalam sistem database Anda, dan Anda ingin bekerja di dalam salah satu database tersebut. Anda menggunakan perintah `USE DATABASE` untuk menentukan database mana yang akan Anda gunakan untuk menjalankan perintah-perintah SQL selanjutnya.

Query Use Database :
```mysql
use databases [Name];
```

Hasil:
![[Pasted image 20240427020042.png]]

Kesimpulan : 
Dalam kesimpulan, untuk menggunakan database tertentu dalam XAMPP, Anda dapat memilihnya melalui antarmuka web phpMyAdmin atau menggunakan perintah SQL `USE` dalam antarmuka baris perintah MySQL. Pastikan untuk mengganti `nama_database` dengan nama database yang sesuai.

### Create Tables
Analisis : 
Program tersebut merupakan sebuah skrip SQL untuk membuat sebuah database dan tabel baru bernama "Pelanggan". Mari kita analisis langkah demi langkah:
1. `CREATE TABLE Pelanggan`: Ini membuat sebuah tabel bernama "Pelanggan" dalam database yang telah dibuat sebelumnya (atau yang sudah ada). Tabel ini memiliki empat kolom:
    - `id_pelanggan`: Sebuah bilangan bulat dengan panjang maksimum 4 digit (int(4)), yang dipilih sebagai primary key (kunci utama). Primary key tidak boleh kosong (not null).
    - `nama_depan`: Sebuah string teks dengan panjang maksimum 25 karakter (varchar(25)), yang tidak boleh kosong (not null).
    - `nama_belakang`: Sebuah string teks dengan panjang maksimum 25 karakter (varchar(25)). Kolom ini boleh kosong, karena tidak ada klausul "not null".
    - `no_telp`: Sebuah string teks dengan panjang tepat 12 karakter (char(12)), yang dijadikan unik (unique). Ini berarti tidak ada dua baris dalam tabel yang bisa memiliki nomor telepon yang sama.
2. `SHOW DATABASES;`: Ini adalah perintah SQL yang menampilkan daftar semua database yang ada di server database. Namun, perintah ini tidak dapat dieksekusi bersamaan dengan perintah SQL lainnya dalam sebagian besar DBMS. Perintah ini biasanya dijalankan secara terpisah, terutama pada command-line interface seperti MySQL shell.
3. `DESCRIBE Pelanggan;`: Ini adalah perintah SQL untuk menampilkan struktur tabel "Pelanggan", yang menghasilkan deskripsi singkat tentang struktur kolom dalam tabel tersebut. Perintah ini akan menampilkan nama kolom, tipe data, dan beberapa informasi lainnya tentang setiap kolom dalam tabel "Pelanggan".

Query Create Table
```mysql
Create table Pelanngan(
id_pelanggan int(4) primary key not null,
nama_depan varchar(25) not null,
nama_belakang varchar(25),
no_telp char(12) unique);
lalu Ketik = Show Databases; 
jika sudah menampilkan hasil databases ketik lagi = describe pelanggan;
Hasilnya seperti dibawa
```

Hasil : 
![[Pasted image 20240427020146.png]]
### Tipe Data
INT  (integer) = digunakan untuk menyimpan bilangan bulat seperti 1.42.10
### Teks
VARCHAR=Digunakan untuk menyimpan teks dengan panjang variabel seperti nama,alamat email
CHAR =digunakan untuk menyimpan teks dengan panjang tetap seperti code pos
TEXT=digunakan untuk menyimpan tanggal seperti 2023-10-01
### Tanggal
Date=Digunakan untuk menyimpan tanggal seperti 2023-10-01
THE 
DateTime=Digunakan Untuk menyimpan tanggal dan waktu seperti 2023-10-01 21:00Pm

### Boolean

### Enum 
`Enum` berfungsi hanya bisa memilih 1,misalkan jenis kelamin Ada L atau P   
L = Adalah Laki-Laki
P = Adalah perempuan

### Set
`set`Berfungsi hanya bisa memilih lebih dari 1,misalkan Hobi Seperti Berenang,makan,main game,jogging,workout 

### QNA

>[!QnA] Mengapa Hanya kolom id_pelanggan yang menggunakan contraint primary key? 
>1. **Unik**: Setiap pelanggan biasanya memiliki ID pelanggan yang unik. Dengan menggunakan ID pelanggan sebagai primary key, Anda dapat dengan mudah memastikan bahwa setiap baris dalam tabel memiliki identifikasi yang unik.
>2. **Stabil**: ID pelanggan biasanya tidak berubah sepanjang waktu. Ini penting karena primary key seharusnya tidak berubah, karena merupakan cara untuk mengidentifikasi unik setiap baris dalam tabel. Jika primary key berubah secara teratur, dapat menyebabkan masalah integritas referensial dan konsistensi data.
>3. **Performa**: Menggunakan kolom yang memiliki nilai unik dan tidak terlalu banyak perubahan seringkali dapat meningkatkan kinerja operasi pencarian dan penggabungan data.


>[!QnA] Mengapa pada kolom no_telp yang menggunakan tioe data char bukan varchar?
> CHAR 
>Tipe data `CHAR` digunakan untuk menyimpan string karakter dengan panjang tetap.
Panjang karakternya tetap, sehingga jika Anda mendefinisikan `CHAR(10)`, maka kolom tersebut selalu akan menyimpan 10 karakter, padat atau tidak.
 Keuntungan dari `CHAR` adalah kecepatan pencarian dan pengindeksan karena panjang data tetap.
Namun, untuk nomor telepon, yang panjangnya mungkin bervariasi, penggunaan `CHAR` bisa mengakibatkan pemborosan ruang penyimpanan.


>[!QnA] Mengapa hanya kolom no_telp yang ,menggunakan contraint unique?
>1. **Unik sebagai Identifier:**
> Nomor telepon sering digunakan sebagai cara untuk mengidentifikasi entitas tertentu, seperti pelanggan atau karyawan.
Menyimpan nomor telepon yang sama untuk dua entitas yang berbeda dapat menyebabkan kebingungan atau masalah dalam pemrosesan data.  
2.**Integritas Data:** 
Constraint UNIQUE membantu menjaga integritas data dengan mencegah adanya duplikat.
 Dengan mencegah duplikasi nomor telepon, tabel tetap konsisten dan dapat diandalkan.
 3.Kemudahan Pencarian dan Pemutakhiran 
 Dengan constraint UNIQUE, operasi pencarian dan pemutakhiran data yang melibatkan nomor telepon dapat dilakukan secara efisien, karena tidak perlu mempertimbangkan kemungkinan adanya duplikat. 


>[!QnA] Mengapa kolom no_telp tidak memakai contraint not null sementara kolom lainnya menggunakan contraint tersebut
>Karena No tlp dianggap opsional nomor telepon hanya menjadi wajib isi saat pengguna melakukan langkah langkah tertentu tetapi mungkin tidak mengwajibkan pengisian telepon pada awal pengisian data

>[!QnA] apa perbedaan Primary key denga unique?
>kalau primary key untuk membedakan data yang sama dan hanya boleh 1 dan tidak ada sedangkan unique boleh 1,2,3 dan seterusnya dan tidak boleh ada

# INSERT
## INSERT 1 DATA

Query
```mysql
Insert INTO pelanggan
Values (1, "nafan","nabil",'0898xxx);
```

1 angka tanpa kutip
abcd string karakter menggunakan kutip 1 atau 2
## Insert >1 data
### Contoh
```mysql
INSERT INTO Pelanggan
Values (2, "FGHI","IHGF",'08x'),
		(3, "Jordan","Null",'08xx'),
		(4, "Nafan","Nabil",'08xxx');
```
## Menyebut Kolom
### Struktur
jika menggunakan insert dengan menyebutkan kolom maka Boleh tidak memperhatikan urut kolom pada tabel / bahkan menghilangkan kolom yang sifatnya bisa di kosongkan
insert INTO [nama_tabel]
(kolom1,kolom2,kolom3,.....);
Values (nilai1,nilai2,nilai3,....);
```mysql
Contoh
INSERT INTO Pelanggan
(nama_depan.id) Values
("STUVW", 5);
```

# Select From
Analisis
Perintah SQL "SELECT * FROM Pelanggan" digunakan untuk mengambil (membaca) data dari tabel "Pelanggan" dalam basis data. Di sini, tanda bintang (*) menunjukkan bahwa kita ingin mengambil semua kolom (atribut) dari setiap baris (record) dalam tabel "Pelanggan". Analisis dari perintah SELECT ini

Query:
```mysql
Select *FROM pelanggan;
```
### Hasil
![[Pasted image 20240427020839.png]]

kesimpulan:
Perintah SQL `SELECT * FROM Pelanggan` dalam MySQL digunakan untuk mengambil semua data yang tersimpan dalam tabel "Pelanggan". Mari kita uraikan:
- `SELECT`: Ini adalah kata kunci yang digunakan untuk memilih data dari database.
- `*`: Ini adalah wildcard yang digunakan untuk menunjukkan bahwa kita ingin memilih semua kolom dalam tabel yang disebutkan.
- `FROM Pelanggan`: Ini menunjukkan tabel dari mana kita ingin mengambil data, dalam hal ini, tabel bernama "Pelanggan".
## Data Kolom tertentu
### Struktur 
### Contoh
```mysql
Select nama_depan From pelanggan;
```

```mysql
Select [nama_kolom1],[nama_kolom2]
		[nama_kolom_n]
From [nama_tabel],
```
## Klausa WHERE
### Struktur
```mysql
SElect [nama_kolom/*] From [nama_tabel]
WHERE [Kondisi];
```
### Contoh
```mysql
Select nama_depan From pelanggan
WHERE id=2;
```

[nama_kolom]  [operator]   [nilai]
contoh kondisi id>1  

=,>,>=,
<,<=,!=
<>,dst

## Uptade

Analisis:
Program terdiri dari dua pernyataan SQL yang dijalankan secara berurutan.
Pernyataan pertama adalah UPDATE, yang bertanggung jawab untuk mengubah nomor telepon pelanggan dengan ID tertentu menjadi nomor telepon baru.
Pernyataan kedua adalah SELECT, yang mengambil semua data dari tabel "pelanggan" setelah perubahan dilakukan.
Secara keseluruhan, program ini bertujuan untuk mengubah nomor telepon pelanggan dengan ID 1 menjadi nomor telepon baru, dan kemudian menampilkan semua data dari tabel "pelanggan" setelah perubahan tersebut.

 Query Uptade:
```
Struktur Program = (update pelanggan set no_telp="08193412451854" where id_pelanggan=1;)
Lalu Ketik
select * From pelanggan;
```

 Hasil:
![[Pasted image 20240427021747.png]]

## DELETE
Analisis:
Perintah "DELETE FROM pelanggan WHERE id_pelanggan = 2;" digunakan untuk menghapus baris atau catatan dari tabel "pelanggan" di mana nilai kolom "id_pelanggan" sama dengan 2.

Query;
```mysql
Delete From pelanggan where id_pelanggan=2;
```

 Hasil
![[Pasted image 20240213024920.png]]

Kesimpulan:
Kesimpulan dari perintah SQL "DELETE FROM pelanggan WHERE id_pelanggan=2;" adalah sebagai berikut:
1. **Tujuan**: Perintah ini bertujuan untuk menghapus baris atau entri dari tabel "pelanggan" di mana nilai kolom "id_pelanggan" sama dengan 2.
2. **Operasi Penghapusan**: Dengan menjalankan perintah ini, baris yang memenuhi kondisi yang ditentukan (id_pelanggan = 2) akan dihapus dari tabel "pelanggan".
3. **Efek Penghapusan**: Penghapusan ini permanen dan akan menghapus data pelanggan yang memiliki ID pelanggan tertentu (2) dari tabel. Data yang dihapus tidak dapat dikembalikan, kecuali jika ada langkah-langkah pemulihan atau cadangan yang dilakukan sebelumnya.
4. **Kondisi Penghapusan**: Penghapusan hanya akan dilakukan pada baris yang memenuhi kondisi yang ditentukan, yaitu ketika nilai kolom "id_pelanggan" sama dengan 2.
5. **Pentingnya Kondisi WHERE**: Kondisi WHERE ("WHERE id_pelanggan=2") penting karena tanpa kondisi tersebut, semua baris dalam tabel "pelanggan" akan dihapus, bukan hanya yang memiliki ID pelanggan 2. Penggunaan kondisi WHERE memastikan bahwa penghapusan dilakukan secara selektif sesuai dengan kriteria yang ditentukan.
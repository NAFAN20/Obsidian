Setelah mempelajari select di materi sebelumnya sekarang kita akan masuk ke dalam materi select lanjutan, fungsi dari select select ini ialah untuk mendapatkan hasil yang lebih spesifik dan lebih luas, sekarang kita akan mempelajari 7 select lanjutan **(AND ,OR ,BETWEEN-AND ,NOT BETWEEN ,<= ,>= ,<> ATAU !=)** Untuk penjelasan lebih lanjutnya ialah seperti berikut :

> [!info]- Isi Table yang akan digunakan :


## AND

untuk **AND** ini akan mengambil "data 1" _dan_ "data 2", contoh kodenya adalah seperti berikut :

```sql
SELECT id_guru,nama_depan FROM tabel_guru WHERE id_guru="3" AND na="Rusdyansyar";
```

Dan hasilnya akan seperti berikut : 
![gambar](Asset/Asset15BD.png)



## OR

Untuk **OR** ini akan mengambil "data 1" _atau_ "data 2", contoh kodenya ialah seperti berikut :

```sql
SELECT warna,pemilik FROM data_mobil WHERE warna="Hitam" OR pemilik="ibrahim";
```

Dan hasilnya akan seperti berikut : 

![gambar](Asset/Asset16BD.png)
## BETWEEN-AND
Untuk **BETWEEN-AND** ini akan mengambil antara "data 1" _sampai_ "data 2" dibantu dengan **AND**, contoh kodenya ialah seperti berikut :

```sql
SELECT * FROM tabel_guru WHERE tanggal_lahir BETWEEN 1982-06-29 AND 2000-09-21;
```

Dan hasilnya akan seperti berikut : 
![gambar](Asset/Asset17BD.png)
## NOT BETWEEN
Untuk **NOT BETWEEN** ini akan mengambil "data" yang _bukan antara_ "data 1" _dan_ "data 2", contoh kodenya ialah seperti berikut :

```sql
SELECT * FROM data_mobil WHERE harga_rental NOT BETWEEN 100000 AND 200000;
```

Dan hasilnya akan seperti berikut : 
![gambar](Asset/Asset18BD.png)
## <=
Untuk **<=** ini akan mengambil "data" lebih kecil atau sama dengan "nilai data", contoh kodenya ialah seperti berikut :

```sql
MariaDB [rental_nafan]> SELECT * FROM data_mobil WHERE harga_rental <= 50000;
```

Dan hasilnya akan seperti berikut : 
![gambar](Asset/Asset19BD.png)
## >=
Untuk **>=** ini akan mengambil "data" lebih besar atau sama dengan "nilai data", contoh kodenya ialah seperti berikut :

```sql
MariaDB [rental_nafan]> SELECT * FROM data_mobil WHERE harga_rental >= 50000;
```

Dan hasilnya akan seperti berikut : 
![gambar](Asset/Asset20BD.png)

## <> atau !=
Untuk **<> atau !=** ini akan mengambil "data" yang tidak sama dengan "nilai data", contoh kodenya ialah seperti berikut :

```sql
MariaDB [rental_nafan]> SELECT * FROM data_mobil WHERE harga_rental <> 50000;
```

Dan hasilnya akan seperti berikut : 
![gambar](Asset/Asset21BD.png)
## Tantangan

Untuk tantangan saya akan mengambil nama pemilik "Ibrahim" dengan cara memanggilnya dengan syarat nomor pelatnya yaitu "DD 2440 AX" lalu hasilnya akan seperti berikut : 
![gambar](Asset/Asset33BD.png)


> [!info]- Analisis
> 
> > "AND" : Mengambil data 1 **dan** data 2. "OR" : Mengambil data antara data 1 **atau** data 2. "BETWEEN-AND" : Mengambil data **antara** data 1 **sampai** data 2. "NOT BETWEEN" : Mengambil data yang tidak **antara** data 1 **sampai** data 2. "<=" : Mengambil data yang lebih kecil atau sama dengan nilai data. ">=" : Mengambil data yang lebih besar atau sama dengan nilai data. "<> atau !=" : Mengambil data yang **tidak** sama dengan nilai data.

Kesimpulan : Select ini memiliki cakupan yang luas dan bervariasi semunya juga memiliki kelebihan dan keunikan masing masing sehingga dapat menampilkan hasil sebuah nilai yang di inginkan, keberagaman select ini mulai dari AND ,OR ,BETWEEN-AND ,NOT BETWEEN ,<= ,>= ,<> ATAU !=.


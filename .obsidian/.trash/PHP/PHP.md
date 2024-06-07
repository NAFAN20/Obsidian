---
_filters: []
_contexts: []
_links: []
_sort:
  field: rank
  asc: false
  group: false
---
# Web Dinamis

Web dinamis adalah jenis situs web yang mampu menghasilkan konten secara dinamis atau berubah sesuai dengan interaksi pengguna, data yang dimasukkan, atau faktor-faktor lainnya. Berbeda dengan situs web statis yang memiliki konten yang tetap dan tidak berubah tanpa interaksi pengguna, situs web dinamis dapat menghasilkan halaman web yang unik untuk setiap pengguna berdasarkan permintaan atau input yang diberikan.

# PHP

PHP adalah bahasa pemrograman yang sering digunakan untuk mengembangkan aplikasi web dinamis. Singkatan dari "Hypertext Preprocessor", PHP berfungsi sebagai skrip sisi server yang dieksekusi di server web untuk menghasilkan konten dinamis. PHP berinteraksi dengan basis data, mengolah formulir, menghasilkan halaman web, dan melakukan banyak tugas lainnya untuk menciptakan pengalaman pengguna yang dinamis di situs web. Dengan bantuan PHP, pengembang dapat membuat situs web yang menanggapi input pengguna dan menyediakan konten yang dipersonalisasi sesuai kebutuhan.

## Struktur Dasar PHP

```PHP

<?

  

$variable = "value";

echo "menampilkan text dan variable dari $variable";

  

```

```output

menampilkan text dan variable value

```

# Program Pertama PHP (Localhost)

Langkah - Langkah Menghubungkan Apache dengan Text Editor()

1. BukaXAMPP app

2. Start Apache in XAMPP

3. Buka Fila Manager

4. Buka Drive C

5. Buka File XAMPP

6. Buka htdocs

7. Create New Folder(Folder_name)

8. Buka Text Editor app

9. Buka Folder_name

10. Add New File PHP in text editor(File.php)S

11. Done

# Echo

- Adalah perintah dalam bahasa pemrograman PHP yang digunakan untuk menampilkan teks atau variabel ke dalam halaman web. Ini memungkinkan pengembang untuk menghasilkan output langsung ke browser pengguna. Misalnya, jika Anda ingin menampilkan teks "Hello, World!" di halaman web menggunakan PHP, Anda dapat melakukannya dengan perintah echo:

**Contoh**

```php

<?

//kutip dua

echo "Hello World";

  

//Kutip satu

echo 'Hello World';

?>

```

## Penjelasan Kutip 1 & 2

`''` hanya membaca sebuah string, variabel dan string dipisahkan oleh tanda titik`.`

`""` *kutip dua* bisa membaca nilai dari variabel

  

# Comentar

- Komentar digunakan dalam kode untuk memberikan penjelasan atau dokumentasi bagi pengembang atau orang lain yang membaca kode. Komentar tidak akan dieksekusi oleh server web dan hanya ada untuk tujuan dokumentasi. Dalam PHP, ada dua jenis komentar: komentar satu baris dan komentar multi-baris.

**Contoh**

```php

// Ini adalah komentar satu baris dalam PHP

  

/*

Ini adalah komentar

multi-baris dalam PHP

*/

```

# Variabel

 **Variabel**: Variabel adalah simbol yang digunakan untuk menyimpan nilai yang dapat berubah selama jalannya program. Dalam PHP, variabel dinyatakan dengan awalan dolar ($) diikuti dengan nama variabel,

- Variabel adalah tempat penyimpanan untuk nilai-nilai dalam sebuah program.

- Setiap variabel memiliki nama yang unik yang digunakan untuk mengidentifikasinya.

- Variabel dapat menyimpan berbagai jenis data seperti angka, teks, boolean, array, dan lainnya.

```php

$nama = "Rahmat";

$umur = 18;

```

Variabel di atas menyimpan nama "Rahmat" dan umur 18. Nilai variabel ini dapat diubah selama jalannya program.

# Constanta

**Konstanta**: Konstanta adalah nilai yang tetap dan tidak dapat diubah selama jalannya program. Mereka berguna untuk menyimpan nilai yang tidak boleh berubah, seperti nilai pi (π) atau nilai-nilai pengaturan yang tetap. Dalam PHP, konstanta didefinisikan menggunakan fungsi define().

- Konstanta adalah nilai yang tetap dan tidak berubah selama jalannya program.

- Nilai konstanta didefinisikan sekali dan tidak dapat diubah kembali.

- Biasanya digunakan untuk menyimpan nilai-nilai seperti konstanta matematis atau pengaturan yang tetap.

```php

define("PI", 3.14);

echo PI;

```

Dalam contoh di atas, kita mendefinisikan konstanta PI dengan nilai 3.14, kemudian menampilkannya.

# Operator

**Operator**: Operator digunakan untuk melakukan operasi pada variabel dan nilai. Ada berbagai jenis operator dalam pemrograman seperti operator aritmatika, operator perbandingan, dan operator logika. Beberapa operator dasar dalam PHP meliputi:

## Operator Aritmatika

### Pemjumlahan

- **Penjelasan:**

    Penjumlahan (+): Digunakan untuk menambahkan dua nilai bersama-sama

```php

$nilai1 = 10;

$nilai2 = 5;

  

$penjumlahan = $nilai1 + $nilai2;

echo "Penjumlahan: " . $penjumlahan . "<br>";

```

```output

Penjumlahan: 15

```

- **Analisis**

    Penjumlahan (+):

    - Operator ini digunakan untuk menambahkan dua nilai bersama-sama.

    - Contoh: `$penjumlahan = $nilai1 + $nilai2;`

    - Hasilnya adalah penjumlahan dari nilai `$nilai1` dan `$nilai2`.

- **Kesimpulan**

    - Kesimpulannya, dengan operator ini, kita dapat menambahkan nilai-nilai numerik dalam PHP dengan mudah.

___

### Pengurangan

- **Penjelasan:**

    Pengurangan (-): Digunakan untuk mengurangkan nilai kedua dari nilai pertama.

```php

$nilai1 = 10;

$nilai2 = 5;

  

$pengurangan = $nilai1 - $nilai2;

echo "Pengurangan: " . $pengurangan . "<br>";

```

```output

Pengurangan: 5

```

- **Analisis**

    Pengurangan (-):

    - Operator ini digunakan untuk mengurangkan nilai kedua dari nilai pertama.

    - Contoh: `$pengurangan = $nilai1 - $nilai2;`

    - Hasilnya adalah pengurangan dari nilai `$nilai2` dari `$nilai1`.

- **Kesimpulan**

    - Kesimpulannya, penggunaan operator ini memungkinkan kita untuk mengurangkan satu nilai dari yang lain dalam pemrograman PHP.

___

### Perkalian

- **Penjelasan**

    Perkalian (*): Digunakan untuk mengalikan dua nilai bersama-sama.

```php

$nilai1 = 10;

$nilai2 = 5;

$perkalian = $nilai1 * $nilai2;

echo "Perkalian: " . $perkalian . "<br>";

```

```output

Perkalian: 50

```

- **Analisis**

    Perkalian (*):

    - Operator ini digunakan untuk mengalikan dua nilai bersama-sama.

    - Contoh: `$perkalian = $nilai1 * $nilai2;`

    - Hasilnya adalah perkalian dari `$nilai1` dan `$nilai2`.

- **Kesimpulan**

    - Kesimpulannya, dengan operator ini, kita dapat melakukan perkalian nilai-nilai numerik dalam PHP untuk mendapatkan hasil perkalian.

___

### Pembagian

- Penjelasan

    Pembagian (/): Digunakan untuk membagi nilai pertama dengan nilai kedua.

```php

$nilai1 = 10;

$nilai2 = 5;

  

$pembagian = $nilai1 / $nilai2;

echo "Pembagian: " . $pembagian . "<br>";

```

```output

Pembagian: 2

```

- **Analisis**

    Pembagian (/):

    - Operator ini digunakan untuk membagi nilai pertama dengan nilai kedua.

    - Contoh: `$pembagian = $nilai1 / $nilai2;`

    - Hasilnya adalah pembagian dari nilai `$nilai1` dengan `$nilai2`.

- **Kesimpulan**

    - Kesimpulannya, operator ini memungkinkan kita untuk membagi nilai-niai numerik dalam PHP dan mendapatkan hasil pembagian.

___

### Modulus

- Penjelasan

    Modulus (%): Digunakan untuk mengembalikan sisa pembagian dari nilai pertama dengan nilai kedua.

```php

$nilai1 = 10;

$nilai2 = 5;

  

$modulus = $nilai1 % $nilai2;

echo "Modulus: " . $modulus . "<br>";

```

```output

Modulus: 0

```

- **Analisis**

    Modulus (%):

    - Operator ini digunakan untuk mengembalikan sisa pembagian dari nilai pertama dengan nilai kedua.

    - Contoh: `$modulus = $nilai1 % $nilai2;`

    - Hasilnya adalah sisa pembagian dari `$nilai1` dengan `$nilai2`.

- **Kesimpulan**

    - Kesimpulannya, dengan menggunakan operator modulus, kita dapat menghitung sisa pembagian dari nilai-nilai numerik dalam PHP.

___

## Operator Perbandingan

- **Penjelasan**

    1. Operator Sama dengan (== ):

     Operator ini digunakan untuk membandingkan apakah dua nilai sama.

     Contohnya, `$a == $b` akan menghasilkan true jika nilai variabel `$a` sama dengan nilai variabel `$b`, dan false jika tidak sama.

  

    2. Operator Tidak Sama dengan (!=):

     Operator ini digunakan untuk membandingkan apakah dua nilai tidak sama.

     Contohnya, `$a != $b` akan menghasilkan true jika nilai variabel `$a` tidak sama dengan nilai variabel `$b`, dan false jika sama.

  

    3. Operator Kurang dari (<):

     Operator ini digunakan untuk membandingkan apakah nilai kiri kurang dari nilai kanan.

     Contohnya, `$a < $b` akan menghasilkan true jika nilai variabel `$a` kurang dari nilai variabel `$b`, dan false jika tidak kurang dari.

  

    4. Operator Lebih Besar dari (>):

     Operator ini digunakan untuk membandingkan apakah nilai kiri lebih besar dari nilai kanan.

     Contohnya, `$a > $b` akan menghasilkan true jika nilai variabel `$a` lebih besar dari nilai variabel `$b`, dan false jika tidak lebih besar dari.

  

    5. Operator Kurang dari atau Sama dengan (<=):  

     Operator ini digunakan untuk membandingkan apakah nilai kiri kurang dari atau sama dengan nilai kanan.

     Contohnya, `$a <= $b` akan menghasilkan true jika nilai variabel `$a` kurang dari atau sama dengan nilai variabel `$b`, dan false jika tidak kurang dari atau sama dengan.

  

    6. Operator Lebih Besar dari atau Sama dengan (>=):  

     Operator ini digunakan untuk membandingkan apakah nilai kiri lebih besar dari atau sama dengan nilai kanan.

     Contohnya, `$a >= $b` akan menghasilkan true jika nilai variabel `$a` lebih besar dari atau sama dengan nilai variabel `$b`, dan false jika tidak lebih besar dari atau sama dengan.

- **Kode Program**

```php

<?php

$a = 5;

$b = 10;

  

// Operator sama dengan (==)

if ($a == $b) {

    echo "$a sama dengan $b";

} else {

    echo "$a tidak sama dengan $b";

}

echo "<br>";

  
  

// Operator tidak sama dengan (!=)

if ($a != $b) {

    echo "$a tidak sama dengan $b";

} else {

    echo "$a sama dengan $b";

}

echo "<br>";

  
  

// Operator kurang dari (<)

if ($a < $b) {

    echo "$a kurang dari $b";

} else {

    echo "$a tidak kurang dari $b";

}

echo "<br>";

  
  

// Operator lebih besar dari (>)

if ($a > $b) {

    echo "$a lebih besar dari $b";

} else {

    echo "$a tidak lebih besar dari $b";

}

echo "<br>";

  
  

// Operator kurang dari atau sama dengan (<=)

if ($a <= $b) {

    echo "$a kurang dari atau sama dengan $b";

} else {

    echo "$a tidak kurang dari atau sama dengan $b";

}

echo "<br>";

  
  

// Operator lebih besar dari atau sama dengan (>=)

if ($a >= $b) {

    echo "$a lebih besar dari atau sama dengan $b";

} else {

    echo "$a tidak lebih besar dari atau sama dengan $b";

}

?>

```

```output

5 tidak sama dengan 10

  

5 tidak sama dengan 10

  

5 kurang dari 10

  

5 tidak lebih besar dari 10

  

5 kurang dari atau sama dengan 10

  

5 tidak lebih besar dari atau sama dengan 10

  

```

- **Analisis**

    - Dua variabel `$a` dan `$b` diinisialisasi dengan nilai numerik, masing-masing 5 dan 10.

    - Program kemudian membandingkan `$a` dan `$b` menggunakan berbagai operator perbandingan dan menampilkan pesan berdasarkan hasil perbandingan.

    - Karena `$a` (5) tidak sama dengan `$b` (10), maka pesan "5 tidak sama dengan 10" akan ditampilkan.

    - Karena `$a` (5) kurang dari `$b` (10), maka pesan "5 kurang dari 10" akan ditampilkan.

    - Karena `$a` (5) tidak lebih besar dari `$b` (10), maka pesan "5 tidak lebih besar dari 10" akan ditampilkan.

    - Karena `$a` (5) kurang dari atau sama dengan `$b` (10), maka pesan "5 kurang dari atau sama dengan 10" akan ditampilkan.

    - Karena `$a` (5) tidak lebih besar dari atau sama dengan `$b` (10), maka pesan "5 tidak lebih besar dari atau sama dengan 10" akan ditampilkan.

- **Kesimpulan**

    - Program ini membantu memahami cara kerja operator perbandingan dalam PHP.

    - Operator perbandingan digunakan untuk membandingkan nilai dan mengontrol alur program berdasarkan hasil perbandingan.

    - Program seperti ini bermanfaat dalam logika pemrograman untuk membuat keputusan berdasarkan kondisi tertentu.

## Operator Logika

- **Penjelasan**

    Dalam PHP, operator logika digunakan untuk menggabungkan kondisi logis dan menghasilkan nilai boolean (true atau false) berdasarkan kebenaran kondisi tersebut. Contoh operator:

    1. **AND (&&):** Menghasilkan true jika kedua kondisi benar.

    2. **OR (||):** Menghasilkan true jika salah satu atau kedua kondisi benar.

    3. **NOT (!):** Membalikkan nilai kondisi, true menjadi false, dan sebaliknya.

```php

<?php

$a = 5;

$b = 10;

$c = 15;

  

// Operator logika AND (&&)

if ($a < $b && $b < $c) {

    echo "$a kurang dari $b dan $b kurang dari $c";

} else {

    echo "Kondisi AND tidak terpenuhi";

}

echo "<br>";

  

// Operator logika OR (||)

if ($a > $b || $b > $c) {

    echo "$a lebih besar dari $b atau $b lebih besar dari $c";

} else {

    echo "Kondisi OR tidak terpenuhi";

}

echo "<br>";

  

// Operator logika NOT (!)

if (!($a == $b)) {

    echo "$a tidak sama dengan $b";

} else {

    echo "$a sama dengan $b";

}

?>

  

```

```output

5 kurang dari 10 dan 10 kurang dari 15

  

Kondisi OR tidak terpenuhi

  

5 tidak sama dengan 10

```

- **Anlisis**

    - Kita memiliki tiga variabel `$a`, `$b`, dan `$c` dengan nilai 5, 10, dan 15.

    - Operator logika `AND` digunakan untuk memeriksa apakah `$a` kurang dari `$b` dan `$b` kurang dari `$c`. Jika  keduanya benar, pesan yang sesuai ditampilkan.

    - Operator logika `OR` digunakan untuk memeriksa apakah `$a` lebih besar dari `$b` atau `$b` lebih besar dari `$c`. Jika salah satu atau kedua kondisi benar, pesan yang sesuai ditampilkan.

    - Operator logika `NOT` digunakan untuk membalikkan nilai kondisi `$a` == `$b`. Jika `$a` tidak sama dengan `$b`, pesan yang sesuai ditampilkan.

- **Kesimpulan**

    - Kode ini menggunakan operator logika untuk membuat keputusan berdasarkan kondisi-kondisi yang dievaluasi.

    - Operator logika memungkinkan kita untuk menggabungkan kondisi-kondisi logis dan mengontrol alur program berdasarkan kebenaran kondisi tersebut.

    - Dengan menggunakan operator logika, kita dapat membuat program yang lebih kompleks dengan logika yang bergantung pada kondisi-kondisi tertentu.

# Conditional Statement

## If

**Penjelasan:**

Pernyataan if digunakan untuk menjalankan blok kode jika kondisi yang diberikan benar (true)

**Struktur:**

```php

if (kondisi) {

    // Blok kode yang dijalankan jika kondisi benar

}

```

**Contoh Program:**

```PHP

$nilai = 80;

  

if ($nilai >= 60) {

    echo "Selamat, Anda lulus!";

}

```

**Hasil:**


**Analisis:**

1. Variabel `$nilai` diberikan nilai 80.

2. Pernyataan if digunakan untuk menguji apakah nilai `$nilai` lebih besar atau sama dengan 60.

3. Karena nilai `$nilai` adalah 80 dan memenuhi kondisi `$nilai >= 60`, blok kode di dalam if akan dieksekusi.

4. Blok kode di dalam if hanya berisi perintah untuk mencetak pesan "Selamat, Anda lulus!" menggunakan pernyataan echo.

5. Setelah blok kode di dalam if dieksekusi, program akan berakhir.

**Kesimpulan:**

Jika variabel `$nilai` memiliki nilai 80, maka kondisi `$nilai >= 60` akan benar, sehingga pesan "Selamat, Anda lulus!" akan ditampilkan.

## If-else

**Penjelasan:**

Pernyataan if-else digunakan untuk menjalankan blok kode tertentu jika kondisi benar (true), dan menjalankan blok kode lain jika kondisi salah (false).

**Struktur:**

```php

if (kondisi) {

    // Blok kode yang dijalankan jika kondisi benar

} else {

    // Blok kode yang dijalankan jika kondisi salah

}

```

**Contoh Program:**

```php

$nilai = 50;

  

if ($nilai >= 60) {

    echo "Selamat, Anda lulus!";

} else {

    echo "Maaf, Anda tidak lulus.";

}

```

**Hasil:**

**Analisis:**

1. Variabel `$nilai` diberikan nilai 50.

2. Pernyataan if digunakan untuk menguji apakah nilai `$nilai` lebih besar atau sama dengan 60.

3. Karena nilai `$nilai` adalah 50 dan tidak memenuhi kondisi `$nilai >= 60`, blok kode di dalam if tidak akan dieksekusi.

4. Karena tidak ada blok kode di dalam if yang dieksekusi, program akan melanjutkan ke blok kode di dalam else.

5. Blok kode di dalam else berisi perintah untuk mencetak pesan "Maaf, Anda tidak lulus." menggunakan pernyataan echo.

6. Setelah blok kode di dalam else dieksekusi, program akan berakhir.

**Kwsimpulan:**

Jika variabel `$nilai` memiliki nilai 50, maka kondisi `$nilai >= 60` akan salah, sehingga pesan "Maaf, Anda tidak lulus." akan ditampilkan.

## if-else-if-else

**Penjelasan:**

Pernyataan if-else-if-else digunakan ketika terdapat beberapa kondisi yang harus diuji secara berurutan.

**Dstruktur:**

```php

if (kondisi1) {

    // Blok kode yang dijalankan jika kondisi1 benar

} elseif (kondisi2) {

    // Blok kode yang dijalankan jika kondisi2 benar

} else {

    // Blok kode yang dijalankan jika semua kondisi salah

}

```

**Contoh Program:**

```php

$nilai = 75;

  

if ($nilai >= 80) {

    echo "Selamat, Anda mendapatkan nilai A!";

} elseif ($nilai >= 70) {

    echo "Anda mendapatkan nilai B.";

} elseif ($nilai >= 60) {

    echo "Anda mendapatkan nilai C.";

} else {

    echo "Maaf, Anda tidak lulus.";

}

```

**Hasil:**

**Analisis:**

1. Variabel `$nilai` diberikan nilai 75.

2. Pernyataan if pertama digunakan untuk menguji apakah nilai `$nilai` lebih besar atau sama dengan 80.

3. Karena nilai `$nilai` tidak mencapai 80, maka blok kode di dalam if pertama tidak akan dieksekusi.

4. Pernyataan elseif pertama digunakan untuk menguji apakah nilai `$nilai` lebih besar atau sama dengan 70.

5. Karena nilai `$nilai` adalah 75 dan memenuhi kondisi `$nilai >= 70`, blok kode di dalam elseif pertama akan dieksekusi.

6. Blok kode di dalam elseif pertama mencetak pesan "Anda mendapatkan nilai B." menggunakan pernyataan echo.

7. Setelah blok kode di dalam elseif pertama dieksekusi, program akan keluar dari struktur kondisional dan berakhir.

**Kesimpulan:**

Jika variabel `$nilai` memiliki nilai 75, maka kondisi `$nilai >= 80` akan salah, namun kondisi `$nilai >= 70` akan benar. Oleh karena itu, pesan "Anda mendapatkan nilai B." akan ditampilkan

## Switch Case

Pernyataan switch case digunakan ketika terdapat beberapa pilihan yang harus diuji.

**Struktur:**

```php

switch (ekspresi) {

    case nilai1:

        // Blok kode yang dijalankan jika ekspresi sama dengan nilai1

        break;

    case nilai2:

        // Blok kode yang dijalankan jika ekspresi sama dengan nilai2

        break;

    default:

        // Blok kode yang dijalankan jika tidak ada case yang cocok

        break;

}

```

**Contoh Program:**

```php

$hari = "Senin";

  

switch ($hari) {

    case "Senin":

        echo "Hari ini adalah hari Senin.";

        break;

    case "Selasa":

        echo "Hari ini adalah hari Selasa.";

        break;

    default:

        echo "Hari ini bukan hari Senin atau Selasa.";

        break;

}

```

**Hasil:**


**Analisis:**

1. Variabel `$hari` diberikan nilai "Senin".

2. Pernyataan switch digunakan untuk memeriksa nilai dari variabel `$hari`.

3. Kasus pertama (`case "Senin"`) akan dieksekusi jika nilai `$hari` adalah "Senin".

4. Karena nilai `$hari` adalah "Senin", blok kode di dalam kasus pertama akan dieksekusi.

5. Blok kode di dalam kasus pertama mencetak pesan "Hari ini adalah hari Senin." menggunakan pernyataan echo.

6. Setelah blok kode di dalam kasus pertama selesai dieksekusi, pernyataan break digunakan untuk menghentikan eksekusi struktur switch.

7. Program akan keluar dari struktur switch dan berakhir.

**Kesimpulan:**

ika variabel `$hari` memiliki nilai "Senin", maka case pertama akan cocok, dan pesan "Hari ini adalah hari Senin." akan ditampilkan.

# Array

## 1 Dimensi

**Penjelasan:**

Array satu dimensi adalah kumpulan nilai yang disimpan dalam satu variabel dengan indeks berurutan secara numerik.

**Struktur:**

```php

$array = array(nilai1, nilai2, nilai3, ...);

```

**Contoh Program:**

```php

$buah = array("Anggur", "Jeruk", "Mangga");

echo $buah[0]; // Output: Apel

echo $buah[1]; // Output: Jeruk

echo $buah[2]; // Output: Mangga

```

**Hasil:**


**Analisis:**

1. Baris pertama mendefinisikan variabel `$buah` sebagai array dengan tiga elemen: "Apel", "Jeruk", dan "Mangga".

2. Baris kedua (`echo $buah[0];`) mencetak nilai buah yang berada pada indeks 0, yaitu "Apel".

3. Baris ketiga (`echo $buah[1];`) mencetak nilai buah yang berada pada indeks 1, yaitu "Jeruk".

4. Baris keempat (`echo $buah[2];`) mencetak nilai buah yang berada pada indeks 2, yaitu "Mangga".

**Kesimpulan:**

Program ini menggunakan array satu dimensi untuk menyimpan dan mengakses kumpulan nilai buah. Dengan menggunakan indeks numerik, kita dapat mengakses nilai buah tertentu dalam array. Dalam contoh ini, program mencetak nilai buah "Apel", "Jeruk", dan "Mangga" sesuai dengan indeks yang ditentukan.

## Asosiatif

**Penjelasan:**

Array asosiatif adalah kumpulan nilai yang disimpan dalam satu variabel dengan indeks berupa kunci (key) yang dapat ditentukan sendiri.

**Struktur:**

```php

$array = array(

    "kunci1" => nilai1,

    "kunci2" => nilai2,

    "kunci3" => nilai3,

    ...

);

```

**Contoh Program:**

```php

$mahasiswa = array(

    "nama" => "John Doe",

    "nim" => "123456",

    "jurusan" => "Teknik Informatika"

);

echo $mahasiswa["nama"]; // Output: John Doe

echo $mahasiswa["nim"]; // Output: 123456

echo $mahasiswa["jurusan"]; // Output: Teknik Informatika

```

**Hasil:**

**Analisis:**

1. Baris pertama mendefinisikan variabel `$mahasiswa` sebagai array asosiatif dengan tiga pasangan kunci-nilai: "nama" dengan nilai "John Doe", "nim" dengan nilai "123456", dan "jurusan" dengan nilai "Teknik Informatika".

2. Baris kedua (`echo $mahasiswa["nama"];`) mencetak nilai yang terkait dengan kunci "nama", yaitu "John Doe".

3. Baris ketiga (`echo $mahasiswa["nim"];`) mencetak nilai yang terkait dengan kunci "nim", yaitu "123456".

4. Baris keempat (`echo $mahasiswa["jurusan"];`) mencetak nilai yang terkait dengan kunci "jurusan", yaitu "Teknik Informatika".

**Kesimpulan:**

Program ini menggunakan array asosiatif untuk menyimpan dan mengakses informasi tentang seorang mahasiswa. Dengan menggunakan kunci yang ditentukan sendiri, kita dapat mengakses nilai-nilai yang terkait dengan kunci tersebut dalam array. Dalam contoh ini, program mencetak informasi nama, nim, dan jurusan mahasiswa sesuai dengan kunci yang ditentukan.

## Multidimensi

**Penjelasan:**

Array multidimensi adalah array yang berisi array di dalamnya, sehingga membentuk struktur data berlapis.

**Struktur:**

```php

$array = array(

    array(nilai1, nilai2, nilai3, ...),

    array(nilai4, nilai5, nilai6, ...),

    ...

);

```

**Contoh Program:**

```php

$matriks = array(

    array(1, 2, 3),

    array(4, 5, 6),

    array(7, 8, 9)

);

echo $matriks[0][0]; // Output: 1

echo $matriks[1][1]; // Output: 5

echo $matriks[2][2]; // Output: 9

```

**Hasil:**

**Analisis:**

1. Baris pertama mendefinisikan variabel `$matriks` sebagai array multidimensi yang terdiri dari tiga array dalam array. Setiap array dalam array tersebut merepresentasikan satu baris dalam matriks.

    - Baris pertama matriks: array(1, 2, 3)

    - Baris kedua matriks: array(4, 5, 6)

    - Baris ketiga matriks: array(7, 8, 9)

2. Baris kedua (`echo $matriks[0][0];`) mencetak nilai yang terletak pada baris pertama (indeks 0) dan kolom pertama (indeks 0) dalam matriks. Outputnya adalah 1.

3. Baris ketiga (`echo $matriks[1][1];`) mencetak nilai yang terletak pada baris kedua (indeks 1) dan kolom kedua (indeks 1) dalam matriks. Outputnya adalah 5.

4. Baris keempat (`echo $matriks[2][2];`) mencetak nilai yang terletak pada baris ketiga (indeks 2) dan kolom ketiga (indeks 2) dalam matriks. Outputnya adalah 9.

**Kesimpulan:**

Program ini menggunakan array multidimensi untuk menyimpan dan mengakses matriks angka. Dengan menggunakan indeks berlapis, kita dapat mengakses nilai-nilai yang terletak pada baris dan kolom tertentu dalam matriks. Dalam contoh ini, program mencetak nilai-nilai dalam matriks sesuai dengan indeks yang ditentukan.

# Var Dump

  

# Looping/Perulangan

## For

**Penjelasan:**

Perulangan for digunakan ketika kita mengetahui jumlah iterasi yang akan dilakukan.

**Struktur:**

```php

for (inisialisasi; kondisi; perubahan) {

    // blok kode yang akan diulang

}

```

**Contoh Program:**

```php

for ($i = 1; $i <= 5; $i++) {

    echo $i;

}

```

**Hasil:**

**Analisis:**

- Pada awal perulangan, variabel `$i` diinisialisasi dengan nilai 1.

- Kondisi perulangan adalah `$i <= 5`, yang berarti perulangan akan terus berjalan selama nilai `$i` kurang dari atau sama dengan 5.

- Setiap kali iterasi perulangan dilakukan, blok kode di dalamnya akan dijalankan. Pada contoh ini, blok kode hanya mencetak nilai `$i` menggunakan perintah `echo`.

- Setelah blok kode dijalankan, variabel `$i` akan bertambah satu menggunakan operator penambahan `$i++`.

- Proses ini akan terus berlanjut hingga kondisi perulangan tidak terpenuhi, yaitu saat nilai `$i` lebih dari 5.

- Output dari program ini akan mencetak angka 1 sampai 5 secara berurutan.

**Kesimpulan:**

Program ini akan mencetak angka dari 1 sampai 5. Hal ini dikarenakan perulangan `for` akan mengulangi blok kode di dalamnya selama kondisi `$i <= 5` bernilai `true`. Setiap iterasi, angka `$i` akan ditampilkan menggunakan perintah `echo`.

## While

**Penjelasan:**

Perulangan while digunakan ketika kita ingin melakukan iterasi selama kondisi bernilai true.

**Struktur:**

```php

while (kondisi) {

    // blok kode yang akan diulang

    // perubahan kondisi harus dilakukan di dalam blok kode

}

```

**Contoh Program:**

```php

$i = 1;

while ($i <= 5) {

    echo $i;

    $i++;

}

```

**Hasil:**

**Analisis:**

- Pada awal program, variabel `$i` diinisialisasi dengan nilai 1.

- Kondisi perulangan adalah `$i <= 5`, yang berarti perulangan akan terus berjalan selama nilai `$i` kurang dari atau sama dengan 5.

- Setiap kali iterasi perulangan dilakukan, blok kode di dalamnya akan dijalankan. Pada contoh ini, blok kode mencetak nilai `$i` menggunakan perintah `echo`.

- Setelah blok kode dijalankan, variabel `$i` akan bertambah satu menggunakan operator penambahan `$i++`.

- Proses ini akan terus berlanjut selama kondisi perulangan terpenuhi, yaitu saat nilai `$i` kurang dari atau sama dengan 5.

- Output dari program ini akan mencetak angka 1 sampai 5 secara berurutan.

**Kesimpulan:**

Program ini akan mencetak angka dari 1 sampai 5. Perulangan `while` akan menjalankan blok kode di dalamnya selama kondisi `$i <= 5` bernilai `true`. Setiap iterasi, angka `$i` akan ditampilkan menggunakan perintah `echo`. Variabel `$i` akan terus bertambah satu setiap kali iterasi dengan menggunakan operator penambahan `$i++`.

## Do While

**Penjelasan:**

Perulangan do while mirip dengan perulangan while, namun blok kode akan dijalankan setidaknya satu kali sebelum melakukan pengecekan kondisi.

**Struktur:**

```php

do {

    // blok kode yang akan diulang

    // perubahan kondisi harus dilakukan di dalam blok kode

} while (kondisi);

```

**Contoh Program:**

```php

$i = 1;

do {

    echo $i;

    $i++;

} while ($i <= 5);

```

**Hasil:**


**Analisis:**

- Pada awal program, variabel `$i` diinisialisasi dengan nilai 1.

- Blok kode di dalam perulangan `do-while` akan dijalankan setidaknya satu kali sebelum kondisi perulangan dievaluasi.

- Pada blok kode pertama, nilai `$i` dicetak menggunakan perintah `echo`.

- Setelah blok kode dijalankan, variabel `$i` akan bertambah satu menggunakan operator penambahan `$i++`.

- Setelah itu, kondisi perulangan `$i <= 5` dievaluasi. Jika kondisi tersebut bernilai `true`, maka perulangan akan kembali ke blok kode awal dan dilanjutkan. Jika kondisi bernilai `false`, perulangan akan berhenti dan program akan melanjutkan eksekusi ke instruksi selanjutnya setelah perulangan.

- Proses ini akan terus berlanjut selama kondisi perulangan terpenuhi, yaitu saat nilai `$i` kurang dari atau sama dengan 5.

- Output dari program ini akan mencetak angka 1 sampai 5 secara berurutan.

**Kesimpulan:**

Program ini akan mencetak angka dari 1 sampai 5. Perulangan `do-while` akan menjalankan blok kode di dalamnya setidaknya satu kali sebelum kondisi perulangan dievaluasi. Setiap iterasi, angka `$i` akan ditampilkan menggunakan perintah `echo`. Variabel `$i` akan terus bertambah satu setiap kali iterasi dengan menggunakan operator penambahan `$i++`. Perulangan akan berlanjut selama kondisi `$i <= 5` bernilai `true`.

## Foreach

**Penjelasan:**

Perulangan foreach digunakan khusus untuk mengiterasi elemen-elemen dalam array atau objek.

**Struktur:**

```php

foreach ($array as $nilai) {

    // blok kode yang akan diulang

}

```

**Contoh Program:**

```php

$buah = array("Apel", "Jeruk", "Mangga");

foreach ($buah as $namaBuah) {

    echo $namaBuah;

}

```

**Hasil:**


**Analisis:**

- Pada awal program, terdapat sebuah array `$buah` yang berisi tiga elemen: "Apel", "Jeruk", dan "Mangga".

- Perulangan `foreach` digunakan untuk mengiterasi setiap elemen dalam array `$buah`.

- Pada setiap iterasi, nilai dari elemen saat ini disimpan dalam variabel `$namaBuah`.

- Blok kode di dalam perulangan akan dijalankan untuk setiap elemen dalam array `$buah`. Pada contoh ini, blok kode mencetak nilai `$namaBuah` menggunakan perintah `echo`.

- Setelah iterasi selesai, perulangan akan berlanjut ke elemen berikutnya dalam array hingga semua elemen telah diproses.

- Output dari program ini akan mencetak nilai dari setiap elemen dalam array `$buah`, yaitu "Apel", "Jeruk", dan "Mangga".

**Kesimpulan:**

Program ini akan mencetak nilai dari setiap elemen dalam array `$buah`, yaitu "Apel", "Jeruk", dan "Mangga". Perulangan `foreach` digunakan untuk mengakses dan memproses setiap elemen dalam array tanpa perlu mengelola indeks secara manual. Pada setiap iterasi, nilai elemen saat ini disimpan dalam variabel `$namaBuah`, yang kemudian dicetak menggunakan perintah `echo`.
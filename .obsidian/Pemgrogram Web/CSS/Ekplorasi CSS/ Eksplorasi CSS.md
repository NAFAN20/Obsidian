# Materi overflow
## Perkenalkan Kelompok
**Kelompok Afaiya**
-M Nafan Nafan Nabil.N
-Muh Daud reski jayadi

## Penjelasan Materi
 Kami dari kelompok Afaiya mendapatkan materi eksplorasi css bagian Tailwind dan tujuan dari pembuatan file obsidian ini ialah untuk memberikan hasil dari kerja kelompok kami, adapun isi dari *penjelasan materi* ini akan terbagi menjadi visible,hidden,scroll,auto,inherit Untuk penjelasan lebih jelasnya akan di paparkan di bawah ini.
### Penjelasan Overflow
### Penjelasan Overflow visible
Properti overflow: visible; dalam CSS digunakan untuk menunjukkan bahwa konten yang melebihi batas kotak elemen akan tetap terlihat di luar kotak tersebut, tanpa adanya pemotongan atau penambahan scrollbar.
#### Kode Program HTML Overflow visible
```html

<!DOCTYPE html>

<html>

<head>

    <link rel="stylesheet" href="style.css">

    <title>Overflow Visible</title>

</head>

<body>

    <div class="container">

        <div class="content">

            <!-- Konten yang melebihi ukuran kotak -->

        </div>

    </div>

</body>

</html>
```

#### Kode Program CSS Overflow Visible
```css
.container {

    width: 200px;

    height: 200px;

    overflow: visible;

    border: 1px solid black;

}

  

.content {

    width: 300px;

    height: 300px;

    background-color: lightblue;
```

#### Hasil Overflow Visible

![[Pasted image 20240425203314.png]]

Dalam contoh ini, `.container` memiliki ukuran 200px x 200px dengan overflow yang diatur menjadi visible. Sedangkan `.content` memiliki ukuran 300px x 300px dengan background warna lightblue yang akan terlihat melebihi batas `.container` karena overflow diatur sebagai visible.
#### Kesimpulan Overflow Visible
Overflow visible adalah properti CSS yang mengatur perilaku overflow dari sebuah elemen dengan cara menampilkan konten yang melebihi ukuran yang ditetapkan untuk elemen tersebut di luar batas elemen tersebut. Dengan overflow visible, konten yang melebihi batas ukuran elemen akan ditampilkan di luar elemen tersebut tanpa adanya pemotongan atau penutupan. Ini berarti konten yang melebihi batas akan terlihat di sekitar elemen tersebut dan tidak akan disembunyikan atau terpotong. Overflow visible berguna ketika Anda ingin konten yang melebihi batas elemen tetap terlihat dan dapat diakses oleh pengguna, meskipun hal ini dapat mengganggu tata letak halaman jika tidak dikelola dengan benar.
### Penjelasan Overflow Hidden
Properti overflow: hidden; dalam CSS digunakan untuk menyembunyikan konten yang melebihi batas kotak elemen, tanpa menampilkan scrollbar.
#### Kode Program HTML Overflow Hidden
```html
<!DOCTYPE html>

<html lang="en">

<head>

    <link rel="stylesheet" href="style.css">

    <title>Overflow Hidden</title>

</head>

<body>

    <div class="container">

        <div class="content">

            <!-- Konten yang melebihi ukuran kotak -->

        </div>

    </div>

</body>

</html>

```

#### Kode Program CSS Hidden
```css
.container {

    width: 200px;

    height: 200px;

    overflow: hidden;

    border: 1px solid black;

}

  

.content {

    width: 300px;

    height: 300px;

    background-color: lightblue;

}
```

#### Hasil Overflow Hidden
![[Pasted image 20240425203001.png]]

Dalam contoh ini, elemen `.container` memiliki ukuran 200px x 200px dengan overflow yang diatur menjadi hidden. Sedangkan elemen `.content` memiliki ukuran 300px x 300px dengan konten yang melebihi batas `.container`. Karena overflow diatur menjadi hidden, bagian konten yang melebihi batas `.container` tidak akan terlihat.
#### Kesimpulan Overflow Hidden
Overflow hidden adalah properti CSS yang mengatur perilaku overflow dari sebuah elemen dengan cara menyembunyikan konten yang melebihi ukuran yang ditetapkan untuk elemen tersebut. Dengan overflow hidden, konten yang melebihi batas ukuran elemen akan terpotong dan tidak akan ditampilkan kepada pengguna. Ini berguna untuk menyembunyikan konten yang tidak diinginkan yang mungkin keluar dari batas elemen, dan memungkinkan penggunaan tata letak yang lebih terkontrol dan rapi. Namun, pengguna harus memperhatikan bahwa dengan overflow hidden, bagian konten yang terpotong tidak akan dapat dilihat atau diakses oleh pengguna, yang dapat mempengaruhi pengalaman pengguna jika konten penting terpotong.
### Penjelasan Overflow Scroll
Properti `overflow: scroll;` dalam CSS digunakan untuk menampilkan scrollbar baik secara horizontal maupun vertikal ketika konten melebihi batas kotak elemen.
#### Kode Program HTML Overflow HTML
```html
<!DOCTYPE html>
<html lang="en">
<head>
<title>Overflow Scroll Example</title>
<link rel="stylesheet" href="styles.css">
</head>
<body>

<div class="container">
  <div class="heading">List of Items:</div>
  <div class="content">
    <ul>
      <li>Item 1</li>
      <li>Item 2</li>
      <li>Item 3</li>
      <li>Item 4</li>
      <li>Item 5</li>
      <li>Item 6</li>
      <li>Item 7</li>
      <li>Item 8</li>
      <li>Item 9</li>
      <li>Item 10</li>
      <li>Item 11</li>
      <li>Item 12</li>
      <li>Item 13</li>
      <li>Item 14</li>
      <li>Item 15</li>
      <li>Item 16</li>
      <li>Item 17</li>
      <li>Item 18</li>
      <li>Item 19</li>
      <li>Item 20</li>
    </ul>
  </div>
</div>

</body>
</html>

```

#### Kode Program CSS Overflow Scroll
```css
.container {
  background-color: #f0f0f0;
  width: 300px;
  height: 200px;
  border: 1px solid #ccc;
  overflow: scroll;
  padding: 10px;
}

.heading {
  font-size: 18px;
  font-weight: bold;
  margin-bottom: 10px;
}

.content {
  font-size: 14px;
}
```
#### Hasil Overflow Scroll
![[Pasted image 20240423100309.png]]

Dalam program ini, kita memiliki sebuah div dengan class `.container` yang memiliki ukuran 300px x 200px dan overflow diatur sebagai scroll. Ini berarti jika konten dalam `.container` melebihi ukurannya, scrollbars akan muncul. Isi konten adalah sebuah daftar (unordered list) dengan 20 item.
#### Kesimpulan Overflow scroll
Overflow scroll adalah properti CSS yang mengatur perilaku overflow dari sebuah elemen dengan menampilkan bilah gulir baik secara horizontal maupun vertikal, terlepas dari apakah konten tersebut melebihi ukuran yang ditetapkan untuk elemen tersebut. Dengan overflow scroll, jika konten di dalam elemen melebihi ukurannya, bilah gulir akan muncul, memungkinkan pengguna untuk menggulir konten untuk melihat bagian yang tidak terlihat. Ini memastikan bahwa pengguna tetap dapat mengakses seluruh konten meskipun area tampilan elemen terbatas. Dengan demikian, overflow scroll sangat berguna dalam menangani konten yang berlebihan dan memastikan pengalaman pengguna yang baik dalam navigasi konten.

### Penjelasan Overflow Auto
  
Properti `overflow: auto;` dalam CSS digunakan untuk menampilkan scrollbar hanya jika konten di dalam elemen melebihi ukuran elemen tersebut.

#### Kode Program HTML Overflow Auto
```html
<!DOCTYPE html>

<html lang="en">

<head>

<title>Overflow Auto Example</title>

<link rel="stylesheet" href="style.css">

</head>

<body>

<div class="container">

  <div class="content">

    <!-- Konten yang lebih besar dari area yang ditetapkan -->

    <p>Kelompok Afaiya Kelompok Afaiya Kelompok Afaiya </p>

    <p>Kelompok Afaiya Kelompok Afaiya Kelompok Afaiya</p>

  </div>

</div>

</body>

</html>

```

#### Kode Program CSS Overflow Auto
```css
.container {

    width: 200px;

    height: 200px;

    overflow: hidden;

    border: 1px solid black;

}

  

.content {

    width: 300px;

    height: 300px;

    background-color: lightblue;

}
```
#### Hasil Overflow Auto
![[Pasted image 20240423103117.png]]

Dalam program ini, kita memiliki sebuah div dengan class `.container` yang memiliki ukuran 300px x 200px dan overflow diatur sebagai auto. Ini berarti jika konten dalam `.container` melebihi ukurannya, scrollbars akan muncul. Jika tidak, maka scrollbars tidak akan muncul. Isi konten adalah sebuah daftar (unordered list) .
#### Kesimpulan Overflow Auto
Overflow auto adalah properti CSS yang digunakan untuk mengatur perilaku overflow dari sebuah elemen. Ketika sebuah elemen memiliki konten yang lebih besar dari ukuran yang ditetapkan untuknya, overflow auto memungkinkan konten tersebut untuk di-scroll secara otomatis ketika konten tersebut tidak muat dalam area yang ditetapkan. Dengan overflow auto, pengguna dapat menggulirkan konten yang tidak terlihat untuk melihat keseluruhan konten yang ada di dalam elemen tersebut. Ini sangat berguna untuk mengelola tata letak yang responsif dan memastikan konten tetap dapat diakses bahkan jika ukurannya melebihi area tampilan yang tersedia.
### Penjelasan Overflow inherit
Overflow inherit adalah properti CSS yang menginstruksikan elemen untuk mewarisi perilaku overflow dari elemen induknya. Ini berarti elemen akan mengadopsi perilaku overflow yang sama seperti elemen induknya.
#### Kode Program HTML Overflow inherit
```html
<!DOCTYPE html>

<html lang="en">

<head>

<title>Overflow Inherit Example</title>

<link rel="stylesheet" href="style.css">

</head>

<body>

<div class="parent-container">

  <div class="child-container">

    <!-- Konten yang lebih besar dari area yang ditetapkan -->

    <p>Kelompok Afaiya</p>

    <p>Kelompok Afaiya</p>

    <p>Kelompok Afaiya</p>

    <p>Kelompok Afaiya</p>

    <p>Kelompok Afaiya</p>

  </div>

</div>

</body>

</html>

```

#### Kode Program CSS Overflow Inherit
```css
.parent-container {

    width: 200px; /* Lebar parent container */

    height: 200px; /* Tinggi parent container */

    border: 1px solid #ccc; /* Garis tepi */

    overflow: scroll; /* Overflow scroll pada parent container */

  }

  .child-container {

    width: inherit; /* Mewarisi lebar dari parent container */

    height: inherit; /* Mewarisi tinggi dari parent container */

    border: 1px solid red; /* Garis tepi (untuk tujuan demonstrasi) */

    overflow: inherit; /* Mewarisi perilaku overflow dari parent container */

  }
```
#### Hasil
![[Pasted image 20240423194453.png]]

Dalam contoh ini, `.parent-container` memiliki properti overflow yang diatur menjadi hidden, sedangkan `.child-container` mewarisi nilai overflow dari induknya dengan menggunakan overflow: inherit. Sebagai hasilnya, overflow di `.child-container` akan sama dengan overflow di `.parent-container`, yaitu hidden. Jadi, konten dalam `.child-container` akan terpotong jika melebihi ukuran kotaknya.
#### Kesimpulan Overflow Inherit
Overflow inherit adalah properti CSS yang memungkinkan sebuah elemen untuk mewarisi perilaku overflow dari elemen induknya. Ini berguna ketika Anda ingin agar perilaku overflow dari suatu elemen sama dengan perilaku overflow dari elemen induknya tanpa harus menetapkan secara langsung. Dengan menggunakan overflow inherit, Anda dapat membuat tata letak yang konsisten dan memastikan bahwa perilaku overflow konsisten di seluruh struktur dokumen HTML Anda.

### Implementasi Web Overflow Scroll Dan Overflow Auto
#### Penjelasan
Implementasi web dengan overflow scroll dan overflow auto adalah teknik yang berguna ketika konten di dalam elemen tidak cukup untuk muat di dalamnya. Berikut adalah beberapa analisis dan kesimpulan terkait implementasi tersebut:
**Penggunaan Overflow Scroll**: Overflow scroll memungkinkan pengguna untuk menggulir konten di dalam elemen secara manual, bahkan jika konten tersebut tidak cukup untuk muat di dalamnya. Ini berguna ketika Anda memiliki banyak konten tetapi ruang yang terbatas. Namun, perlu diperhatikan bahwa pengguna harus melakukan interaksi langsung untuk melihat seluruh konten.
**Penggunaan Overflow Auto**: Overflow auto secara otomatis menentukan apakah gulir diperlukan atau tidak. Jika konten melebihi ukuran elemen, maka scrollbar akan muncul dan pengguna dapat menggulirnya. Jika tidak, tidak akan ada scrollbar yang muncul. Ini memberikan pengalaman yang lebih baik karena hanya menampilkan scrollbar saat diperlukan, mengurangi kebingungan pengguna.
**Pertimbangan Desain**: Saat menggunakan overflow scroll atau overflow auto, penting untuk mempertimbangkan desain secara keseluruhan. Warna, transparansi, dan bayangan latar belakang dapat mempengaruhi keterbacaan konten yang digulir. Pastikan konten tetap mudah dibaca dan tidak terlalu tersembunyi oleh efek latar belakang.
**Responsif**: Pastikan bahwa desain Anda responsif, sehingga penggunaan overflow scroll atau auto berfungsi dengan baik di berbagai perangkat dan ukuran layar. Hal ini dapat dicapai dengan menggunakan unit relatif seperti persentase untuk lebar dan tinggi, dan dengan menguji tampilan Anda di berbagai perangkat.
**Performa**: Penting untuk diingat bahwa penggunaan overflow, terutama overflow scroll dengan banyak konten, dapat memengaruhi performa halaman web, terutama pada perangkat dengan spesifikasi rendah. Pastikan untuk menguji performa halaman Anda dan melakukan optimasi jika diperlukan.
#### Kode Program HTML Implementasi Web
```html
<!DOCTYPE html>

<html lang="en">

  <head>

    <meta charset="UTF-8" />

    <meta name="viewport" content="width=device-width, initial-scale=1.0" />

    <title>Overflow Scroll dan Auto dengan Background</title>

    <link rel="stylesheet" href="Implemenasi-E.css" />

  </head>

  < class="body">

    <div class="container">

      <div class="scroll">

        <h2>Overflow Scroll</h2>

        <p>Afaiya Afaiya Afaiya Afaiya</p>

        <p>Afaiya Afaiya Afaiya Afaiya</p>

        <p>Afaiya Afaiya Afaiya Afaiya</p>

        <p>Afaiya Afaiya Afaiya Afaiya</p>

        <p>Afaiya Afaiya Afaiya Afaiya</p>

        <p>Afaiya Afaiya Afaiya Afaiya</p>

        <p>Afaiya Afaiya Afaiya Afaiya</p>

        <p>Afaiya Afaiya Afaiya Afaiya</p>

        <p>Afaiya Afaiya Afaiya Afaiya</p>

        <p>Afaiya Afaiya Afaiya Afaiya</p>

        <p>Afaiya Afaiya Afaiya Afaiya</p>

        <p>Afaiya Afaiya Afaiya Afaiya</p>

        <p>Afaiya Afaiya Afaiya Afaiya</p>

        <p>Afaiya Afaiya Afaiya Afaiya</p>

        <p>Afaiya Afaiya Afaiya Afaiya</p>

      </div>

      <div class="auto" width="50" height="50">

        <h2>Overflow Auto</h2>

        <p>

          Afaiya Afaiya Afaiya Afaiya Afaiya Afaiya Afaiya Afaiya Afaiya Afaiya

          Afaiya Afaiya Afaiya Afaiya Afaiya Afaiya Afaiya Afaiya

        </p>

        <p>Afaiya Afaiya Afaiya Afaiya Afaiya Afaiya Afaiya Afaiya Afaiya</p>

        <p>Afaiya Afaiya Afaiya Afaiya Afaiya Afaiya Afaiya Afaiya Afaiya</p>

        <p>Afaiya Afaiya Afaiya Afaiya Afaiya Afaiya Afaiya Afaiya Afaiya</p>

        <p>Afaiya Afaiya Afaiya Afaiya Afaiya Afaiya Afaiya Afaiya Afaiya</p>

        <p>Afaiya Afaiya Afaiya Afaiya Afaiya Afaiya Afaiya Afaiya Afaiya</p>

        <p>Afaiya Afaiya Afaiya Afaiya Afaiya Afaiya Afaiya Afaiya Afaiya</p>

        <p>Afaiya Afaiya Afaiya Afaiya Afaiya Afaiya Afaiya Afaiya Afaiya</p>

        <p>Afaiya Afaiya Afaiya Afaiya Afaiya Afaiya Afaiya Afaiya Afaiya</p>

        <p>Afaiya Afaiya Afaiya Afaiya Afaiya Afaiya Afaiya Afaiya Afaiya</p>

      </div>

    </div>

    <img src="./assets/smk7.png" alt="SMK Negeri 7 MAKASSAR" class="dark" width="280" height="280"></img>

  </body>

</html>
```
#### Kode Program CSS Implementasi Web
```css
body {

  font-family: Arial, sans-serif;

  margin: 0;

  padding: 0;

  background-image: url('./assets/dark.jpg');

}

  

.container {

  justify-content: space-around;

  align-items: flex-start;

}

  

.scroll, .auto {

  width: 45%;

  max-height: 200px;

  padding: 10px;

  border-radius: 20px;

  overflow-x: auto;

  overflow-y: auto;

  min-width: 300px;

}

  

.scroll {

  background-color: #f0f0f0;

  background-size: cover;

  margin-top: 450px;

  overflow: scroll;

}

  

.auto {

  background-color: white; width: 50px; ;

  background-size: 50px;

  overflow: auto;

  width: 450px;

  float: right;

  margin-top: -500px;

 min-width: 100px;

}

  

.dark{

  width: 400px;

  float: right;

  margin-top: -250px;

}
```
#### Hasil
![[Pasted image 20240428082424.png]]

#### Kesimpulan Implementasi Web 
**Penggunaan Overflow Scroll dan Overflow Auto**: Program ini menggunakan kedua properti overflow, yaitu overflow scroll dan overflow auto. Elemen dengan kelas "scroll" menggunakan overflow scroll, sementara elemen dengan kelas "auto" menggunakan overflow auto.
**Desain Container**: Elemen dengan kelas "container" memiliki aturan CSS untuk menetapkan tata letak kontennya. Dalam hal ini, konten disusun dengan menggunakan justify-content: space-around; dan align-items: flex-start;.
 **Desain Konten Overflow Scroll dan Auto**: Elemen dengan kelas "scroll" dan "auto" memiliki aturan CSS yang menentukan warna latar belakang, ukuran, dan overflow-x serta overflow-y. Overflow-x dan overflow-y diatur sebagai auto pada keduanya, tetapi hanya overflow-x yang seharusnya digunakan pada "scroll".
**Desain Latar Belakang Body**: Latar belakang body diatur menggunakan properti background-image dengan gambar yang diberikan. Hal ini memberikan tampilan latar belakang yang sesuai dengan desain keseluruhan halaman.
 **Desain Gambar Tambahan**: Terdapat gambar tambahan (SMK Negeri 7 MAKASSAR) yang dimasukkan sebagai elemen img. Gambar ini memiliki aturan CSS untuk ukuran dan penempatan tertentu dalam halaman.
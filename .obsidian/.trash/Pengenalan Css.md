---
_filters: []
_contexts: []
_links: []
_sort:
  field: rank
  asc: false
  group: false
---
# SINTAKSIS

Intrnal

1. di dalam tag style


selector : bagian mana yang ingin di modifikasi

property : bentuk modifikasi apa

value : value nilai modifikasinya

  

~~~html

<!DOCTYPE html>

  
  

<html lang="en">

  

<head>

  

    <title>MATERI CSS</title>

  

    <style>

  

        p,h1 {

  

            color: red;

  

        }

  

        h1 {

  

            color: orange;

  

        }

  

    </style>

  

</head>

  

<body>

  

    <h1>ini judul</h1>

  

    <p>ini kita coba</p>

  

</body>

  

</html>

~~~

  

hasil :

![](AsetCSS/1.png]]

  

# PEMANGGILAN SECARA INLINE CSS

  

1.Invite

Di dalam tag ada style

Langsung di tag di inginkan

Lebih di prioritaskan

  

contoh:

~~~ css

<p style="font-size: 50px; color: blue";</p>

~~~

contoh program:

~~~html

<!DOCTYPE html>

  

<html lang="en">

  

    <head>

  

        <title>materi CSS</title>

  

    </head>

  

    <body>

  

        <h1>judul</h1>

        <p>iqbaaalaaaaal</p>

        <p style="font-size: 50px; color: blue;">NafanGanteng</p>

  

    </body>

  

</html>

~~~

hasil :

  

![[Screenshot (27) 1.png]]

  

# PEMANGGILAN SECARA EXTERNAL CSS

Pemanggilan CSS secara eksternal mengacu pada praktik menyimpan kode CSS dalam file terpisah dan memanggilnya ke dalam halaman HTML menggunakan tag `<link>`. Ini memungkinkan Anda untuk memisahkan gaya dari struktur dan konten halaman, membuat kode lebih terorganisir dan lebih mudah dipelihara.

 contoh :

 ~~~html

 <!DOCTYPE html>

  

<html>

  

  

<head>

  

    <link rel="stylesheet" type="text/css" href="index14.css">

  

</head>

  

  

<body>

  

    <div class="container">

  

        <h1>Halo, Bumi!</h1>

  

        <p>Ini adalah contoh pemanggilan CSS eksternal.</p>

  

    </div>

  

</body>

  

  

</html>

~~~

  

contoh :

~~~css

body {

  

    background-color: #f2f2f2;

  

    font-family: Arial, sans-serif;

  

  }

  

  h1 {

  

    color: #333333;

  

  }

 ~~~

 hasil :

 

# COLOR

Pada CSS, warna dapat ditentukan menggunakan beberapa metode. Berikut adalah beberapa cara umum untuk menentukan warna menggunakan properti "color":

  

1. Nama Warna: Anda dapat menggunakan nama warna bawaan dalam CSS seperti "red" (merah), "blue" (biru), "green" (hijau), dan lain-lain. Contoh penggunaan:

    contoh :

    ~~~css

    color: red;

    ~~~    

1. Nilai Hexadecimal: Anda dapat menggunakan kode hexadecimal untuk menentukan warna. Kode hexadecimal terdiri dari enam digit, yang mewakili kombinasi merah, hijau, dan biru (RGB). Contoh penggunaan:

    contoh  :

    ~~~css

    color: #FF0000; /* merah */

    color: #00FF00; /* hijau */

    color: #0000FF; /* biru */

    ~~~

2. Nilai RGB: Anda dapat menggunakan nilai RGB untuk menentukan warna. Nilai RGB terdiri dari tiga angka yang mewakili intensitas merah, hijau, dan biru dalam rentang 0 hingga 255. Contoh penggunaan:

    contoh :

    ~~~css

    color: rgb(255, 0, 0); /* merah */

    color: rgb(0, 255, 0); /* hijau */

    color: rgb(0, 0, 255); /* biru */

    ~~~

3. Nilai RGBA: Selain nilai RGB, Anda dapat menggunakan nilai RGBA yang juga mencakup komponen alpha (transparansi). Nilai alpha berkisar antara 0 hingga 1, di mana 0 adalah transparan dan 1 adalah opak. Contoh penggunaan:

    contoh :

    ~~~css

    color: rgba(255, 0, 0, 0.5); /* merah dengan transparansi 50% */

    ~~~

4. Nilai HSL dan HSLA: Anda juga dapat menggunakan nilai HSL (Hue, Saturation, Lightness) atau HSLA (HSL dengan komponen alpha) untuk menentukan warna. Nilai Hue berkisar antara 0 hingga 360, Saturation dan Lightness berkisar antara 0 hingga 100, dan nilai alpha berkisar antara 0 hingga 1. Contoh penggunaan:

    contoh :

    ~~~css

    color: hsl(0, 100%, 50%); /* merah */

    color: hsla(120, 100%, 50%, 0.5); /* hijau dengan transparansi 50% */

    ~~~

Itulah beberapa metode yang dapat digunakan untuk menentukan warna teks menggunakan properti "color" dalam CSS. Anda dapat memilih metode yang paling sesuai dengan kebutuhan Anda.

- Background - color

   background color berguna untuk memberikan style warna pada latar belakang teks yang sudah ada di tentukan misalnya kita ingin latar memberi warna ungu terang maka kita menggunakan code bluevilolet.

hasil :

![[Pasted image 20231212145337.png]]

  

1.EXTERNAL

- File html dan css di pisah

- file html panggil file css dengan link

- file harus satu folder

  

Program Css:

``` css

h1 {

  Background-color: blue;

}

```

contoh program HTML :

~~~ html

<!DOCTYPE html>

  

<html lang="en">

  

    <head>

  

        <title>materi CSS</title>

        <link rel="stylesheet" Href="dex.css">

  

    </head>

  

    <body>

  

        <h1>judul</h1>

        <p>iqbalaaaal</p>

  

    </body>

  

</html>

~~~

Hasil:

  

![[Screenshot (26).png]]

  

# FONT

  

>[!Penjelasan]

>Digunakan untuk mengatur berbagai aspek teks, termasuk jenis huruf, ukuran huruf, gaya huruf, ketebalan huruf, warna huruf, warna teks, dan sebagainya. Property "font" ini memberikan kontrol atas penampilan teks di elemen HTML.

  

*Berikut adalah beberapa property font umum di CSS*:

## font family

 `Font-family`: Menentukan jenis huruf atau jenis font yang akan digunakan. Anda dapat menyediakan daftar font alternatif untuk memberikan opsi jika font utama tidak tersedia.

### contoh:

~~~CSS

P {font-family: "Arial";}

~~~

hasil :

![[Pasted image 20231212184631.png]]

## font size

`Font-size`: Menentukan ukuran huruf teks. Anda dapat menggunakan nilai dengan piksel, em, atau unit ukuran lainnya.

### contoh:

~~~CSS

P{ font-size: 16px; }

~~~

hasil :

![[Pasted image 20231212184506.png]]

## font weight

`Font-weight`: mengatur ketebalan huruf. Nilai umum termasuk normal, bold, atau menggunakan nilai numerik seperti 400 atau 700.

  

## contoh :

~~~css

  font-weight: bold;

  ~~~

hasil :

![[Pasted image 20231212185034.png]]

  

# BACKGROUND

- Background - color

   background color berguna untuk memberikan style warna pada latar belakang teks yang sudah ada di tentukan misalnya kita ingin latar memberi warna ungu terang maka kita menggunakan code bluevilolet.

### contoh:

  

1. background-color: Mengatur warna latar belakang elemen. Anda dapat menggunakan nama warna, nilai hexadecimal, nilai RGB, atau nilai HSL. Contoh penggunaan:

    ~~~css

    ````

    background-color: red;

    background-color: #00ff00;

    background-color: rgb(255, 0, 0);

    ~~~

    hasil :

    ![[Pasted image 20231212151351.png]]

2. background-image: Menentukan gambar yang akan digunakan sebagai latar belakang elemen. Anda dapat menggunakan URL gambar atau nilai none jika tidak ada gambar yang digunakan. Contoh penggunaan:

    ~~~css

    background-image: url("gambar.jpg");

    background-image: none;

    ~~~

3. background-repeat: Mengatur pengulangan gambar latar belakang. Nilai yang umum digunakan adalah repeat (mengulang secara horizontal dan vertikal), repeat-x (hanya mengulang secara horizontal), repeat-y (hanya mengulang secara vertikal), dan no-repeat (tidak mengulang). Contoh penggunaan:

  ~~~css

    background-repeat: repeat;

    background-repeat: no-repeat;

    ~~~

hasil :

![[Pasted image 20231212153518.png]]

4. background-position: Menentukan posisi gambar latar belakang. Anda dapat menggunakan nilai seperti top, bottom, left, right, center, atau kombinasi dari nilai horizontal dan vertikal dalam piksel atau persentase. Contoh penggunaan:

    ~~~css

    background-position: top left;

    background-position: center;

    background-position: 50% 50%;

    ~~~

    hasil :

    ![[Pasted image 20231212153141.png]]

  

5. background-size: Mengatur ukuran gambar latar belakang. Anda dapat menggunakan nilai seperti auto (ukuran asli gambar), cover (memastikan gambar tercakup sepenuhnya dalam elemen), contain (memastikan gambar tetap proporsional dalam elemen), atau nilai ukuran dalam piksel atau persentase. Contoh penggunaan:

~~~css

    background-size: cover;

    background-size: contain;

    background-size: 100px 200px;

~~~

hasil :

![[Pasted image 20231212153357.png]]

  

Ini hanya beberapa sub-properti yang umum digunakan dalam properti "background". Dalam praktiknya, Anda dapat menggunakan kombinasi dari sub-properti ini sesuai dengan kebutuhan Anda untuk mencapai tampilan latar belakang yang diinginkan pada elemen HTML.

  

## *kesimpulan* :

  

Berikut adalah kesimpulan mengenai properti "background" dalam CSS:

  

- Properti "background-color" digunakan untuk mengatur warna latar belakang elemen.

- Properti "background-image" digunakan untuk menentukan gambar yang akan digunakan sebagai latar belakang elemen.

- Properti "background-repeat" digunakan untuk mengatur pengulangan gambar latar belakang.

- Properti "background-position" digunakan untuk menentukan posisi gambar latar belakang.

- Properti "background-size" digunakan untuk mengatur ukuran gambar latar belakang.

  

Anda dapat menggunakan kombinasi dari sub-properti ini sesuai dengan kebutuhan Anda untuk mencapai tampilan latar belakang yang diinginkan pada elemen HTML.

  

Selain itu, penting juga untuk memahami bahwa properti "background" dapat memiliki nilai default, yang biasanya adalah "transparent" untuk "background-color" dan "none" untuk "background-image". Anda dapat menggabungkan atau mengabaikan sub-properti sesuai kebutuhan desain Anda.

  

Dengan menggunakan properti "background" dengan bijak, Anda dapat menciptakan tampilan visual yang menarik dan meningkatkan pengalaman pengguna pada halaman web Anda.

  
  

# SELECTOR CSS

~~~css

#tesid {

   Font-size:50px;

}

<p id="tesid">

    Paragraf 1

</p>

~~~

  

*analisis*

-  Dalam kode CSS, kita menggunakan selector ID (`#tesid`) untuk memilih elemen dengan atribut `id="tesid"`. Selector ID merupakan selektor yang paling spesifik karena ID harus unik di dalam satu halaman HTML.

-  Properti `font-size` digunakan untuk mengatur ukuran font pada elemen yang memiliki ID `tesid`.

- Nilai `50px` pada properti `font-size` menentukan ukuran font sebesar 50 piksel.

  

Dalam kode HTML, kita menggunakan elemen `<p>` (paragraf) dengan atribut `id="tesid"`. Elemen ini dipilih oleh selector CSS dengan ID yang sama.

  

Dengan kombinasi kode CSS dan HTML tersebut, paragraf yang memiliki ID `tesid` akan memiliki ukuran font sebesar 50 piksel. Hal ini akan menghasilkan tampilan paragraf dengan teks yang lebih besar dibandingkan dengan ukuran font defaultnya.

  

Perlu diingat bahwa analisis ini didasarkan pada informasi yang diberikan, dan implementasi akhirnya akan bergantung pada konteks dan pengaturan CSS yang lebih luas.

  

*kesimpulan*

Berikut adalah kesimpulan mengenai selector dalam CSS:

  

-  Selector CSS digunakan untuk memilih elemen atau kelompok elemen dalam halaman HTML yang ingin Anda gayakan (styling).

-  Selector dasar adalah selector elemen, yang memilih elemen berdasarkan nama tagnya, seperti `p` untuk memilih semua elemen paragraf.

-  Anda juga dapat menggunakan selector kelas (class selector) dengan menambahkan tanda titik (`.`) diikuti dengan nama kelas, seperti `.kelas` untuk memilih elemen yang memiliki kelas "kelas".

-  Selector ID (id selector) digunakan untuk memilih elemen berdasarkan atribut ID yang unik. Anda dapat menggunakan tanda pagar (`#`) diikuti dengan nama ID, seperti `#id` untuk memilih elemen dengan ID "id".

-  Selector atribut memungkinkan Anda memilih elemen berdasarkan atribut dan nilainya. Misalnya, `[type="text"]` akan memilih elemen input dengan atribut tipe "text".

## Pengertian Value css

  

Value CSS adalah nilai dari property. Misalkan untuk property background - color yang digunakan untuk mengubah warna latar belakang dari sebuah selector, value atau nilainya latar belakang dari sebuah selector, value atau nilainya dapat berupa read, blue, black, atau white.

  

contoh :

~~~css

backgroud-color : red;

~~~

  

*analisis* :

-  Properti "background-color" digunakan untuk mengatur warna latar belakang elemen HTML.

-  Nilai "red" yang digunakan dalam contoh ini adalah nama warna merah dalam CSS.

-  Dengan properti ini, latar belakang elemen akan diisi dengan warna merah.

-  Warna merah dapat memiliki berbagai makna dan konotasi, seperti keberanian, gairah, atau peringatan, tergantung pada konteks penggunaannya.

-  Nilai "red" juga dapat diganti dengan nilai lain yang valid, seperti nilai hexadecimal "#FF0000" atau nilai RGB "rgb(255, 0, 0)", yang akan menghasilkan warna merah yang sama.

  

*kesimpulan* :

-  Nilai dalam CSS digunakan untuk memberikan informasi spesifik kepada properti CSS tentang bagaimana elemen HTML harus ditampilkan atau diposisikan.

-  Nilai dalam CSS dapat berupa angka, teks, atau kombinasi keduanya, tergantung pada properti yang digunakan.

-  Beberapa contoh nilai dalam CSS meliputi warna, ukuran font, ukuran dan posisi latar belakang, lebar dan tinggi elemen, dan tampilan elemen.

-  Nilai warna dapat dinyatakan dalam nama warna, nilai hexadecimal, atau nilai RGB.

  

# BOX MODEL

  

~~~HTML

<html>

  

    <head>

  

<title>home</title>

  

        <link rel="stylesheet" href="bal.css">

  

    </head>

  

    <body>

  

        <p class="text">

  

        klik untuk mencintai denpul

  

        </p>

  

        <button class="btn">❤️ENTER</button>

  

    </body>

  

</html>

~~~

hasil :

![[Screenshot (32).png]]

  

Tampilan css

~~~css

.btn{

  

    background-color:aqua;

  

    color: white;

  

    border: none;

  

    width: 300px;

  

    height: 200px;

  

    font-size: 50px;

  

    font-family: 'segoe UI';

  

    font-weight: bold;

  

    border-radius: 40px;

  

}

  

  

.text{

  

    font-size: 50px;

  

    font-style: italic;

  

    font-family: 'calibri';

  

    color:antiquewhite;

  

}

  

body{

  

    background-image: url(me.jpg);

  

    text{

  

        background-color: blueviolet;

  

    }

~~~

  

## Analisis :

Analisis dari kode CSS yang diberikan adalah sebagai berikut:

  

1. Kode CSS dimulai dengan selector `.btn`, yang akan memilih semua elemen dengan kelas "btn".

2. Properti `background-color: aqua;` mengatur warna latar belakang elemen dengan kelas "btn" menjadi "aqua".

3. Properti `color: white;` mengatur warna teks pada elemen dengan kelas "btn" menjadi "putih".

4. Properti `border: none;` menghilangkan border pada elemen dengan kelas "btn".

5. Properti `width: 300px;` dan `height: 200px;` mengatur lebar dan tinggi elemen dengan kelas "btn" menjadi 300 piksel dan 200 piksel.

6. Properti `font-size: 50px;` mengatur ukuran font pada elemen dengan kelas "btn" menjadi 50 piksel.

7. Properti `font-family: 'segoe UI';` mengatur jenis font pada elemen dengan kelas "btn" menjadi "segoe UI".

8. Properti `font-weight: bold;` mengatur ketebalan font pada elemen dengan kelas "btn" menjadi tebal.

9. Properti `border-radius: 40px;` mengatur radius sudut elemen dengan kelas "btn" menjadi 40 piksel, memberikan efek sudut melengkung.

  

Selanjutnya, kode CSS melanjutkan dengan selector `.text`, yang akan memilih semua elemen dengan kelas "text".

  

1. Properti `font-size: 50px;` mengatur ukuran font pada elemen dengan kelas "text" menjadi 50 piksel.

2. Properti `font-style: italic;` mengatur gaya font pada elemen dengan kelas "text" menjadi miring (italic).

3. Properti `font-family: 'calibri';` mengatur jenis font pada elemen dengan kelas "text" menjadi "calibri".

4. Properti `color: antiquewhite;` mengatur warna teks pada elemen dengan kelas "text" menjadi "antiquewhite".

  

File css

~~~css

  

body {

  

  

     background-color: rgb(93, 93, 174);

  

    }

  

    .judul {

  

    color:white;

  

    }

  

    .btn {

  

     width: 200px;

  

    height: 50px;

  

    border: none;

  

    border-radius: 10px;

  

    background-color: blue;

  

    color: white;

  

    box-shadow: 0px 5px 15px 5px rgb(65, 65, 211);

  

    }

  

    .img {

  

     width: 350px;

  

     height: 300px;

  

    border-radius: 20px;

  

    }

  

    .box {

  

    border: 15px white solid;

  

    border-radius: 20px;

  

    padding: 10px 0px 20px 40px;

  

    width: 390px;

  

    box-shadow: 15px 20px 10px 5px black;

  

    margin-top: 90px;

  

    margin-right: 80px;

  

     margin-left: 65px;

  

    color: white;

  

     float: left;

  

    }

  

~~~

  

hasil :

  

![[Screenshot (34).png]]

  
  

> [!faq]- penjelasan border radius

> [body  (background-color: rgb(93, 93, 174); )] untuk memberi background pada halaman web

> [.judul] Nama class. [Color:white] Memberi warna pada konten class judul

> [width] Mengatur lebar konten. [height] Mengatur tinggi konten

> [border] memberi garis tepi pada konten. Tapi, karena di beri [none] maka garis tepi di hilangkan

> [border-radius] menumpulkan garis tepi pada konten

> [background-color] Memberi warna pada bakground konten

> [background-image] Memberi gambar pada halaman web

> [color] Memberi warna pada konten

> [box-shadow] memberi bayangan pada border yang yang di buat

> [box-sizing] Merubah kalkulasi lebar element

> [float: left;] Perintah untuk menyalin konten yang telah di buat ke kanan

> [font-family] Mengatur jenis teks

  
  

> [!faq]- penjelasan margin

> [Margin]

> [Margin] Mengatur jarak yang beda element

> [Margin-top] Mengatur jarak atas yang beda element

> [margin-right] Mengatur jarak atas yang beda element

> [margin-bottom] Mengatur jarak bawa yang beda element

> [matgin-left] Mengatur jarak kiri yang beda element

  
  

> [!faq]- penjelasan padding

> [padding] Mengatur jarak sesama element

> [padding-top] Mengatur jarak atas sesama element

> [padding-right] Mengatur jarak kanan sesama elemet

> [padding-bottom] Mengatur jarak bawa sesama element

> [padding-left] Mengatir jarak kiri sesama element.

# TRANSFORM

~~~css

transform: scale(1.30);

~~~

  

> [!faq]- trasform adalah salah satu yang terpenting yang harus di pahami bagi yang ingin membuat efek animasi dengan css. property ini trasform menerapkan transformasi 2d dan 3d ke suatu elemen. property ini memungkinkan anda memutar, menskalakan, memindahkan, memiringkan, dll.

  

# TRANSITION

~~~css

transition: all 0.3s ease-in;

~~~

  

> [!faq]- transition adalah efek transis yang memungkinkan sebuah elemen secara bertahap berubah dari satu gaya ke gaya lain. fungsi dari efek transisi adalah untuk membuat animasi pada hover, dimana saat kursor kita arahkan pada elemen yang mempunyai fungsi hover maka elemen tersebut akan secara bertahap berubah gaya.

  

file css

~~~css

.btn{

  

    background-color:aqua;

  

    color: white;

  

    border: none;

  

    width: 300px;

  

    height: 200px;

  

    font-size: 50px;

  

    font-family: 'segoe UI';

  

    font-weight: bold;

  

    border-radius: 40px;

  

    cursor: pointer;

  

    transform: rotate3d();

  

}

  

  

.text{

  

    font-size: 50px;

  

    font-style: italic;

  

    font-family: 'calibri';

  

    color:antiquewhite;

  

}

  

body{

  

    background-image: url(me.jpg);

  

    text{

  

        background-color: blueviolet;

  

    }

  

  

.btn:hover{

  

    background-color:blueviolet;

  

    color:aqua;

  

    width: 500px;

  

    transition: all 0.3s ease-in;

  

}

  

  

.btn:active{

  

    transform: scale(1.30);

  

}

~~~

  

hasil :

![[home — Mozilla Firefox 2023-10-09 01-08-54.mp4]]

 *Analisis* :

   - `btn` merupakan sebuah kelas yang diberikan kepada elemen yang ingin diberi gaya tertentu.

    - `background-color: aqua;` mengatur warna latar belakang menjadi aqua.

    - `color: white;` mengatur warna teks menjadi putih.

    - `border: none;` menghilangkan border atau garis tepi elemen.

    - `width: 300px;` mengatur lebar elemen menjadi 300 piksel.

    - `height: 200px;` mengatur tinggi elemen menjadi 200 piksel.

    - `font-size: 50px;` mengatur ukuran font menjadi 50 piksel.

    - `font-family: 'segoe UI';` mengatur jenis font menjadi 'segoe UI'.

    - `font-weight: bold;` mengatur teks menjadi tebal.

    - `border-radius: 40px;` mengatur radius sudut border menjadi 40 piksel, memberikan efek sudut yang melengkung.

    - `cursor: pointer;` mengubah kursor menjadi tanda panah saat diarahkan ke elemen.

    - `transform: rotate3d();` terdapat kesalahan sintaksis dalam transformasi ini karena tidak ada nilai yang diberikan. Seharusnya ada nilai yang mengindikasikan rotasi pada sumbu tertentu.

    - `text` merupakan sebuah kelas yang diberikan kepada elemen teks.

    - `font-size: 50px;` mengatur ukuran font menjadi 50 piksel.

    - `font-style: italic;` mengatur teks menjadi miring (italic).

    - `font-family: 'calibri';` mengatur jenis font menjadi 'calibri'.

    - `color: antiquewhite;` mengatur warna teks menjadi antique white.

    - `body` merupakan selector yang mengatur properti pada elemen body.

    - `background-image: url(me.jpg);` mengatur gambar latar belakang dengan menggunakan file "me.jpg".

    - `text` merupakan pseudoselector yang tidak valid pada elemen body.

    - `btn:hover` merupakan sebuah pseudoselector yang akan diterapkan saat elemen dengan kelas `.btn` sedang dihover (diarahkan kursor kepadanya).

    - `background-color: blueviolet;` mengatur warna latar belakang menjadi blueviolet saat dihover.

    - `color: aqua;` mengatur warna teks menjadi aqua saat dihover.

    - `width: 500px;` mengatur lebar elemen menjadi 500 piksel saat dihover.

    - `transition: all 0.3s ease-in;` mengatur transisi perubahan properti menjadi halus dengan durasi 0.3 detik dan fungsi transisi ease-in.

    - `.btn:active` merupakan sebuah pseudoselector yang akan diterapkan saat elemen dengan kelas `.btn` sedang dalam status aktif (ditekan atau diklik).

    - `transform: scale(1.30);` mengatur skala elemen menjadi 1.30 kali ukuran aslinya saat dalam status aktif.
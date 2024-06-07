# Penjelasan
## Desklarasi
mendaftarkan variable ke dalam lingkup yang sesuai
### Inialisasi 
Menyiapkan Memori untuk variabel

### Assignment
menetapkan nilai yang spesifik ke dalam variabel



# Contoh Deklarasi , Inisialisasi , dan assignment

`var x; //proses deklarasi & inisalisasi
`x=30; // assignment`

# Keyword Deklarasi Variabel
## Contoh Var 
`Var` Jangan Pernah Space Teks Yang Ditulis
`var` 1kalicoba;
`var` yangboleh1;
`var` ada_garis_bawah;
`var` mataduitan$;

`Let`

`const`
# Keyword (Reserved word) yang tidak boleh dipakai
break case catch class conts continue debugger default delete to else enum export extends false finally for function  if implements import in instanceof interface let new null package private protected public return static super switch this throw true try typeof var void while with yield

# Javascript tutorial
## Peralatan Untuk Belajar Javascript
Apa saja peralatan yang harus disiapkan untuk belajar javascript
1. Web Browser (Google Chrome Firefox Opera Dll)
2. Teks Editor (Rekomendasi: Vs Code)
## Penulisan Java Script
1. Menulis javascript pada tag
`<script>`
penulisan kode javascript menggunakan tag `<script>` adalah cara umum yang digunakan
Tag `<script>`dapat kita buat didalam tag `<head>`maupun `<body>`
### Contoh
### Hasil 

Mana sih yang lebih baik ditulis dalam `<head>` atau di `<body>?`
kedua cara ini memang sah-sah saja dilakukan namun ada juga pendapat yang mengatakan
```
Placing script at the bottom of the `<body>` element improves the display speed. because script interpretation slows down the display
```
Penulis di akhir `<body>`
Meningkatkan kecepatan display atau tampilnya konten diweb Karena jika ditulis didalam `<head>`,script tersebut akan dieksekusi terlebih dahulu sebelum konten ditampilkan Jadi disarankan menulis kode javascript di dalam `<body>`, tepatya sebelum tutup `</body>`

2. Menulis javascript pada File eksternal
 Cara Kedua kita bisa menulis javascript di file yang terpisah dengan HTML Biasanya digunakan jika kita tidak ingin kode javascript bercampur dengan kode HTML
 Bagaimana caranya?
 Caranya buatlah sebuah file yang berekstensi `.js`file ini kita isi dengan kode javascript
 sebagai contoh saya akan membuat file eksternal dengan nama `kode-script.js`dan `file-external.html`sebagai kode HTML-nya
Berikut ini isi file `kode-script.js :`
![[ss document write.png]]
Lalu isi `file-external.html`adalah sebagai berikut.
![[contoh meta .png]]

Coba Perhatikan
Pada Kode HTML.`file-external.html`,kita tetap menggunakan tag `<script>`,Akan tetapi tag ini tidak kita isi dengan kode javascript melainkan kita menggunakan atribut `src` untuk menggunakan kode javascript yang ada difile `kode-script.js`

Perlu Diperhatikan Juga:
Tag `<script>`tetap harus ditutup dengan `</script>`walaupun tidak punya 
Dibawa Ini Contoh Yang salah
![[contoh salah src.png]]
Dibawa ini Contoh Yang Benar

![[Contoh yang benar .png]]
Lalu Bagaimana jika kode javascript-nya berada difolder yang berbeda dengan dokumen HTML-nya Atau Javascriptnya berada diinter? Untuk Kode javascript yang beara difolder yang berbeda kita menulis mengikuti alamat path foldernya

Misalnya Struktur foldernya seperti ini:

Karena File `kode-script.js` berada du dalam folder `js` maka kita harus menulisnya
![[Contoh yang benar .png]]
Nah, untuk kode javascript yang diambil dari internet kita cukup tuliskan alamat URL dari javascript tersebut contoh 
![[contoh visual code.png]]
3. Menulis Javascript pada atribut
Penulisan Javascript pada atribut biasanya dilakukan pada atribut event 
Contoh

![[contoh.png]]
Pada contoh ini kita membuat elemen `<button>`dan memiliki atribut `onclick`yang berisi kode javascript Nantinya kode javascript yang ada didalam atribut `onclick`akan dieksekusi saat event klik terjadi pada elemen `<button>`
Apakah Javascript hanya bisa ditulis pada atribut `onclick`saja? Atribut event yang ada DiHTML kode javascript bisa ditulis disemua atribut event
ingat atribut event bukan atribut biasa jika kamu ingin lihat semua atribut event silahkan cek `Event.Reference`

Penulisan atribut event di HTML diawali dengan `on`misalnya untuk event `click`maka pada atribut HTML ditulis `onclick`
Contoh lagi biar makin paham
![[contoh meta .png]]
Pada contoh ini kita menggunakan envent `keyup` maka ditulis `onkeyup`.event ini terjadi saat kita melepas tombol dikeyboard jadi nantinya saat kita mengetik pada elemen `<textarea>`,kode javascript yang ada di `onkeyup`akan dieksekusi Kode Javascript tersebut berfungsi untuk menampilkan jumlah karakter yang diketik

4.Penulisan Javascript pada URL 
Nah Ini yang menurut saya cacra yang cukup aneh Cara ini memang jarang digunakan dan hampir tidak ada yang menggunakannya di dalam aplikasi Tapi tetap bisa caranya pada URL kita gunakan `javascript:`Lalu diikuti dengan kode javascript yang ingin dieksekusi
Contoh:
![[javascript.js.png]]
ini diketik pada addres bar browser: 
`"Catatan: Cara ini tidak bekerja diweb browser versi terbaru karena ini merupakan sebuah celah yang bisa dipakai untuk serangan XSS."`
Lalu Bagaimana kita menggunakan cara ini diHTML Cara ini bisa kita gunakan pada tag `<a>`lalu mengisinya diatribut `href`.
Contoh
![[a href.png]]
Hasilnya:

Jadi Saat link `<a>`diklik ia akan membuka URL `javascript:` dan menjalankan kode javascript yang ada disana  Mirip seperti evnet `onclick`ya 
Akhir Kata
Nah itulah 4cara menulis javascript di HTML Cara manakh yang akan kamu gunakan menurut saya cara pertama kedua dan ketiga cukup sering dan umum dipakai sedangkan cara keempat tidak saya rekomendasikan untuk digunakan cukup diketahui sja
## Menampilkan Output pada javascript 
Output adalah sebuah tampilan programn yang biasanya digunakan untuk memperhatikan hasil akhir
1. Menggunakan Fungsi `console.log();`
2. Menggunakan Fungsi `alert();`
3. Menggunakan Fungsi
  `document.write();`
4. Menggunakan innerHTML.
  Apaan Perbedaan dari keempat cara tersebut
  
1. Menggunakan Fungsi
   `console.log()`
   Fungsi `console.log()`adalah fungsi untuk menampilkan teks keconsole javascript 
   contoh penggunaan
  ![[console log.png]]
  Hasilnya

Fungsi `Console.log()` biasanya digunakan untuk debugging karena setiap perasaan error dijavascript selalu ditampilkan didalam console.
Selain `console.log()`terdapat juga beberapa fungsi untuk debugging seperti
`console.debug()`, `console.info()`
`console.error()`, `console.dir()`
dsb
Fungsi fungsi console ini juga berlaku pada console nodejs.

2. Menggunakan Fungsi `alert()`
Fungsi `alert()`adalah fungsi untuk menampilkan jendela dialog.Fungsi menampilkan jendela dialog.fungsi sebenarnya berada pada objek `windows` secara lengkap ditulis

![[Screenshot 2024-01-23 231336.png]]
Bisa juga ditulis `alert()`saja seperti ini:


Fungsi `alert()`hanya bisa digunakan didalm browser saja sedangkan pada nodejs fungsi ini tidak ada


Contoh penggunaan fungsi `alert():`
![[doctype function.png]]
Hasilnya:


3. Menggunakan Fungsi 
`document.write()`
Objek `document`adalah objek yang mewakili dokumen HTML didalam Javascript Dalam Objek `document`,terdapat fungsi `write()`untuk menulis sesuatu ke dokumen HTML
Contoh:
![[write.png]]
Hasilnya :   


Selain Fungsi `write()`.objek `document`juga menyediakan berbagai macam fungsi untuk manipulasi dokumen HTML

4. Menggunakan `InnerHTML`
`innerHTML`adalah sebuah atribut didalam (objek)elemen HTML. Yang berisi string HTML..
Dengan `innerHTML`kita dapata menampilkan output keelemen yang lebih spesifik

Contoh
![[var.png]]
Hasilnya :  


Kita Ringkas akan seperti ini:
1. fungsi `console.log()`untuk menampilkan output ke console javascript:
2. Fungsi `alert()`untuk menampilkan output kejendela dialog :  
3. Fungsi `document.write()`untuk menulis output kedokumen HTML 
4. Atribut `innerHTML`untuk menampilkan output keelemen HTML.yang lebih spesifik

## Cara membuat Variabel DiJavascript
cara membuat variabel yang umum digunakan di javascript adalah menggunakan kata kunci `var` lalu diikuti dengan nama variabel dan nilainya 
Contoh
![[var pak fajar.png]]
Pada Contoh diatas kita membuat variabel bernama `title`dengan nilai berupa teks `(string);` `"Belajar Programan Javascript"`
## 1. Dialog Alert

Dialog `alert()` biasanya digunakan untuk menampilkan sebuah pesan peringatan atau informasi.

Fungsi `alert()` berada dalam objek `window`.

Kita bisa menggunakannya seperti ini:

```javascript
window.alert("Hello World!");
```

Atau seperti ini:

```javascript
alert("Hello kawan");
```

Karena objek `window` berisfat global, kita boleh tidak menulisnya.

Dialog `alert()` tidak akan mengembalikan nilai apa-apa saat dieksekusi.

Mari kita coba:

```html
<!DOCTYPE html>
<html>
    <head>
        <title>Dialog Alert</title>
    </head>
    <body>
    <script>
        alert("Selamat datang di tutorial Javascript");
    </script>
    </body>
</html>
```

Hasilnya:

![Jendela dialgo alert](https://www.petanikode.com/img/js/dialog/alert.png)
Dialog `alert()` memiliki satu perameter yang harus diberikan, yaitu: teks yang akan ditampilkan pada dialog.

Pada contoh di atas, kita memberikan teks `"Selamat datang di tutorial Javascript"`.

Pertanyaanya:

Bagaimana cara menampilkan dialog `alert()` pada _event_ tertentu, misalnya saat sebuah tombol diklik?

Ini bisa kita lakukan dengan menambahkan fungsi dialog pada _event_ _listener_.

Pada HTML, kita bisa masukan fungsi `alert()` pada atribut `onClick` agar nanti ditampilkan saat sebuah elemen diklik.

Contoh:

```html
<!DOCTYPE html>
<html>
    <head>
        <title>Dialog Alert</title>
    </head>
    <body>
        <button onClick="alert('Tombol diklik!')">Klik Saya</button>
    </body>
</html>
```

Hasilnya:

![Jendela dialog alert tampil saat tombol diklik](https://www.petanikode.com/img/js/dialog/alert-click.gif)

## 2. Dialog Confirm

Dialog `confirm()` digunakan untuk melakukan konfirmasi dalam melakukan tindakan tertentu.

Misalnya:

Saat kita menghapus sesuatu, maka ada baiknya menampilkan dialog `confirm()`. Karena tindakan tersebut cukup berbahaya.

Dialog confirm dapat dibuat dengan fungsi `confirm()`.

Contoh: ```javascript
onfirm("Apakah anda yakin akan menghapus?");
```

Dialog `confirm()` akan mengembalikan nilai `true` apabila kita memilih tombol **OK** dan akan mengembalikan nilai `false` apabila kita memilih **Cancel**.

Nilai kembalian ini dapat kita tampung dalam variabel untuk diproses.

Contoh:

```html
<!DOCTYPE html>
<html>
    <head>
        <title>Dialog Confirm</title>
    </head>
    <body>
    <script>
        var yakin = confirm("Apakah kamu yakin akan mengunjungi petanikode?");

        if (yakin) {
            window.location = "https://www.petanikode.com";
        } else {
            document.write("Baiklah, tetap di sini saja ya :)");
        }
    </script>
    </body>
</html>
```

Hasilnya:

![Jendela dialog konfirmasi](https://www.petanikode.com/img/js/dialog/confirm.gif)

## 3. Dialog Prompt

Dialog `prompt()` berfungsi untuk mengambil sebuah inputan dari pengguna.

Dialog `prompt()` akan mengembalikan sebuah nilai string dari apa yang diinputkan oleh pengguna.

Contoh:

```html
<!DOCTYPE html>
<html>
    <head>
        <title>Dialog Promp</title>
    </head>
    <body>
    <script>
        var nama = prompt("Siapa nama kamu?", "");
        document.write("<p>Hello "+ nama +"</p>");
    </script>
    </body>
</html>
```

Hasilnya:

![Jendela dialog prompt](https://www.petanikode.com/img/js/dialog/prompt.gif)

Dialog `prompt()` memiliki beberapa parameter yang harus diberikan:

1. Teks yang akan ditampilkan pada form;
2. Nilai default untuk field input.

Pada contoh di atas, kita memberikan nilai default-nya berupa string kosong dengan tanda petik `""`.
Apa itu operator?

Ada operator apa saja di Javascript?

dan bagaimana cara menggunakannya?

Mari kita pelajar…

Misalkan kita punya dua variabel seperti ini:

```javascript
var a = 3;
var b = 4;
```

Bagaimana cara menjumlahkan variabel `a` dan `b`?

Jawabannya: menggunakan tanda plus (`+`).

```javascript
var c = a + b;
```

Hasil penjumlahannya akan disimpan di dalam variabel `c`.

Tanda plus `+` adalah sebuah operator.

Jadi…

## Apa itu Operator?

Operator adalah simbol yang digunakan untuk melakukan operasi pada suatu nilai dan variabel.

Operator dalam pemrograman terbagi dalam 6 jenis:

1. Operator aritmatika;
2. Operator Penugasan (Assignment);
3. Operator relasi atau perbandingan;
4. Operator Logika;
5. Operator Bitwise;
6. Operator Ternary;

Operator wajib ada di setiap bahasa pemrograman. Ke 6 jenis operator di atas harus kamu pahami.

Mari kita bahas satu-persatu…

## 1. Operator Aritmatika pada Javascript

Operator aritmatika merupakan operator untuk melakukan operasi aritmatika seperti penjumlahan, pengurangan, pembagian, perkalian, dsb.

Operator aritmatika terdiri dari:

|Nama Operator|Simbol|
|---|---|
|Penjumlahan|+|
|Pengurangan|-|
|Perkalian|*|
|Pemangkatan|**|
|Pembagian|/|
|Sisa Bagi|%|

Untuk melakukan operasi perkalian, kita menggunakan simbol asterik `*`.

Jangan gunakan `x`, karena simbol `x` bukan termasuk dalam operator di dalam pemrograman.

Lalu untuk pemangkatan kita menggunakan asterik ganda `**`.

Untuk pembagian, kita gunakan simbol garis miring `/`.

Mari kita coba…

Contoh:

```javascript
var a = 5;
var b = 3;

// menggunakan operator penjumlahan
var c = a + b;
console.log(c);
```

Hasilnya:

![Operator penjumlahan pada javascript](https://www.petanikode.com/img/js/operator/penjumlahan.png)

Coba juga untuk operator yang lainnya:

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <title>Operator Aritmatika</title>
</head>

<body>

    <script>
        var a = 15;
        var b = 4;
        var c = 0;

        // pengurangan
        c = a - b;
        document.write(`${a} - ${b} = ${c}<br/>`);

        // Perkalian
        c = a * b;
        document.write(`${a} * ${b} = ${c}<br/>`);

        // pemangkatan
        c = a ** b;
        document.write(`${a} ** ${b} = ${c}<br/>`);

        // Pembagian
        c = a / b;
        document.write(`${a} / ${b} = ${c}<br/>`);

        // Modulo
        c = a % b;
        document.write(`${a} % ${b} = ${c}<br/>`);
    </script>
</body>

</html>
```

Hasilnya:

![Operator aritmatika di Javascript](https://www.petanikode.com/img/js/operator/aritmatika.png)

Coba perhatikan operator modulo (`%`) dan operator penjumlahan (`+`).

Operator modulo adalah operator untuk menghitung sisa bagi.

Misal `3` dibagi `2`, maka sisanya adalah `1`.

```javascript
3 % 2 = 1
```

### Operator Penggabungan Teks

Mohon perhatikan!

Jangan sampai salah.

Pada Javascript, apabila kita akan melakukan operasi terhadap **tipe data string** atau teks menggunakan penjumlahan (`+`), maka yang akan terjadi adalah **penggabungan**; Bukan penjumlahan.

Contoh:

```javascript
var a = "10" + "2";
```

Maka hasilnya akan:

```txt
102
```

Kenapa tidak `12`?

Karena kedua angka tersebut merupakan string—perhatikan, dia diapit dengan tanda petik.

Untuk operasi yang lainnya, silakan dicoba-coba melalui _console_.

![Operasi string di Javascript](https://www.petanikode.com/img/js/operator/operasi-string.png)

## 2. Operator Penugasan pada Javascript

Operator penugasan adalah operator yang digunakan untuk memberikan tugas kepada variabel. Biasanya digunakan untuk mengisi variabel.

Contoh:

```javascript
var a = 19;
```

Variabel `a` kita berikan tugas untuk menyimpan nilai `19`.

Operator penugasan terdiri dari:

|Nama Operator|Sombol|
|---|---|
|Pengisian Nilai|=|
|Pengisian dan Penambahan|+=|
|Pengisian dan Pengurangan|-=|
|Pengisian dan Perkalian|*=|
|Pengisian dan Pemangkatan|**=|
|Pengisian dan Pembagian|/=|
|Pengisian dan Sisa bagi|%=|

Operator penugasan sama seperti operator aritmatika. Ia juga digunakan untuk melakukan operasi aritmatika.

Contoh:

```javascript
var jumlahView = 12;

// menggunakan operator penugasan penjumlahan
// untuk menambah nilai
jumlahView += 1;
```

Hasilnya:

Variabel `jumlahView` akan bertambah satu.

Maksud dari `jumlahView += 1` adalah seperti ini:

```javascript
jumlahView = jumlahView + 1;
```

Bisa dibaca:

Isi variabel `jumlahView` dengan penjumlahan dari nilai `jumlahView` sebelumnya dengan `1`.

Khusus untuk operator penugasan yang dijumlahkan dan dikurangi dengan satu, bisa disingkat dengan `++` dan `--` untuk pengurangan.

Contoh:

```javascript
var a = 2;
a++;
```

Maka nilai dari variabel `a` akan menjadi `3`.

Lalu pertanyaannya:

Apa bedanya dengan operator penugasan dengan operator aritmatika?

Operator aritmatika hanya melakukan operasi aritmatika saja, sedangkan operator penugasan… ia melakukan operasi aritmatika dan juga pengisian.

Berikut ini contoh operator penugasan:

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <title>Operator Penugasan</title>
</head>

<body>

    <script>
        document.write("Mula-mula nilai score...<br>");
        // pengisian nilai
        var score = 100;
        document.write("score = "+ score + "<br/>");

        // pengisian dan menjumlahan dengan 5
        score += 5;
        document.write("score = "+ score + "<br/>");

        // pengisian dan pengurangan dengan 2
        score -= 2;
        document.write("score = "+ score + "<br/>");

        // pengisian dan perkalian dengan 2
        score *= 2;
        document.write("score = "+ score + "<br/>");

        // pengisian dan pembagian dengan 4
        score /= 4;
        document.write("score = "+ score + "<br/>");

        // pengisian dan pemangkatan dengan 2
        score **= 2;
        document.write("score = "+ score + "<br/>");

        // pengisian dan modulo dengan 3;
        score %= 3;
        document.write("score = "+ score + "<br/>");
    </script>
</body>

</html>
```

Hasilnya:

![Contoh operator penugasan pada Javascript](https://www.petanikode.com/img/js/operator/penugasan.png)

## 3. Operator Perbandingan pada Javascript

Operator relasi atau perbandingan adalah operator yang digunakan untuk membandingkan dua nilai.

Operator perbandingan akan menghasilkan sebuah nilai _boolean_ `true` dan `false`.

Operator perbandingan terdiri dari:

|Nama Operator|Simbol|
|---|---|
|Lebih Besar|>|
|Lebih Kecil|<|
|Sama Dengan|== atau ===|
|Tidak Sama dengan|!= atau !==|
|Lebih Besar Sama dengan|>=|
|Lebih Kecil Sama dengan|<=|

Contoh:

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <title>Operator Perbandingan</title>
</head>

<body>

    <script>
        var aku = 20;
        var kamu = 19;

        // sama dengan
        var hasil = aku == kamu;
        document.write(`${aku} == ${kamu} = ${hasil}<br/>`);
        
        // lebih besar
        var hasil = aku > kamu;
        document.write(`${aku} > ${kamu} = ${hasil}<br/>`);
        
        // lebih besar sama dengan
        var hasil = aku >= kamu;
        document.write(`${aku} >= ${kamu} = ${hasil}<br/>`);
        
        // lebih kecil
        var hasil = aku < kamu;
        document.write(`${aku} < ${kamu} = ${hasil}<br/>`);
        
        // lebih kecil sama dengan
        var hasil = aku <= kamu;
        document.write(`${aku} <= ${kamu} = ${hasil}<br/>`);
        
        // tidak sama dengan
        var hasil = aku != kamu;
        document.write(`${aku} != ${kamu} = ${hasil}<br/>`);
    </script>
</body>

</html>
```

Hasilnya:

![Contoh operator relasi di Javascript](https://www.petanikode.com/img/js/operator/relasi.png)

Pertanyaannya:

Apa perbedaan `==` (dua simbol sama dengan) dengan `===` (tiga simbol sama dengan)?

Perbandingan dengan menggunakan simbol `==` hanya akan membandingkan nilai saja. Sedangkan yang menggunakan `===` akan membandingkan dengan tipe data juga.

Contoh:

```javascript
// ini akan bernilai true
var a = "4" == 4; //-> true

// sedangkan ini akan bernilai false
var b = "4" === 4; //-> false
```

Mengapa nilai `b` bernilai `false`?

Karena `"4"` (string) dan `4` (integer). Tipe datanya berbeda.

## 4. Operator Logika pada Javascript

Operator logika digunakan untuk melakukan operasi terhadap dua nilai `boolean`.

Operator ini terdiri dari:

|Nama Operator|Simbol|
|---|---|
|Logika AND|&&|
|Logika OR|\||
|Negasi/kebalikan|!|

Contoh:

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <title>Operator Logika</title>
</head>

<body>

    <script>
        var aku = 20;
        var kamu = 19;

        var benar = aku > kamu;
        var salah = aku < kamu;

        // operator && (and)
        var hasil = benar && salah;
        document.write(`${benar} && ${salah} = ${hasil}<br/>`);
        
        // operator || (or)
        var hasil = benar || salah;
        document.write(`${benar} || ${salah} = ${hasil}<br/>`);
        
        // operator ! (not)
        var hasil = !benar
        document.write(`!${benar} = ${hasil}<br/>`);

    </script>
</body>

</html>
```

Hasilnya:

![Contoh operator logika di javascript](https://www.petanikode.com/img/js/operator/logika.png)

## 5. Operator Bitwise pada Javascript

Operator bitwise merupakan operator yang digunakan untuk operasi berdasarkan bit (biner).

Operator ini terdiri dari:

|Nama|Simbol di Java|
|---|---|
|AND|&|
|OR|\||
|XOR|^|
|Negasi/kebalikan|~|
|Left Shift|«|
|Right Shift|»|
|Left Shift (unsigned)|«<|
|Right Shift (unsigned)|»>|

Operator ini berlaku untuk tipe data `int`, `long`, `short`, `char`, dan `byte`.

Operator ini akan menghitung dari bit-ke-bit.

Misalnya, kita punya variabel `a = 60` dan `b = 13`.

Bila dibuat dalam bentuk biner, akan menjadi seperti ini:

```ruby
a = 00111100
b = 00001101
```

_(perhatikan bilangan binernya, angka `0` dan `1`)_

Kemudian, dilakukan operasi bitwise

Operasi AND

```ruby
a     = 00111100
b     = 00001101
a & b = 00001100
```

Operasi OR

```ruby
a     = 00111100
b     = 00001101
a | b = 00111101
```

Operasi XOR

```ruby
a     = 00111100
b     = 00001101
a ^ b = 00110001
```

Operasi NOT (Negasi/kebalikan)

```ruby
a   = 00111100
~a  = 11000011
```

Konsepnya memang hampir sama dengan operator Logika. Bedanya, Bitwise digunakan untuk biner.

Untuk lebih jelasnya…

Mari kita coba lihat contohnya:

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <title>Operator Bitwise</title>
</head>

<body>

    <script>
        var x = 4;
        var y = 3;

        // operator bitwise and
        var hasil = x & y;
        document.write(`${x} & ${y} = ${hasil}<br/>`);

        // operator bitwise or
        var hasil = x | y;
        document.write(`${x} | ${y} = ${hasil}<br/>`);

        // operator bitwise xor
        var hasil = x ^ y;
        document.write(`${x} ^ ${y} = ${hasil}<br/>`);

        // operator negasi
        var hasil = ~x;
        document.write(`~${x} = ${hasil}<br/>`);
        
        // operator bitwise right shift >>
        var hasil = x >> y;
        document.write(`${x} >> ${y} = ${hasil}<br/>`);

        // operator bitwise right shift <<
        var hasil = x << y;
        document.write(`${x} << ${y} = ${hasil}<br/>`);

        // operator bitwise right shift (unsigned) >>>
        var hasil = x >>> y;
        document.write(`${x} >>> ${y} = ${hasil}<br/>`);

    </script>
</body>

</html>
```

Hasilnya:

![Contoh operator bitwise dalam Javascript](https://www.petanikode.com/img/js/operator/bitwise.png)

## 6. Operator Ternary pada Javascript

Terakhir ada operator Ternary…

Operator ternary merupakan operator yang terdiri dari tiga bagian.

Operator-operator sebelumnya hanya dua bagian saja, yaitu: bagian kiri dan kanan. Ini disebut operator binary.

Sementara operator trinary ada bagian kiri, tengah, dan kanan.

```txt
bagian kiri <operator> bagian tengah <operator> bagian kanan
```

Operator ternary pada Javascript, biasanya digunakan untuk membuat sebuah percabangan _if/else_.

Simbol operator ternary terdiri dari tanda tanya dan titik dua (`?:`).

Bentuknya seperti ini:

```txt
<kondisi> ? "benar" : "salah"
```

Perhatikan! `<kondisi>` dapat kita isi dengan ekspresi yang menghasilkan nilai `true` dan `false`.

Apabila kondisi bernilai `true`, maka `"benar"` yang akan dipilih dan sebaliknya—apabila `false`—maka `"salah"` yang akan dipilih.

Operator ini unik, seperti membuat pertanyaan.

![Bentuk operator ternary](https://3.bp.blogspot.com/-OKB4MDtGjE4/WObxiPfq-wI/AAAAAAAAEmQ/kR9Ldcc1hr88u90060rCff0Gvs4lDRfQgCPcB/s1600/operator%2Bternary%2Bdi%2Bjava.png)

Pada contoh di atas, “Kamu suka aku” adalah pertanyaan atau kondisi yang akan diperiksa.

Kalau jawabannya benar, maka `iya`. Sebaliknya akan `tidak`.

Lebih jelasnya, mari kita coba contohnya.

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <title>Operator Ternary</title>
</head>

<body>

    <script>
        var pertanyaan = confirm("Apakah kamu berumur di atas 18 tahun?")

        var hasil = pertanyaan ? "Selamat datang" : "Kamu tidak boleh di sini";
        document.write(hasil);
    </script>
</body>

</html>
```

Hasilnya:

![Contoh operator ternary pada Javascript](https://www.petanikode.com/img/js/operator/ternary.gif)

Apa itu percabangan dan kenapa dinamakan percabangan?

Buat yang belum pernah kuliah atau belajar tentang algoritme dan flowchart, mungkin ini istilah yang baru pertama kamu dengar.

Istilah ini sebenarnya untuk menggambarkan alur program yang bercabang.

Pada flow chart, logika **“jika…maka”** digambarkan dalam bentuk cabang.

![Logika program jika/maka](https://www.petanikode.com/img/python/percabangan/jika-maka.png)

Karena itu, ini disebut percabangan.

Selain percabangan, struktur ini juga disebut: _control flow_, _decision_, struktur kondisi, Struktur if, dsb.

Percabangan akan mampu membuat program berpikir dan menentukan tindakan sesuai dengan logika/kondisi yang kita berikan.

Pada pemrograman Javascript, terdapat **6 bentuk percabangan** yang **harus** kita kitahui.

Apa saja itu?

Mari kita bahas…

## 1. Percabangan _if_

Percabangan _if_ merupakan percabangan yang hanya memiliki **satu blok pilihan** saat kondisi bernilai benar.

Coba perhatikan _flowchart_ berikut ini:

![Flowchart percabangan if](https://www.petanikode.com/img/js/percabangan/flowchart-if.png)

_Flowchart_ tersebut dapat kita baca seperti ini:

“Jika total belanja lebih besar dari Rp 100.000, Maka tampilkan pesan **Selamat, Anda dapat hadiah**”

Kalau di bawah Rp 100.000 bagaimana?

Ya pesannya tidak ditampilkan.

Mari kita coba dalam program Javascript:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Percabangan if</title>
</head>
<body>
    <script>
        var totalBelanja = prompt("Total belanja?", 0);

        if(totalBelanja > 100000){
            document.write("<h2>Selamat Anda dapat hadiah</h2>");
        }

        document.write("<p>Terima kasih sudah berbelanja di toko kami</p>");
    </script>
</body>
</html>
```

Hasilnya:

![Contoh program percabangan if di javascript](https://www.petanikode.com/img/js/percabangan/demo-if.gif)

Perhatikan bagian ini:

```javascript
if(totalBelanja > 100000){
    document.write("<h2>Selamat Anda dapat hadiah</h2>");
}
```

Ini yang disebut blok.

Blok program pada Javascript, diawali dengan tanda buka kurung kurawal `{` dan diakhiri dengan tutup kurung kurawal `}`.

Apabila di dalam blok hanya terdapat satu baris ekspresi atau statement, maka boleh tidak ditulis tanda kurungnya.

```javascript
if(totalBelanja > 100000)
    document.write("<h2>Selamat Anda dapat hadiah</h2>");
```

## 2. Percabangan _if/else_

Percabangan _if/else_ merupakan percabangan yang memiliki **dua blok pilihan**.

Pilihan pertama untuk kondisi **benar**, dan pilihan kedua untuk kondisi **salah** (_else_).

Coba perhatikan flowchart ini:

![Flowchart percabangan if/else](https://www.petanikode.com/img/js/percabangan/flowchart-if-else.png)

Ini adalah flowchart untuk mengecek password.

Apabila password benar, pesan yang ada pada blok hijau akan ditampilkan: **“Selamat datang bos!”**

Tapi kalau salah, maka pesan yang ada di blok merah yang akan ditampilkan: **“Password salah, coba lagi!”**

Kemudian, pesan yang berada di blok abu-abu akan tetap ditampilkan, karena dia bukan bagian dari blok percabangan _if/else_.

Perhatikan arah panahnya, setiap blok _if/else_ mengarah ke sana…

![Flowchart percabangan if/else](https://www.petanikode.com/img/js/percabangan/flowchart-if-else-arrow.png)

Untuk lebih jelasnya, mari kita coba dalam program:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Percabangan if/else</title>
</head>
<body>
    <script>
        var password = prompt("Password:");

        if(password == "kopi"){
            document.write("<h2>Selamat datang bos!</h2>");
        } else {
            document.write("<p>Password salah, coba lagi!</p>");
        }

        document.write("<p>Terima kasih sudah menggunakan aplikasi ini!</p>");

    </script>
</body>
</html>
```

Hasilnya:

![Contoh program percabangan if/else di javascript](https://www.petanikode.com/img/js/percabangan/demo-if-else.gif)

## 3. Percabangan _if/else/if_

Percabangan _if/else/if_ merupakan percabangan yang memiliki **lebih dari dua blok pilihan**.

Coba perhatikan flowchart berikut:

![Flowchart percabangan if/else/if](https://www.petanikode.com/img/js/percabangan/if-else-if.png)

Perhatikan blok yang saya beri warna…

Ini adalah blok untuk percabangan _if/else/if_. Kita bisa menambahkan berapapun blok yang kita inginkan.

Contoh Program:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Percabangan if/else/if</title>
</head>
<body>
    <script>
        var nilai = prompt("Inputkan nilai akhir:");
        var grade = "";

        if(nilai >= 90) grade = "A"
        else if(nilai >= 80) grade = "B+"
        else if(nilai >= 70) grade = "B"
        else if(nilai >= 60) grade = "C+"
        else if(nilai >= 50) grade = "C"
        else if(nilai >= 40) grade = "D"
        else if(nilai >= 30) grade = "E"
        else grade = "F";

        document.write(`<p>Grade anda: ${grade}</p>`);
    </script>
</body>
</html>
```

Hasilnya:

![Contoh program percabangan if/else/if di javascript](https://www.petanikode.com/img/js/percabangan/demo-if-else-if.gif)

Pada program di atas, kita tidak menggunakan kurung kurawal untuk membuat blok kode untuk _if/else/if_.

karena hanya terdapat satu baris perintah saja. Yaitu: `grade = ...`.

Bila kita menggunakan kurung kurawal, maka program di atas akan menjadi seperti ini:

```html
<script>
    var nilai = prompt("Inputkan nilai akhir:");
    var grade = "";

    if (nilai >= 90){
        grade = "A"
    } else if(nilai >= 80) {
        grade = "B+"
    } else if(nilai >= 70) {
        grade = "B"
    } else if(nilai >= 60) {
        grade = "C+"
    } else if(nilai >= 50) {
        grade = "C"
    } else if(nilai >= 40) {
        grade = "D"
    } else if(nilai >= 30) {
         grade = "E"
    } else { 
        grade = "F";
    }
    document.write(`<p>Grade anda: ${grade}</p>`);
</script>
```

## 4. Percabangan _switch/case_

Percabangan _switch/case_ adalah bentuk lain dari percabangan _if/else/if_.

Strukturnya seperti ini:

```javascript
switch(variabel){
    case <value>:
        // blok kode
        break;
    case <value>:
        // blok kode
        break;
    default:
        // blok kode
}
```

Kita dapat membuat blok kode (`case`) sebanyak yang diinginkan di dalam blok switch.

Pada `<value>`, kita bisa isi dengan nilai yang nanti akan dibandingkan dengan `variabel`.

Setiap `case` harus diakhiri dengan `break`. Khusus untuk `default`, tidak perlu diakhiri dengan `break` karena dia terletak di bagian akhir.

Pemberian `break` bertujuan agar program berhenti mengecek `case` berikutnya saat sebuah `case` terpenuhi.

Contoh:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Percabangan switch/case</title>
</head>
<body>
    <script>

        var jawab = prompt("Kamu beruntung! Silakan pilih hadiahmu dengan memasukkan angka 1 sampai 5");
        var hadiah = "";
        
        switch(jawab){
            case "1":
                hadiah = "Tisu";
                break;
            case "2":
                hadiah = "1 Kotak Kopi";
                break;
            case "3":
                hadiah = "Sticker";
                break;
            case "4":
                hadiah = "Minyak Goreng";
                break;
            case "5":
                hadiah = "Uang Rp 50.000";
                break;
            default:
                document.write("<p>Opps! anda salah pilih</p>");
        }

        if(hadiah === ""){
            document.write("<p>Kamu gagal mendapat hadiah</p>");
        } else {
            document.write("<h2>Selamat kamu mendapatkan " + hadiah + "</h2>");
        }
    </script>
</body>
</html>
```

Hasilnya:

![Contoh program percabangan switch/case di javascript](https://www.petanikode.com/img/js/percabangan/demo-switch-case.gif)

Percabangan _switch/case_ juga dapat dibuat seperti ini:

```javascript
var nilai = prompt("input nilai");
var grade = "";

switch(true){
    case nilai < 90:
        grade = "A";
        break;
    case nilai < 80:
        grade = "B+";
        break;
    case nilai < 70:
        grade = "B";
        break;
    case nilai < 60:
        grade = "C+";
        break;
    case nilai < 50:
        grade = "C";
        break;
    case nilai < 40:
        grade = "D";
        break;
    case nilai < 30:
        grade = "E";
        break;
    default:
        grade = "F";
}
```

Pertama-tama, kita berikan nilai `true` pada `switch`, ini agar kita bisa masuk ke dalam blok `switch`.

Lalu di dalam blok `switch`, kita buat kondisi dengan menggunakan `case`.

Hasilnya akan sama seperti pada contoh percabangan _if/else/if_.

## 5. Percabangan dengan Operator Ternary

Percabangan menggunakan operator _ternary_ merupakan bentuk lain dari percabangan _if/else_.

Bisa dibilang:

Bentuk singkatnya dari _if/else_.

Contoh:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Percabangan Ternary</title>
</head>
<body>
    <script>
        var jwb = prompt("Apakah Jakarta ibu kota indonesia?");

        var jawaban = (jwb.toUpperCase() == "IYA") ? "Benar": "Salah";

        document.write(`Jawaban anda: <b>${jawaban}</b>`);
    </script>
</body>
</html>
```

Fungsi dari method `toUpperCase()` untuk mengubah teks yang diinputkan menjadi huruf kapital semua.

Hasilnya:

![Contoh program percabangan dengan operator ternary di javascript](https://www.petanikode.com/img/js/percabangan/demo-ternary.gif)

Operator _ternary_ berperan sebagai percabangan _if/else_:

```javascript
var jawaban = (jwb.toUpperCase() == "IYA") ? "Benar": "Salah";
```

Apabila kondisi yang ada di dalam kurung—`(jwb.toUpperCase() == "IYA")`—bernilai `true`, maka nanti isi dari variabel `jawaban` akan sama dengan `"Benar"`.

Tapi kalau bernilai `false`, maka variabel `jawaban` akan berisi `"Salah"`.

## 6. Percabangan Bersarang _(Nested)_

Kita juga dapat membuat blok percabangan di dalam percabangan. Ini disebut percabangan bersarang atau _nested if_.

Contoh:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Percabangan Ternary</title>
</head>
<body>
    <script>
        var username = prompt("Username:");
        var password = prompt("Password:");

        if(username == "petanikode"){
            if(password == "kopi"){
                document.write("<h2>Selamat datang pak bos!</h2>");
            } else {
                document.write("<p>Password salah, coba lagi!</p>");
            }
        } else {
            document.write("<p>Anda tidak terdaftar!</p>");
        }
    </script>
</body>
</html>
```

Hasilnya:

![Contoh program percabangan bersarang di javascript](https://www.petanikode.com/img/js/percabangan/demo-nested.gif)

## Bonus: Menggunakan Operator Logika pada Percabangan

Percabangan bersarang, sebenarnya bisa kita buat lebih sederhana lagi dengan menggunakan operator logika.

Contohnya:

```javascript
var username = prompt("Username:");
var password = prompt("Password:");

if(username == "petanikode"){
    if(password == "kopi"){
        document.write("<h2>Selamat datang pak bos!</h2>");
    } else {
        document.write("<p>Password salah, coba lagi!</p>");
    }
} else {
    document.write("<p>Anda tidak terdaftar!</p>");
}
```

Ini dapat kita buat lebih sederhana lagi dengan operator logika AND (`&&`).

```javascript
var username = prompt("Username:");
var password = prompt("Password:");

if(username == "petanikode" && password == "kopi"){
    document.write("<h2>Selamat datang pak bos!</h2>");
} else {
    document.write("<p>Password salah, coba lagi!</p>");
}
```

Namun, ini bukanlah solusi terbaik.

Karena kita tidak bisa mengecek, apakah user terdaftar atau tidak.

## Apa itu Array?

Sebelum kita membahas Array, kita bahas dulu apa itu struktur data?

**Struktur data** merupakan cara-cara atau metode yang digunakan untuk menyimpan data di dalam memori komputer.

Salah satu struktur data yang sering digunakan dalam pemrograman adalah **Array**.

Array merupakan struktur data yang digunakan untuk **menyimpan sekumpulan data** dalam satu tempat.

Setiap data dalam Array memiliki indeks, sehingga kita akan mudah memprosesnya.

![Array](https://www.petanikode.com/img/php/array/array.png)

Indeks array selalu dimulai dari angka nol (`0`).

Pada teori struktur data…

…Ukuran array akan bergantung dari banyaknya data yang ditampung di dalamnya.

## Cara Membuat Array pada Javascript

Pada javascript, array dapat kita buat dengan tanda kurung siku (`[...]`).

Contoh:

```javascript
var products = [];
```

Maka variabel `products` akan berisi sebuah array kosong.

Kita bisa mengisi data ke dalam array, lalu setiap data dipisah dengan tanda koma (`,`).

Contoh:

```javascript
var products = ["Flash disk", "SDD", "Monitor"];
```

Oya, karena javascript merupakan bahasa pemrograman yang _dynamic typing_…

…maka kita bisa menyimpan dan mencampur apapun di dalam array.

Contoh:

```javascript
var myData = [12, 2.1, true, 'C', "Petani Kode"];
```

## Cara Mengambil Data dari Array

Seperti yang sudah kita ketahui…

Array akan menyimpan sekumpulan data dan memberinya nomer indeks agar mudah diakses.

Indeks array selalu dimulai dari nol `0`.

Misalkan kita punya array seperti ini:

```javascript
var makanan = ["Nasi Goreng", "Mie Ayam", "Mie Gelas"];
```

Bagaimana cara kita mengambil nilai `"Mie Ayam"`?

Jawabannya seperti ini:

```javascript
makanan[1] //-> "Mie Ayam"
```

Kenapa bukan `2`?

Ingat: indeks array selalu dimulai dari nol.

Biar lebih jelas, mari kita coba dalam program:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Mengambil data dari array</title>
</head>
<body>
    <script>
        // membuat array
        var products = ["Senter", "Radio", "Antena", "Obeng"];

        // mengambil radio
        document.write(products[1]);
    </script>
</body>
</html>
```

Hasilnya:

![Mengambil data dari array](https://www.petanikode.com/img/js/array/ambil-data.png)

## Mencetak isi Array dengan Perulangan

Kita bisa saja mencetak semua isi array satu-per-satu seperti ini:

```javascript
document.write(products[0]);
document.write(products[1]);
document.write(products[2]);
document.write(products[3]);
document.write(products[4]);
```

Bagaimana kalau nanti isi array-nya ada `100`?

Tentu kita tidak akan mau menulis `100` baris kode untuk mencetak array.

Solusinya: [**Gunakan perulangan**](https://www.petanikode.com/javascript-perulangan/).

Mari kita lihat contohnya:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Array dan perulangan</title>
</head>
<body>
    <script>
        // membuat array
        var products = ["Senter", "Radio", "Antena", "Obeng"];

        document.write("<h3>Daftar Produk:</h3>");
        document.write("<ol>");
        // menggunakan perulangan untuk mencetak semua isi array
        for(let i = 0; i < products.length; i++){
            document.write(`<li>${ products[i] }</li>`);
        }
        document.write("</ol>");
    </script>
</body>
</html>
```

Hasilnya:

![Menggunakan perulangan untuk mencetak semua isi array](https://www.petanikode.com/img/js/array/perulangan.png)

Perhatikan…

Pada contoh di atas, kita menggunakan properti `length` untuk mengambil panjang array.

Kita memiliki `4` data di dalam array `products`, maka properti `length` akan bernilai `4`.

Lalu kita gunakan properti ini untuk membatasi jumlah perulangan di dalam _for_.

```javascript
for(let i = 0; i < products.length; i++){
    document.write(`<li>${ products[i] }</li>`);
}
```

…dan di dalam blok for, kita mencetak isi produk dengan indeks yang mengacu pada variabel `i`.

Cara lain:

Kita bisa menggunakan perulangan dengan method `forEach()`.

Contoh:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Array dan perulangan</title>
</head>
<body>
    <script>
        // membuat array
        var products = ["Senter", "Radio", "Antena", "Obeng"];

        document.write("<h3>Daftar Produk:</h3>");
        document.write("<ol>");
        // menggunakan perulangan untuk mencetak semua isi array
        products.forEach((data) => {
            document.write(`<li>${data}</li>`);
        });
        document.write("</ol>");
    </script>
</body>
</html>
```

Hasilnya akan sama seperti di atas.

![Perulangan array dengan method forEach()](https://www.petanikode.com/img/js/array/perulangan.png)

## Cara Menambahkan Data ke Dalam Array

Ada dua cara yang bisa dilakukan untuk menambah data ke dalam array:

1. Mengisi menggunakan indeks;
2. Mengisi menggunakan method `push()`.

Mengisi dengan indeks maksudnya begini…

Misal kita punya array dengan isi sebagai berikut:

```javascript
var buah = ["Apel", "Jeruk", "Manggis"];
```

Terdapat tiga data di dalam array `buah` dengan indeks:

- `0`: `"Apel"`
- `1`: `"Jeruk"`
- `2`: `"Manggis"`

Kita ingin menambahkan data lagi pada indeks ke-`3`, maka kita bisa melakukannya seperti ini:

```javascript
buah[3] = "Semangka";
```

Sekarang array `buah` akan berisi `4` data.

Mari kita coba pada _console_ Javascript.

![Menambahkan data ke dalam array](https://www.petanikode.com/img/js/array/add-data.png)

Benar kan…

`"Semangka"` berhasil kita tambahkan ke dalam array `buah`.

Tapi kekurangan dari cara ini ialah:

Kita **harus tahu** jumlah data atau panjang array-nya, barulah kita bisa menambahkan.

Apabila kita memasukkan nomer indeks sembarangan, maka nanti yang akan terjadi adalah data yang ada di dalam indeks tersebut akan ditindih.

Lalu solusinya bagaimana donk?

Kita gunakan method `push()`.

Kita tidak perlu tahu berapa panjang array-nya, karena method `push()` akan menambahkan data ke dalam array dari ekor atau belakang.

Contoh:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Mengisi data ke array</title>
</head>
<body>
    <script>
        // membuat array
        var products = ["Senter", "Radio", "Antena", "Obeng"];

        // menambahkan tv ke dalam array products
        products.push("Televisi");

        // menampilkan isi array
        document.write(products);
    </script>
</body>
</html>
```

Maka hasilnya:

![Memabahkan data dengan method push](https://www.petanikode.com/img/js/array/add-data-array.png)

Kita juga bisa menambahkan beberapa data sekaligus dengan cara seperti ini:

```javascript
products.push("Alarm", "Gembok", "Paku");
```

## Cara Menghapus Data Array

Sama seperti menambahkan data ke array, menghapus data juga memiliki dua cara:

1. Menggunakan `delete`;
2. Menggunakan method `pop()`.

Contoh:

```javascript
delete buah[2];
```

Kita dapat menghapus data dengan nomer indeks tertentu dengan `delete`. Sedangkan `pop()` akan menghapus dari belakang.

Kekurangan dari `delete`, ia akan menciptakan ruang kosong di dalam array.

Percobaan di dalam _console_:

![Menghapus data dengan delete](https://www.petanikode.com/img/js/array/delete.png)

Tentu ini kurang bagus…

…karena array akan tetap memiliki panjang `4`.

Cara kedua menggunakan method `pop()`, kebalikan dari method `push()`.

Method `pop()` akan menghapus array yang ada di paling belakang.

Array pada javascript dapat kita pandang sebagai sebuah _stack_ (tumpukan), yang mana memiliki sifat _LILO (Last in Last out)_.

![Stack dalam Javascript](https://www.petanikode.com/img/js/array/stack.png)

Mari kita coba di dalam _console_.

![Fungsi pop pada javascript](https://www.petanikode.com/img/js/array/pop.png)

Kita memanggil method `pop()` sebanyak `4` kali, maka array-nya akan kosong `[]`. Karena isinya hanya `4` saja.

Method `pop()` akan mengembalikan nilai item atau data yang terhapus dari array.

### Menghapus Data dari Depan

Kita juga dapat menghapus data dari depan dengan menggunakan method `shift()`.

Contoh:

```javascript
var bunga = ["Mawar", "Melati", "Anggrek", "Sakura"];

// hapus data dari depan
bunga.shift();
```

Maka data yang terhapus adalah `"Mawar"`.

Percobaan pada console:

### Menghapus Data pada Indeks Tertentu

Apabila kita ingin menghapus data pada indeks tertentu, maka fungsi atau method yang digunakan adalah `splice()`.

Fungsi ini memiliki dua parameter yang harus diberikan:

```javascript
array.splice(<indeks>, <total>);
```

Keterangan:

- `<indeks>` adalah indeks dari data di dalam array yang akan dihapus;
- `<total>` adalah jumlah data yang akan dihapus dari indeks tersebut.

Biasanya kita berikan nilai total dengan nilai `1` agar hanya menghapus satu data saja.

Contoh:

```javascript
var bunga = ["Mawar", "Melati", "Anggrek", "Sakura"];

// hapus Anggrek
bunga.splice(2, 1);
```

Percobaan pada _console_:

![Menghapus data pada indeks tertentu](https://www.petanikode.com/img/js/array/splice.png)

Pada percobaan di atas, apabila kita tidak mengisi `<total>` data yang akan dihapus, maka semua data dari indeks yang terpilih akan dihapus.

## Mengubah isi Array

Untuk mengubah isi array, kita bisa mengisi ulang seperti ini:

```javascript
var bahasa = ["Javascript", "Kotlin", "Java", "PHP", "Python"];
bahasa[1] = "C++";
```

Maka `"Kotlin"` akan diganti dengan `"C++"`.

Percobaan pada _console_:

![Ubah data pada array](https://www.petanikode.com/img/js/array/update.png)

Sangat mudah bukan…

## Method-method penting pada Array

Selain method-method atau fungsi yang sudah kita coba di atas, terdapat beberapa method dalam Array yang perlu kita ketahui.

### 1. Method `filter()`

Method `filter()` berfungsi untuk menyaring data dari array.

Parameter yang harus diberikan pada method `filter()` sama seperti method `forEach()`, yaitu: sebuah fungsi _callback_.

Contoh:

```javascript
const angka = [1, 2, 3, 4, 5, 6, 7, 8, 9];

// Kita ambil data yang hanya habis dibagi dua saja
const filteredArray = angka.filter((item) => {return item % 2 === 0});

console.log(filteredArray) // -> [2, 4, 6, 8]
```

Pada contoh di atas, kita memberikan _arrow function_ sebagai fungsi callback yang akan melakukan penyaringan terhadap array.

Sebenarnya kita bisa buat lebih sederhana lagi seperti ini:

```javascript
const filteredArray = angka.filter(item => item % 2 === 0);
```

### 2. Method `includes()`

Method ini berfungsi untuk mengecek apakah sebuah data ada di dalam array atau tidak. Biasanya digunakan untuk melakukan pencarian untuk memastikan data sudah ada di dalam array.

Contoh:

```javascript
var tanaman = ["Padi", "Kacang", "Jagung", "Kedelai"];

// apakah kacang sudah ada di dalam array tanaman?
var adaKacang = tanaman.includes("Kacang");

console.log(adaKacang); // -> true

// apakah bayam ada?
var adaBayam = tanaman.includes("Bayam");

console.log(adaBayam); // -> false
```

### 3. Method `sort()`

Method `sort()` berfungsi untuk mengurutkan data pada array.

Contoh:

```javascript
var alfabet = ['a','f','z','e','r','g'];
var angka = [3,1,2,6,8,5];

console.log(alfabet.sort()); //->  ["a", "e", "f", "g", "r", "z"]
console.log(angka.sort()); // -> [1, 2, 3, 4, 5, 6, 7, 8, 9]
```

## Apa Selanjutnya?

Kita sudah belajar tentang dasar-dasar array pada javascript, seperti membuat array, menambahkan data pada array, mengubah data pada array, menghapus data pada array, dan juga method-method yang biasa digunakan pada array.

Masih banyak lagi method-method yang belum kita coba.

Saran saya:

Sering-seringlah berlatih.

Gunakan _console_ Javascript untuk mencoba-coba method yang ada pada Array.

![Method pada array](https://www.petanikode.com/img/js/array/method.png)

Selanjutnya kita akan belajar tentang fungsi pada Javascript untuk membuat program yang lebih terstruktur. Serta di sana kita akan membuat aplikasi dengan menggunakan array sebagai penyimpanan datanya.

## Apa itu Fungsi?

Fungsi adalah sub-program yang bisa digunakan kembali baik di dalam program itu sendiri, maupun di program yang lain.

Fungsi di dalam Javascript adalah sebuah objek. Karena memiliki properti dan juga _method_.

Bagi pemula konsep ini cukup membingungkan. Apalagi yang belum mengenal konsep [OOP](https://www.petanikode.com/topik/oop/).

Tapi tentang saja…

Kita pelajari dulu tentang fungsi, nanti saya akan bahas tentang objek di kesempatan yang berbeda.

## 4 Cara Membuat Fungsi di Javascript

Ada 4 cara yang bisa kita lakukan untuk membuat fungsi di Javascript:

1. Menggunakan cara biasa;
2. Menggunakan ekspresi;
3. Menggunakan tanda panah (`=>`);
4. dan menggunakan _Constructor_.

Mari kita coba semuanya…

### 1. Membuat Fungsi dengan Cara Biasa

Cara ini paling sering digunakan, terutama buat yang baru belajar Javascript.

```javascript
function namaFungsi(){
    console.log("Hello World!");
}
```

### 2. Membuat Fungsi dengan Ekspresi

Cara membuat fungsi dengan ekspresi:

```javascript
var namaFungsi = function(){
    console.log("Hello World!");
}
```

Kita menggunakan variabel, lalu diisi dengan fungsi. Fungsi ini sebenarnya adalah fungsi anonim _(anonymous function)_ atau fungsi tanpa nama.

### 3. Membuat Fungsi dengan Tanda Panah

Cara ini sering digunakan di kode Javascript masa kini, karena lebih sederhana. Akan tetapi sulit dipahami bagi pemula. Fungsi ini mulai muncul pada standar ES6.

Contoh:

```javascript
var namaFungsi = () => {
    console.log("Hello World!");
}

// atau seperti ini (jika isi fungsi hanya satu baris):
var namaFungsi = () => console.log("Hello World!");
```

Sebenarnya hampir sama dengan yang menggunakan ekspresi. Bedanya, kita menggunakan tanda panah (`=>`) sebagai ganti `function`.

Pembuatan fungsi dengan cara ini disebut _arrow function_.

### 4. Membuat Fungsi dengan Kostruktor

Cara ini sebenarnya tidak direkomendasikan oleh [Developer Mozilla](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions), karena terlihat kurang bagus. Soalnya _body_ fungsinya dibuat dalam bentuk string yang dapat mempengaruhi kinerja _engine_ javascript.

Contoh:

```javascript
var namaFungsi = new Function('console.log("Hello World!");');
```

Untuk yang masih pemula, saya rekomendasikan gunakan cara yang pertama dulu. Nanti kalau sudah terbiasa baru coba gunakan cara ke-2 dan ke-3.

## Cara Memanggil/Eksekusi Fungsi

Setelah mengetahui cara membuat fungsi, lalu bagaimana cara memanggilnya?

Kita bisa memanggil fungsi di dalam kode Javascript dengan menuliskan nama fungsinya seperti ini:

```javascript
namaFungsi();
```

Contoh:

```javascript
// membuat fungsi
function sayHello(){
    console.log("Hello World!");
}

// memanggil fungsi
sayHello() // maka akan menghasilkan -> Hello World!
```

Selain dengan cara di atas, kita juga bisa memanggil fungsi melalui atribut _event_ pada HTML.

Contoh:

```html
<!DOCTYPE html>
<html>
<head>
    <script>
    // membuat fungsi
    var sayHello = () => alert("Hello World!");
    </script>
</head>
<body>
    <!-- Memanggil fungsi saat link diklik -->
    <a href="#" onclick="sayHello()">Klik Aku!</a>
</body>
</html>
```

Hasilnya:

![Eksekusi Fungsi](https://www.petanikode.com/img/js/fungsi/eksekusi-fungsi.png)

## Fungsi dengan Parameter

Parameter adalah variabel yang menyimpan nilai untuk diproses di dalam fungsi.

Contoh:

```javascript
function kali(a, b){
    hasilKali = a * b;
    console.log("Hasil kali a*b = " + hasilKali);
}
```

Pada contoh di atas, `a` dan `b` adalah sebuah parameter.

Lalu cara memanggil fungsi yang memiliki parameter adalah seperti ini:

```javascript
kali(3, 2); // -> Hasil kali a*b = 6
```

Kita memberikan `3` untuk parameter `a` dan `2` untuk parameter `b`.

## Fungsi yang Mengembalikan Nilai

Agar hasil pengolahan nilai di dalam fungsi dapat digunakan untuk proses berikutnya, maka fungsi harus mengembalikan nilai.

Pengembalian nilai pada fungsi menggunakan kata kunci `return` kemudian diikuti dengan nilai atau variabel yang akan dikembalikan. Contoh:

```javascript
function bagi(a,b){
    hasilBagi = a / b;
    return hasilBagi;
}

// memanggil fungsi
var nilai1 = 20;
var nilai2 = 5;
var hasilPembagian = bagi(nilai1, nilai2);

console.log(hasilPembagian); //-> 4
```

## Contoh Program Javascript dengan Fungsi

Setelah kita paham dasar-dasar pembuatan fungsi dan jenis-jenisnya, sekarang mari kita coba membuat program sederhana.

Program ini berisi CRUD _(Crete, Read, Update, Delete)_ data barang yang tersimpan dalam sebuah array.

Silahkan buat dua file baru:

```bash
js-fungsi/
├── fungsi.js
└── index.html
```

File `index.html` adalah file yang menampilkan halaman web. Sedangkan file `fungsi.js` adalah programnya.

Berikut ini isi file `index.html`:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Belajar Fungsi di Javascript</title>
</head>
<body>
    
    <fieldset>
        <legend>Input Form</legend>
        <input type="text" name="barang" placeholder="input nama barang..." />
        <input type="button" onclick="addBarang()" value="Tambah" />
    </fieldset>

    <div>
        <ul id="list-barang">
        </ul>
    </div>

    <script src="fungsi.js"></script>
</body>
</html>
```

Berikutnya kita akan buat kode di file `fungsi.js`. Silahkan gunakan gaya pembuatan fungsi yang kamu sukai.

Pada contoh ini, kita akan menggunakan cara yang pertama. Karena lebih mudah.

Berikut ini isi file `fungsi.js`:

```javascript
var dataBarang = [
    "Buku Tulis",
    "Pensil",
    "Spidol"
];


function showBarang(){
    var listBarang = document.getElementById("list-barang");
    // clear list barang
    listBarang.innerHTML = "";

    // cetak semua barang
    for(let i = 0; i < dataBarang.length; i++){
        var btnEdit = "<a href='#' onclick='editBarang("+i+")'>Edit</a>";
        var btnHapus = "<a href='#' onclick='deleteBarang("+i+")'>Hapus</a>";

        listBarang.innerHTML += "<li>" + dataBarang[i] + " ["+btnEdit + " | "+ btnHapus +"]</li>";        
    }
}

function addBarang(){
    var input = document.querySelector("input[name=barang]");
    dataBarang.push(input.value);
    showBarang();
}

function editBarang(id){
    var newBarang = prompt("Nama baru", dataBarang[id]);
    dataBarang[id] = newBarang;
    showBarang();
}

function deleteBarang(id){
    dataBarang.splice(id, 1);
    showBarang();
}

showBarang();
```

Hasilnya:

![Program fungsi dengan javascript](https://www.petanikode.com/img/js/fungsi/demo-program.png)

## Akhir Kata…

Fungsi merupakan hal yang wajib dipahami di dalam Javascript, karena kedepan kita akan banyak bekerja dengan fungsi baik dalam membuat objek, manipulasi HTML, melakukan ajax dan sebagainya.

Tulisan ini hanya mengajari dasar-dasar saja. Sebenarnya masih banyak lagi hal yang harus dibahas tentang fungsi.


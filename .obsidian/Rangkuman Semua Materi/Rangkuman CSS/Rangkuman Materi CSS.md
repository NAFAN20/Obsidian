## Anatomi CSS

![gambar](AsetRangkumanCSS/Anatomi.jpg)
### Selector
Selector CSS di gunakan untuk memilih elemen HTML yang akan diberi gaya.Dengan menggunakan selector, Anda dapat menargetkan satu atau lebih elemen HTML untuk menerapkan properti CSS.
### Property

Property dalam CSS adalah karakteristik atau gaya yang diterapkan pada elemen HTML, seperti warna, ukuran font, atau margin. Properti bekerja dengan selector untuk mengatur tata letak dan penampilan elemen
### Property value
Dalam CSS property value (nilai sifat) merujuk pada nilai konkret yang diberikan kepada suatu properti.
## Percobaan I
### Kode Program
```html
<!DOCTYPE html>
<html>
    <head>
        <title>Belajar CSS 1</title>
        <style>
            p {
                color: red;
            }
        </style>
    </head>
    <body>
        <p>Welcome CSS</p>
    </body>
</html>
```
## Hasil
![gambar](AsetRangkumanCSS/Asset2CSS.png)

Penjelasan
- Jenis dokumen HTML yang digunakan (HTML5).
- Elemen utama yang memuat seluruh konten dokumen.
- Bagian dengan informasi tambahan seperti judul dan link stylesheet.
- `<title>`: Menentukan judul halaman web di tab browser.
- `<style>`: Bagian untuk aturan CSS mengubah tampilan elemen HTML.
- `p { color: red; }`: Aturan CSS untuk warna teks merah pada semua `<p>`.
- Bagian dengan konten utama halaman web seperti teks dan gambar.
- `Welcome CSS`: Elemen paragraf "Welcome CSS" dengan teks merah.

---

## Percobaan II 

Dengan aturan CSS ini, setiap elemen `<button>` dalam dokumen HTML akan memiliki lebar 150 piksel, tinggi 50 piksel, teks berwarna putih dengan ukuran 20 piksel, dan teks tersebut akan sejajar ke kanan di dalam tombol.
### Kode Program
```css
button{         
width: 150px;             
height: 50px;               
color: white;               
font-size: 20px;              
text-align: right;        
}
```

### Hasil

Before
![gambar](AsetRangkumanCSS/Asset4CSS.png)
After
![gambar](AsetRangkumanCSS/Asset3CSS.png)

### Penjelasan
- `width: 150px;` : Mengatur lebar tombol menjadi 150 piksel.
- `height: 50px;` : Mengatur tinggi tombol menjadi 50 piksel.
- `color: white;` : Mengatur warna teks tombol menjadi putih.
- `font-size: 20px;` : Mengatur ukuran teks tombol menjadi 20 piksel.
- `text-align: right;` : Mengatur teks tombol sejajar ke kanan.

---
## Font
### Font-size

Aturan CSS di bawah mengatur ukuran font dari elemen HTML `<p>` menjadi 100 piksel.
#### Kode Program
```css
p{ 
font-size: 100px; 
}
```

#### Hasil
![gambar](AsetRangkumanCSS/Asset22CSS.png)

#### Penjelasan 

- `p`: Selector CSS yang memilih semua elemen `<p>` (paragraf) di halaman HTML.
- `{ ... }`: Kurung kurawal yang membungkus aturan CSS yang berlaku untuk elemen yang dipilih.
- `font-size: 100px;`: Deklarasi properti CSS yang mengatur ukuran font teks dalam elemen `<p>` menjadi 100 piksel.
---
## Text
### Text Align

CSS di bawah adalah aturan yang mengatur penempatan teks ke tengah (center) pada elemen HTML `<p>`, yaitu paragraf.

#### Kode Program
```css
p{
Text-align: center;
}
```

#### Hasil
![gambar](AsetRangkumanCSS/Asset10CSS.png)

#### Penjelasan
- `p`: Selector CSS yang memilih semua elemen `<p>` (paragraf) di halaman HTML.
- `{ ... }`: Kurung kurawal yang membungkus aturan CSS yang berlaku untuk elemen yang dipilih.
- `text-align: center;`: Deklarasi properti CSS yang mengatur teks dalam elemen `<p>` agar diratakan ke tengah (center).

---
## Background 

### Background-image 

CSS di bawah adalah aturan yang mendefinisikan gaya untuk elemen HTML `<p>`. Aturan ini menggunakan sebuah gambar sebagai latar belakang untuk elemen `<p>`.
#### Kode Program
```css
p{ 
background-image: url("aset/nafan.png");
}
```

#### Hasil
![gambar](AsetRangkumanCSS/Asset17CSS.png)

#### Penjelasan

- `p`: Selector CSS yang memilih semua elemen `<p>` (paragraf) di halaman HTML.
- `{ ... }`: Kurung kurawal yang membungkus aturan CSS yang berlaku untuk elemen yang dipilih.
- `background-image: url("aset/nafan.png");`: Deklarasi properti CSS yang mengatur gambar latar belakang elemen `<p>` menggunakan gambar yang terdapat pada path `"aset/nafan.png"`.
---
## Border

### Border Color

CSS di bawah adalah sebuah aturan yang mendefinisikan gaya untuk elemen HTML `<button>`. Aturan ini mengatur warna border (bingkai) dari elemen `<button>` menjadi oranye kemerahan (`orangered`).
#### Kode Program
```css
button{ 
border-color: orangered;
}
```

#### Hasil
![gambar](AsetRangkumanCSS/Asset26CSS.png)

#### Penjelasan
mengubah warna bingkai (border) tombol `<button>` menjadi oranye kemerahan (`orangered`).

---
## Padding

### Padding Left

Aturan CSS di atas mengatur jarak (padding) di sebelah kiri dari elemen HTML `<button>` menjadi 29 piksel.
#### Kode Program
```css
button{  
padding-left: 29px; 
}
```

#### Hasil
![gambar](AsetRangkumanCSS/Asset27CSS.png)

#### Penjelasan
- **Selector**: `button` - Menetapkan elemen HTML `<button>` sebagai target aturan CSS ini.
- **Property**: `padding-left` - Mengontrol jarak (padding) dari sisi kiri elemen.
- **Value**: `29px` - Menyatakan bahwa jarak (padding) di sisi kiri dari elemen `<button>` diatur sebesar 29 piksel.
---
## Margin

### Margin Left

Aturan CSS di bawah mengatur jarak (margin) di sebelah kiri dari elemen HTML `<button>` menjadi 600 piksel.
#### Kode Program
```css
button{
margin-left: 600px;
}
```

#### Hasil
![gambar](AsetRangkumanCSS/Asset31CSS.png)

#### Penjelasan 
- **Selector**: `button` - Menetapkan elemen HTML `<button>` sebagai target aturan CSS ini.
- **Property**: `margin-left` - Mengontrol jarak (margin) dari sisi kiri elemen.
- **Value**: `600px` - Menyatakan bahwa jarak (margin) di sisi kiri dari elemen `<button>` diatur sebesar 600 piksel.

---
## Background Color
CSS di bawah adalah aturan yang akan diterapkan pada elemen `<button>` ketika tombol tersebut sedang dalam keadaan "hover" (saat kursor mouse mengarah ke atasnya).

```css
button:hover{ 

background-color:red; 
color:white; 
height:100px;
width:100px;

}
```

Hasil
![gambar](AsetRangkumanCSS/Asset36CSS.png)

#### Penjelasan
- **Selector**: `button:hover` - Mengenali elemen `<button>` saat kursor mouse mengarah ke atasnya (hover).
- **Properties**:
    - `background-color: red;` - Mengubah warna latar belakang tombol menjadi merah saat dihover.
    - `color: white;` - Mengubah warna teks di dalam tombol menjadi putih saat dihover.
    - `height: 100px;` - Menetapkan tinggi tombol menjadi 100 piksel saat dihover.
    - `width: 100px;` - Menetapkan lebar tombol menjadi 100 piksel saat dihover.

---
## Transition

CSS di bawah adalah aturan yang akan mengubah tampilan tombol `<button>` ketika tombol tersebut sedang dalam keadaan "hover" (saat kursor mouse mengarah ke atasnya). Selain itu, aturan ini juga menambahkan efek transisi pada perubahan properti.
### Kode Program
```css
button:hover{
background-color:red;
color:white;
height:100px; 
width:100px; 
transition:all 0.9s ease-in; 
}
```

### Hasil
![gambar](AsetRangkumanCSS/Asset38CSS.png)

### Penjelasan 

- `background-color: red;` - Mengubah latar belakang tombol menjadi merah saat dihover.
- `color: white;` - Mengubah warna teks di dalam tombol menjadi putih saat dihover.
- `height: 100px;` - Menetapkan tinggi tombol menjadi 100 piksel saat dihover.
- `width: 100px;` - Menetapkan lebar tombol menjadi 100 piksel saat dihover.
- `transition: all 0.9s ease-in;` - Menambahkan efek transisi untuk semua perubahan properti tombol, dengan durasi 0.9 detik dan efek "ease-in" (perubahan lambat di awal dan cepat di akhir).
---
## Transform

CSS di bawah adalah aturan yang akan mengubah transformasi (transform) dari elemen `<button>` ketika tombol tersebut sedang dalam keadaan "hover" (saat kursor mouse mengarah ke atasnya).
### Kode Program
```css
button:hover{
transform:matrix(0.7,-0.5,0.5,0.4,0.5,0.7);
}
```

Hasil
![gambar](AsetRangkumanCSS/Asset39CSS.png)

### Penjelasan
- **Selector**: `button:hover` - Mengubah tampilan elemen `<button>` saat kursor mouse mengarah ke atasnya (hover).
- **Property**: `transform` - Digunakan untuk melakukan transformasi seperti rotasi, scaling, skewing, dan pemindahan (translation) terhadap elemen.
- **Value**: `matrix(0.7, -0.5, 0.5, 0.4, 0.5, 0.7)` - Menerapkan transformasi matriks khusus ke elemen `<button>`, termasuk scaling (0.7), rotasi, dan skewing (pemiringan).

---
## Flex Direction

CSS di bawah adalah aturan yang mempengaruhi tata letak dari sebuah container yang menggunakan Flexbox dengan class `box-container`. Aturan ini mengubah arah tata letak dari defaultnya menjadi kolom (top to bottom).
### Kode program
```css
    .box-container{ 
    flex-direction: column; 
    }
```

### Hasil
![gambar](AsetRangkumanCSS/Asset40CSS.png)

### Penjelasan 
- **Selector**: `.box-container` - Menargetkan elemen dengan class `box-container`. Elemen ini menggunakan Flexbox untuk mengatur tata letak anak-anaknya.
- **Property**: `flex-direction` - Properti CSS dalam Flexbox yang menentukan arah tata letak dari elemen-elemen flex di dalam container.
- **Value**: `column` - Nilai dari properti `flex-direction`, yang mengatur agar anak-anak dari `.box-container` disusun dalam satu kolom dari atas ke bawah.
---
## Align-items

CSS di bawah adalah aturan yang mengatur penempatan vertikal dari elemen-elemen di dalam sebuah container dengan class `.box-container` menggunakan Flexbox.
### Kode Program
```css
.box-container{
align-items:center ;
}
```

### Hasil
![gambar](AsetRangkumanCSS/Asset41CSS.png)

### Penjelasan
- **Selector**: `.box-container` - Menargetkan elemen dengan class `box-container`, mempengaruhi tampilan anak-anaknya.
- **Property**: `align-items` - Properti Flexbox untuk menengahkan elemen flex secara vertikal di dalam container.
- **Value**: `center` - Nilai yang menengahkan (center) anak-anak dari `.box-container` secara vertikal.
---
## Justify-contet

CSS di bawah adalah aturan yang mengatur penempatan horizontal dari elemen-elemen di dalam sebuah container dengan class `.box-container` menggunakan Flexbox.
```css
.box-container{ 
justify-content: center ; 
}
```

Hasil
![gambar](AsetRangkumanCSS/Asset42CSS.png)

### Penjelasan
- **Selector**: `.box-container` - Menargetkan elemen dengan class `box-container`, mempengaruhi tampilan anak-anaknya.
- **Property**: `justify-content` - Properti Flexbox untuk menengahkan elemen flex secara horizontal di dalam container.
- **Value**: `center` - Nilai yang menengahkan (center) anak-anak dari `.box-container` secara horizontal.

---
## Position

CSS di bawah adalah aturan yang akan memengaruhi tampilan dari elemen dengan class 
`box-1`. Berikut adalah penjelasan singkatnya:

### Kode Program
```css
box-1{ 
background-color:aqua;
position:relative;
top:20px; 
left:30px;
}
```

### Hasil
![gambar](AsetRangkumanCSS/Asset47CSS.png)

### Penjelasan 

- `background-color: aqua;` - Latar belakang elemen diubah menjadi aqua.
- `position: relative;` - Posisi elemen disesuaikan relatif terhadap posisi normal.
- `top: 20px;` - Geser elemen 20 piksel ke bawah dari posisi normal.
- `left: 30px;` - Geser elemen 30 piksel ke kanan dari posisi normal.
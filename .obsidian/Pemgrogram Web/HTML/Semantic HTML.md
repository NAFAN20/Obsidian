# Apa itu Semantic HTML
Semantic HTML adalah konsep dalam pengembangan web yang berfungsi menyediakan makna atau arti lebih dalam kode HTML.

Dalam semantic HTML, masing-masing elemen memiliki nama yang mencerminkan arti dari kontennya, bukan hanya presentasinya. Semantic membantu mesin pencari dan perangkat pembaca layar (screen reader) untuk memahami struktur dan konten dari halaman web dengan lebih maksimal. 

Artinya, jika kamu ingin membuat kode yang mudah dipahami, tidak hanya oleh manusia tapi juga oleh mesin, semantic HTML adalah solusi yang tepat. saya berikan contoh dari gambar berikut.
![[Pasted image 20240506031632.png]]
Mungkin kalian bertanya-tanya, “Apa perbedaan antara semantic HTML dan non-semantic HTML?” 

Perbedaan keduanya cukup sederhana.

Semantic HTML menggunakan elemen yang menggambarkan arti dari konten, seperti

,

, dan

. Sedangkan non-semantic HTML menggunakan elemen seperti

dan yang tidak mengungkapkan informasi apa pun tentang kontennya. Untuk memahami lebih jelas, mari kita lihat contoh kode berikut:

Bukan Semantic

```html
<div id="header"></div>
<div id="sidebar"></div>
<div  class="main">
	<div class="Section">
		<div class="articel">
				<div class="figure">
					<img>
					<div class="figcaption"></div>
				</div>
				
			</div>
			
		</div>
	</div>
<div id="footer"></div>
```

Semantic HTML : 
```css
<header></header>
<main>
	<section>
		<articel>
			<figure>
				<img>
				<figcaption></figcaption>
			</figure>
			
		</articel>
	
	</selection>

</main>
<footer></footer>
```
# Mengapa Menulis Semantic HTML

1. Aksesibilitas 
	Tag HTML yang semantik membantu membuat konten lebih mudah diakses oleh pembaca layar dan perangkat bantu lainnya. Ini meningkatkan pengalaman pengguna untuk orang dengan disabilitas
2. .SEO (Search Engine Optimization): 
	 Mesin pencari, seperti Google, cenderung memberikan peringkat lebih tinggi pada halaman web yang menggunakan Semantic HTML karena struktur yang jelas membantu mesin pencari memahami dan mengindeks konten dengan lebih baik.
3. Mudah Dibaca Pengembang/Developer 
	Penggunaan tag yang memiliki makna membuat kode HTML lebih mudah dibaca dan dimengerti oleh pengembang dan anggota tim lainnya. Ini mempermudah pemeliharaan dan pengembangan kode.
# Jenis Jenis Tag Semantic HTML

Tag semantik dapat mendefinisikan berbagai bagian halaman web. 

Mari kita lihat elemen semantik HTML yang paling umum, dibagi menjadi dua kategori berdasarkan penggunaannya:

* Tag semantik HTML untuk struktur
* Tag semantik HTML untuk teks 
# Tag  Semantic HTML untuk Struktur

Banyak tag HTML semantik mengkomunikasikan tata letak halaman.

Tag "struktural" ini diperkenalkan ketika HTML4 ditingkatkan ke HTML5. Itulah mengapa juga dikenal sebagai tag HTML5 semantik atau elemen HTML5 semantik.

`<Header>`

Tag header mendefinisikan konten yang harus dianggap sebagai informasi pengantar halaman atau bagian

`<nav>`
Tag navigasi digunakan untuk tautan navigasi. Tag ini dapat diletakkan di dalam tag

`<header>` namun tag navigasi sekunder`<nav>`juga biasa digunakan di tempat lain pada halaman.

`<main>`

Tag ini berisi konten utama (juga disebut badan) halaman. Hanya boleh ada satu tag per halaman.

`<section>`
Menggunakan `<section>`  adalah cara untuk  mengelompokkan konten yang  berdekatan dengan tema yang sama tag `<section>` berbeda dengan tag artikel. Tag `<section>`  tidak  selalu sendiri, tetapi merupakan bagian dari sesuatu  yang lain

`<Artikel>`
Tag artikel mendefinisikan konten yang dapat berdiri sendiri terlepas dari halaman atau situs tempat konten tersebut berada. Ini tidak selalu berarti "posting blog". Anggap saja sebagai "sebuah artikel" - sebuah item mandiri yang dapat digunakan dalam berbagai konteks.

`<aside>`
Elemen aside ini sering digunakan untuk bilah sisi-area yang menambahkan informasi pelengkap.

`<aside>`
Elemen `<footer>` juga sering digunakan di bagian bawah halaman. Biasanya mencakup informasi kontak, informasi hak cipta, dan beberapa navigasi situs.

# Tag Semantic HTML Untuk Teks
Tag HTML semantik untuk teks adalah tag HTML yang-selain pemformatan-juga menyampaikan fungsi semantik teks yang dikandungnya.

`<h1 (heading)>`
Tag H1 menandai judul tingkat atas. Biasanya hanya ada satu judul H1 per halaman.

`<p> paragraf`
Paragraf teks yang berdiri sendiri.

`<a> anchor`
Digunakan untuk menandai hyperlink dari satu halaman ke halaman lainnya.

`<ol> daftar terurut`
Daftar item yang ditampilkan dalam urutan tertentu, dimulai dengan poin-poin. Satu tag `<li>`
(item daftar) berisi satu item dalam daftar

`<ul> daftar tidak berurutan`
Daftar item yang tidak perlu ditampilkan dalam urutan tertentu, dimulai dengan nomor urut. Satu tag `<li>`(item daftar) berisi satu item dalam daftar.

`<q> / <blockqoute>`
Kutipan teks. Gunakan `<blockqoute>`untuk kutipan panjang dengan banyak baris dan`<q>` untuk kutipan pendek dan sejajar.

`<em>`
Digunakan untuk teks yang harus ditekankan.

`<strong>`
Digunakan untuk teks yang harus diberi penekanan kuat.

`<code>`
Blok kode computer.

Disini saya hanya mencantumkan beberapa tag HTML semantik yang paling umum. Anda dapat menggunakan banyak lainnya seperti `<summary>`, `<time>`, `<addres>`, `<video>`  dll. untuk membuat konten situs web Anda lebih mudah dipahami. Untuk menemukan lebih banyak elemen semantik HTML, lihat pada web berikut https://developer.mozilla.org/en-US/docs/Glossary/Semantics

# Tips & Best Practices Semantic HTML
mari kita bahas beberapa tips penerapan HTML berdasarkan kesalahan umum yang dilakukan orang saat menggunakan tag HTML semantic.
# Jangan Gunakan Tag Semantic HTML Untuk Styling
Meskipun browser web menerapkan styling pada banyak tag semantik (misalnya, teks dalam tag  `<a>`biasanya berwarna biru dan bergaris bawah), bukan berarti tag HTML seharusnya digunakan untuk menata gaya teks Anda.

Dengan kata lain, sama seperti Anda tidak akan menggunakan tag`<a>` untuk teks “non-link” hanya untuk membuatnya berwarna biru dan bergaris bawah, Anda juga tidak boleh menggunakan tag semantik lain hanya untuk tujuan gaya.

Berikut beberapa contoh umum penggunaan tag semantik yang salah:

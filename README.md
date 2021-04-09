# lab2wab
1.	Persiapkan text editor misalnya VSCode. 
2.	Buat file baru dengan nama lab2_css_dasar.html 
3.	Buat struktur dasar dari dokumen HTML. 
4.	Ikuti langkah-langkah praktikum yang akan dijelaskan berikutnya. 

a. Membuat dokumen HTML 
Buatlah dokumen HTML seperti berikut
saya sudah screenshoot langsung file vs code  nya dengan firefox seperti berikut:
 
![1 0](https://user-images.githubusercontent.com/56192368/114229383-f4285380-99a1-11eb-8cf5-9be802898f99.png)

b. Mendeklarasikan CSS Internal 
Kemudian tambahkan deklarasi CSS internal seperti berikut pada bagian head dokumen. 

![1 1](https://user-images.githubusercontent.com/56192368/114230128-f3dc8800-99a2-11eb-9736-f97b55d0f617.JPG)

c. Menambahkan Inline CSS 
Kemudian tambahkan deklarasi inline CSS pada tag <p> seperti berikut. 
|<p style="text-align: center; color: #ccd8e4;">|
  
Simpan kembali dan refresh kembali browser untuk melihat perubahannya.

![1 3](https://user-images.githubusercontent.com/56192368/114230425-52096b00-99a3-11eb-80f4-6454a003d21b.JPG)


d. Membuat CSS Eksternal 
Buatlah file baru dengan nama style_eksternal.css kemudian buatlah deklarasi CSS seperti berikut. 

(nav { 
    background: #20A759;    
    color:#fff;     
    padding: 10px; 
} 
nav a {     
color: #fff;     
text-decoration: 
none;     
padding:10px 20px; 
} 
nav .active,  nav a:hover { 
    background: #0B6B3A; 
} ) 


Kemudian tambahkan tag <link> untuk merujuk file css yang sudah dibuat pada bagian <head> :
  
(<head> 
    <!-- menyisipkan css eksternal --> 
    <link rel="stylesheet" href="style_eksternal.css" type="text/css"> 
</head> )

Selanjutnya refresh kembali browser untuk melihat perubahannya

![2 0](https://user-images.githubusercontent.com/56192368/114230883-e07dec80-99a3-11eb-8356-22729f868153.JPG)


e. Menambahkan CSS Selector 
Selanjutnya menambahkan CSS Selector menggunakan ID dan Class Selector. Pada file style_eksternal.css, tambahkan kode berikut. 

(/* ID Selector */ 
#intro { 
    background: #418fb1;    
    border: 1px solid #099249;     
    min-height: 100px;     padding: 10px; 
} 
#intro h1 {     
    text-align: left;     
    border: 0;     
    color: #fff; 
} 
 
/* Class Selector */ 
.button { 
    padding: 15px 20px;    
    background: #bebcbd;     
    color: 
    #fff;     
    display: 
    inline-block;     
    margin: 10px; 
    text-decoration: none; 
} 
.btn-primary { 
    background: #E42A42; 
} )
 

Kemudian simpan kembali dan refresh browser untuk melihat perubahannya. 


![2 1](https://user-images.githubusercontent.com/56192368/114231033-191dc600-99a4-11eb-8bd2-d6546deaa9b3.JPG)




Pertanyaan dan Tugas 
1.	Lakukan eksperimen dengan mengubah dan menambah properti dan nilai pada kode CSS dengan mengacu pada CSS Cheat Sheet yang diberikan pada file terpisah dari modul ini. 
jawaban:
saya merubah properti coler pada css dengan perubahan

(h1 { 
            font-size: 24px;             
            color: #343438;             
            text-align: center;             
            padding: 20px 10px; 
        }         
        h1 i { 
            color:#f70a59;)
            
dan hasil refresh nya dibuka di browsur:


![1 1](https://user-images.githubusercontent.com/56192368/114233597-c940fe00-99a7-11eb-9771-24654c800811.JPG)



2.	Apa perbedaan pendeklarasian CSS elemen h1 {...} dengan #intro h1 {...}? berikan penjelasannya! 
jawaban:
perbedaan antara CSS elemen h1 {...} dengan #intro h1 {...} adalah:
elemen h1 merupakan sebuah perintah untuk penulisan judul dalam sebuah file dokumen html sedangkanuntuk pemanggilan #intro h1 {...}ini adalah untuk menyeleksi elemen berdasarkan id tertentu tersebut


3.	Apabila ada deklarasi CSS secara internal, lalu ditambahkan CSS eksternal dan inline CSS pada elemen yang sama. Deklarasi manakah yang akan ditampilkan pada browser? Berikan penjelasan dan contohnya! 
jawaban:
deklarassi yang akan muncul pada browser adalah deklarasi menggunakan inline style pada salah satu elemen saja seperti contoh

(style="text-align: center; color: #ccd8e4;">Kami sedang belajar HTML dan CSS dasar, pada mata kuliah <b>Pemrograman Web</b> di <i>Universitas Pelita Bangsa</i>. Pelajaran pertama yang kami dapat adalah membuat tampilan web sederhana dalam rangka mengenal tag-tag dasar HTML dan CSS.</p>

maka perubahan style nya hanya terdapat pada elemen tersebut


4.	Pada sebuah elemen HTML terdapat ID dan Class, apabila masing-masing selector tersebut terdapat deklarasi CSS, maka deklarasi manakah yang akan ditampilkan pada browser?
 Berikan penjelasan dan contohnya!  ( <p id="paragraf-1" class="text-paragraf"> ) 
 
jawaban:

Keterangan :
Untuk penggunaan Id maka setiap menuliskan code CSS wajib didahului oleh tanda paga (#)
Untuk penggunaan Class maka setiap menuliskan code CSS wajib didahului oleh tanda titik (.)
Seperti contoh di atas
#header   : Id
.intro        : Class

Untuk memunculkan Id gunakan <div id="nama id">
untuk memunculkan class gunakan <p class="nama class">


biasanya id dan class digunakan untuk membagi-bagi bagian antara header footer dan juga sidebar, agar lebih spesifik.

contohnya:

![last](https://user-images.githubusercontent.com/56192368/114241411-49209580-99b3-11eb-882a-02792cba990f.JPG)

sekian dan terimaksih


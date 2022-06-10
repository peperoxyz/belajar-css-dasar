# Belajar CSS Dasar
Resource: MDN Web Docs & others(w3school, freecodecamp, dll)

## Box Dimensions
Cara yang paling banyak digunakan untuk menentukan dimensi kotak pada CSS adalah dengan menggunakan pixel, ems, atau persentase. 
```
       .box {
           height: 300px;
           width: 300px;
           background-color: #11C5C6;
       }
       p {
           height: 75%;
           width: 75%;
           background-color: #FBDD1C;
       }
```
Pada contoh di atas, elemen div memilki dimensi lebar: 300px dan tinggi 300px. Di dalamnya terdapat elemen p dengan ukuran 75% dari lebar dan tinggi elemen induknya : yaitu 225px.

## Limiting Dimension
Bertujuan untuk membuat website responsive(ukuran layout mengukuti ukuran layar pengguna).
1. ```min-width``` : Digunakan untuk menetapkan nilai lebar minimal yang harus dimiliki elemen
2. ```max-width``` : Digunakan untuk menetapkan nilai lebar maksimal yang harus dimiliki elemen

## Overflowing Content
Jika kita tetapkan dimensi box secara manual, konten di dalamnya bisa saja mengalami overflow(tumpah-tumpah). Di CSS, kita bisa mengatasi hal ini dengan beberapa properti:
1. ```overflow: visible``
2. ```overflow:hidden```
3. ```overflow:scroll```
4. ```overflow:auto```

## Border
### Border Width
```border-width: 2px 2px 2px 2px; /*top right bottom left*/```
> Notes!
- Ketika satu nilai ditentukan, maka nilai berlaku untuk empat sisi.
- Ketika dua nilai ditentukan, nilai pertama berlaku untuk sisi atas dan bawah, nilai kedua untuk sisi kiri dan kanan.
- Ketika tiga nilai ditentukan, nilai pertama berlaku untuk sisi atas, nilai yang kedua untuk sisi kiri dan kanan, nilai ketiga untuk sisi bawah.
- Ketika empat nilai ditentukan, nilai pertama berlaku untuk sisi atas, nilai yang kedua untuk sisi kanan, nilai yang ketiga untuk sisi bawah, dan nilai yang keempat untuk sisi kiri. Urutan tersebut berdasarkan arah jarum jam (clockwise).

> Shorthand Border
``` border: width style color;```


## Display Roles
Terdapat dua jenis display box roles pada CSS: Block Boxes dan Inline Boxes. Karakteristik box model ini merujuk kepada bagaimana perilaku box terhadap box lain dan halamannya. 

### Outer Display : Block and Inline

#### Block Boxes
- Ketika dibuat, box akan muncul di baris baru
- Secara default, box akan menyesuaikan ukurannya dengan container miliknya 100%
- Width and height properties bisa diubah
- Padding, margin, dan border akan menyebabkan elemen lain terdorong menjauh dari box
- Beberapa elemen HTML seperti h1 dan p termasuk tipe block untuk outer display nya by defaulT


#### Inline Boxes
- Ketika dibuat, box tidak muncul di baris baru
- Width dan height tidak dapat diubah
- Vertical padding, margins, dan border: berpengaruh, tapi tidak akan menyebabkan inline boxes lainnya menjauh dari box
- Horizontal padding, margins, dan border: berpengaruh, dan akan menyebabkan inline boxes lainnya menjauh dari box. 
- a span em dan strong termasuk yang menggunakan inline type of outer display by default.

> Tipe dari box didefinisikan dengan properti ```display``` dengan value ```block```, ```inline```
1. ```display: inline``` : Mengubah elemen block berperilaku menjadi elemen inline
2. ```display: block``` : Mengubah elemen inline berperilaku menjadi elemen block
3. ```display: inline-block``` : digunakan ketika kita tidak ingin sebuah item muncul di line baru, namun masih ingin bisa mengatur width dan height dari item tersebut. Padding, margin dan border pun akan dapat diterapkan.
4. ```display: none``` : Menyembunyikan elemen dari halaman

# Belajar CSS Dasar
Resource: MDN Web Docs & others(w3school, freecodecamp, dll)

## Responsive Layout: Flexbox

### Flexbox Box Model
Merupakan teknik dalam penyusunan layout responsive pada CSS3 dengan mengunakan container. Konsep FLEXBOX yang wajib diketahui:
1. Dapat mengubah ukuran dimensi elemen dengan menyesuaikan ukuran yang cook bagi ruang kosong yang ada pada container-nya.
2. Bersifat directional agnostic. Tidak mengacu pada display inline maupun block.
3. Dibuat untukmenyusun layout yang mobile friendly.

### Flexbox Container
Flex container: wadah container yang menampung beberapa flex-item. Secara default, deretan flex-item pada container ditampilkan secara horizontal. 

Untuk membuat flex-container, kita gunakan properti ```display: flex```. Seluruh anak dari container tersebut akan menjadi flex item.

#### Properti untuk flex container
- ```display: flex```
- ```flex-direction: row``` : untuk mengatur arah dari urutan elemen2 di dalam flex-container secara horizontal
- ```flex-direction: column``` : untuk mengatur arah dari urutan elemen2 di dalam flex-container secara vertical
- ```flex-wrap: wrap``` : untuk membuat item ter-wrap ketika tidak cukup

##### Justify Content: Mengatur spacing antar flex items
- ``` justify-content: flex-start ```: rata kiri
- ``` justify-content: flex-end ```: rata kanan
- ``` justify-content: center ```: rata tengah
- ``` justify-content: space-between ```: elemen awal-rata kiri, elemen akhir-rata kanan, sisanya akan diberi jarak yang sama.
- ``` justify-content: space-around ```: membagi rata setiap sisi kanan dan kiri dari tiap elemen.
- ``` justify-content: space-evenly```

##### Align Items: Mengatur kesejajaran antar items secara vertikal dengan container | Alignt Content: Sama seperti align items, namun berlaku untuk item dengan lebih dari 2 baris
- ``` align-items: flex-start ```: rata kiri
- ``` align-items: flex-end ```: rata kanan
- ``` align-items: center ```: rata tengah
- ``` align-items: stretch ```: memenuhi parent (ketika kita tidak memberikan height pada flex item)
- ``` align-items: baseline ```

#### Properti untuk flex items
- ``` order: 1 ```: untuk mengubah urutan konten tanpa mengubah HTML
- ``` flex-grow ```: untuk menentukan ukuran pada items, tanpa mengatur width dan height

### Flex Grow
Properti ```flex-grow``` ini digunakan untuk memberitahu berapa banyak ukuran yang harus ditetapkan oleh flex-item. Nilai dari properti ini bukan nilai dari dimensi asli pada flex item, melainkan nilai yang relatif terhadap ruang kosong pada flex container.

Jika kita menetapkan nilai flex-grow yang sama pada seluruh flex item, maka dimensi dari tiap flex item akan sama rata dan memenuhi ruang kosong yang ada pada container. Namun jika kita memberikan nilai yang berbeda dari salah satu item-nya, contohnya nilai yang lebih besar, maka flex item tersebut akan mencakup ukuran yang lebih besar. Flex item yang lain akan menyusut menyesuaikan agar tetap masuk pada ruang flex container.

### Flex Direction
Secara default, deretan flex-item akan ditampilkan secara horizontal, namun kita dapat mengubahnya dengan menetapkan properti ```flex-direction: column``` pada flex-container nya.

Ada empat nilai yang bisa digunakan untuk properti flex-direction, antara lain:

1. ```row``` : merupakan nilai default, di mana deretan flex-item pada container ditampilkan secara horizontal.
2. ```row-reverse``` : memiliki sifat yang sama seperti row, namun urutan flex item-nya ditukar.
3. ```column``` : Deretan flex-item pada container ditampilkan secara vertikal.
4. ```column-reverse``` : memiliki sifat yang sama seperti column, namun urutan flex item-nya ditukar.

> Dengan menggunakan properti ini, kita dapat membuat dua dimensional layout dengan menempatkan flex container di dalam flex container, dalam arti lain sebuah flex container dapat memiliki child berupa flex container lain.

### Flex Basis
Digunakan untuk menentukan ukuran flex item. Mirip seperti width dalam menentukan dimensi box. Satuan yg bisa dipakai: px, pt, pc, cm, %. 

Properti ini digunakan ketika kita ingin menetapkan ukuran awal sebuah flex-item. Flex grow biasa digunakan ketika kita menerapkan nested flex-container dan terdapat perbedaan jumlah child pada container-nya.

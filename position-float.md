# Belajar CSS Dasar
Resource: MDN Web Docs & others(w3school, freecodecamp, dll)

## Positioning
Digunakan agar kita dapat mengubah posisi sebuah elemen tanpa memengaruhi elemen di sekitarnya. 

1. NORMAL FLOW/STATIC FLOW : Merupakan default behaviour pada elemen HTML, di mana setiap elemen block akan ditampilkan dalam baris baru ketika dibuat, bahkan jika di sampingnya masih terdapat space kosong.
2. RELATIVE POSITIONING : Membuat elemen bisa berpindah posisi ke atas, kanan, bawah, atau kiri dari posisi semula. Perpindahan posisinya tidak memengaruhi elemen di sekitarnya.
3. ABSOLUTE POSITIONING : Sama seperti relative, namun posisinya relatif pada jendela browser dan induk elemen(selama induk elemen berada di luar normal flow). Perbedaannya dengan relative adalah elemen ini benar-benar tidak dianggap ada oleh elemen pada normal flow. Akibatnya, lokasi awal elemen yang diberikan nilai absolute akan ditempati oleh elemen di bawahnya.
4. FIXED POSITIONING : Absolute position, namun posisi relatif pada jendela browser, walaupun pengguna melakukan scroll layar sekalipun, posisinya tidak berubah.

### Static Flow dan Non Static Flow
Jika memindahkan elemen yang posisinya static flow, maka elemen di sekitarnya ikut terpengaruhi. Sedangkan jika kita sudah mengatur posisinya menjadi non static, maka elemen lainnya tidak akan terpengaruhi.

> Note: Properti top, left, right, dan bottom hanya akan berpengaruh pada elemen yang menerapkan non-static-flow(position: relative, absolute, fixed)

## Floating
### Permasalahan Pada Floating
Elemen yang memiliki properti FLOAT akan dianggap tidak ada oleh elemen induknya: Dia akan keluar dari posisi normal flow. 
### Solusi-1: Clear Property
Properti clear memang dibuat untuk menghilangkan sifat float, dengan demikian elemen yang menerapkan properti float akan kembali “dianggap ada”. Namun untuk menerapkan properti ini kita perlu membuat sebuah elemen kosong (biasanya menggunakan div tanpa konten) yang menerapkan properti clear.
```
//css
.clear {
        clear: left;
        }
 
 //html
 <div class="clear"></div>
```

### Solusi-2: Overflow Technique
Menetapkan properti ```overflow: auto;``` pada elemen yang menampung elemen float.  

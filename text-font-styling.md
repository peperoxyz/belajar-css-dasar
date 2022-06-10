# Belajar CSS Dasar
Resource: MDN Web Docs & others(w3school, freecodecamp, dll)

## Formatting Text (Text and Font Styling)
CSS memisahkan styling untuk Font dan Text. Properti FONT digunakan untuk menetapkan styling pada TAMPILAN teks: tipe font, ukuran, ketebalan, dll. Sedangkan properti TEXT digunakan untuk mendukung hal lainnya dalam menampilkan teks: text-alignment(posisi teks), dekorasi, spacing, dll.

### Font Styling
A. Paket properti FONT
1. ```font-family``` : Menetapkan jenis font yang akan diterapkan pada target. 

2. ```font-size``` : Menetapkan ukuran font. 

- Satuan Relatif: em(relatif terhadap aslinya), ex(height), rem(relatif root element), ch(width), vw, vh.
- Satuan Absolut: px(pixel), pt(points), pc(picas=12 point), mm, cm, in.

3. ```font-weight``` : Mengatur ketebalan dari font yang ditampilkan.
```normal, bold, bolder, lighter```

4. ```font-style``` : Mengatur style dari font(vetikal/normal, atau miring)
```normal, italic, oblique```

> Shorthand
```
target {font: style weight variant-size font-family};
```
contoh:
```
p {font: bold 1em sans-serif}
```

### Text Styling
1. ```line-height``` : Bekerja seperti line spacing pada rich text editor (ms word)
2. ```text-indent``` : Memberi jarak/lekuk di awal paragraf (seperti TAB)
3. ```text-alignt``` : Mengatur perataan teks (rata kanan, kiri, tengah, kanan-kiri)

### Text Decoration
1. ``` text-decoration: underline``` : Memberikan efek underline pada teks
2. ``` text-decoration: overline``` : Efek garis atas pada teks
3. ``` text-decoration: line-through``` : Efek text dicoret 
4. ``` text-decoration: none``` : Menghilangkan dekoraasi yang ada

### Text Transform
1. ``` text-transform: none``` : Tidak ada perubahan
2. ``` text-transform: capitalize``` : Mentransform ke huruf kapital tiap kata
3. ``` text-transform: lowercase``` : Mentransform seluruh teks agar menggunakan huruf kecil
4. ``` text-transform: uppercase``` : Mentransform seluruh teks agar menggunakan huruf besar

### Word and Letter Spacing
1. ```letter-spacing: npx;``` 
2. ```word-spacing: npx;``` 

### Text Shadow
```text-shadow: kiri, atas, blur, warna```
contoh: 
```
text-shadow: 2px 2px 7px #111111;
```

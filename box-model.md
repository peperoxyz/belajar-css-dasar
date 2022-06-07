# Belajar CSS Dasar
Resource: MDN Web Docs & others(w3school, freecodecamp, dll)

## CSS Box Model
Terdapat dua jenis box model pada CSS: Block Boxes dan Inline Boxes. Karakteristik box model ini merujuk kepada bagaimana perilaku box terhadap box lain dan halamannya. 

### Outer Display : Block and Inline

#### Block Boxes
- Ketika dibuat, box akan muncul di baris baru
- Secara default, box akan menyesuaikan ukurannya dengan container miliknya 100%
- Width and height properties are respected
- Padding, margin, dan border akan menyebabkan elemen lain terdorong menjauh dari box
- Beberapa elemen HTML seperti h1 dan p termasuk tipe block untuk outer display nya by defaulT


#### Inline Boxes
- Ketika dibuat, box tidak muncul di baris baru
- Width dan height tidak akan memengaruhi
- Vertical padding, margins, dan border: berpengaruh, tapi tidak akan menyebabkan inline boxes lainnya menjauh dari box
- Horizontal padding, margins, dan border: berpengaruh, dan akan menyebabkan inline boxes lainnya menjauh dari box. 
- a span em dan strong termasuk yang menggunakan inline type of outer display by default.

> Tipe dari box didefinisikan dengan properti ```display``` dengan value ```block```, ```inline```

#### Inline-Block [Gabungan]
```display: inline-block``` digunakan ketika kita tidak ingin sebuah item muncul di line baru, namun masih ingin bisa mengatur width dan height dari item tersebut. Padding, margin dan border pun akan dapat diterapkan.

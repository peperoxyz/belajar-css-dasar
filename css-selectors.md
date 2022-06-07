# Belajar CSS Dasar
Resource: MDN Web Docs & others(w3school, freecodecamp, dll)

## CSS Selecotors
CSS Selectors adalah sebuah pola dari elemen yang memberi tahu browser elemen HTML yang mana yang harus di-select untuk memiliki value dari property CSS yang diberikan.

### Tipe-tipe Selectors
1. Selector by Type (HTML Tags)
``` h1 {property: value;} ```
Artinya: select tag h1

2. Selector by Class
``` .className {property: value;} ```
Artinya: select tag dengan class bernama className

3. Selector by ID
``` #uniqueID {property: value;} ```
Artinya: select tag dengan ID uniqueID

4. Attribute Selectors
``` a[href="www.awebsite.com"] {property: value;} ```
Artinya: select tag anchor dengan atribut href tersebut

5. Pseudo-Classes and Pseudo-Elements
``` a:hover {property: value;}```
Artinya: select semua anchor ketika di-hover
``` p:first-line {property: value;}```
Artinya: select baris pertama dari sebuah paragraf

6. Combinators
``` article > p {property: value;} ``` 
Artinya: select semua tag p yang berada tepat di bawah tag article


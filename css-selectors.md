# Belajar CSS Dasar
Resource: MDN Web Docs & others(w3school, freecodecamp, dll)

## CSS Selecotors
CSS Selectors adalah sebuah pola dari elemen yang memberi tahu browser elemen HTML yang mana yang harus di-select untuk memiliki value dari property CSS yang diberikan.

### Tipe-tipe Selectors
#### Basic Selectors
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

### Pseudo-Classes and Pseudo-Elements
1. Pseudo Classes
``` a:hover {property: value;}```
Artinya: select semua anchor ketika di-hover

``` a:link {property: value;}```
Artinya: select semua anchor yang belum pernah dikunjungi

``` a:visited {property: value;}```
Artinya: select semua anchor yang sudah pernah dikunjungi

2. Pseudo Elements
```
p::first-letter {
font-size: 32px;
font-weight: bold;
color: saddlebrown;
}
```
Artinya: select karakter pertama pada sebuah paragraf dan terapkan stylingnya

#### Combinator Selectors
1. Child Selector
``` article > p {property: value;} ``` 
Artinya: select semua tag p yang berada tepat di dalam tag article(sebagai anak dari tag article)

2. Adjacent Sibling Selector (+)
``` article + p {property: value;} ``` 
Artinya: select satu tag p yang berada tepat di bawah tag article

3. General Sibling Selector (~)
``` article ~ p {property: value;}```
Artinya: select seluruh tag p yang berada di bawah tag article

4. Descendant Selector (space)
``` article p {property: value;}```
Artinya: select seluruh tag p yang berada di bawah tag article, walaupun tidak secara langsung.

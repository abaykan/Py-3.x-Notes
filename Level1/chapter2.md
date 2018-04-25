<p align='center'><img src='https://upload.wikimedia.org/wikipedia/commons/f/f8/Python_logo_and_wordmark.svg' /></p>

# Py-3.x-Notes: Level 1

## Chapter 2
### Perlu diketahui
[Deklarasi](https://en.wikipedia.org/wiki/Declaration_(computer_programming)) : Pembuatan variabel tanpa / dengan adanya nilai awal 

[Inisialisasi](https://en.wikipedia.org/wiki/Initialization_(programming)) : Pengisian nilai awal pada sebuah variabel 

[Assign](https://en.wikipedia.org/wiki/Assignment_(computer_science)) : Pengisian(ulang) nilai pada sebuah variabel

[Syntax](https://en.wikipedia.org/wiki/Syntax_(programming_languages)) : Aturan penulisan code pada programming

[Semantic](https://en.wikipedia.org/wiki/Semantics_(computer_science)) : Penamaan yang memiliki arti sebenarnya

[Naming Convention](https://en.wikipedia.org/wiki/Naming_convention_(programming)) : Aturan penamaan yang sudah ditetapkan

[White Space](https://simple.wikipedia.org/wiki/Whitespace_(computer_science)) : Karakter yang ada namun tidak terlihat bentuknya
### Variabel
[Variabel](https://en.wikipedia.org/wiki/Variable_(computer_science)) di python akan mengetahui secara otomatis apa tipe datanya saat kita melakukan deklarasi

Untuk deklarasi Variabel python menggunakan syntax : 
```python
nama_variabel = 'value dari variabel'
```

Naming convention di python adalah [Snake Case](https://en.wikipedia.org/wiki/Snake_case), dimana kita menggunakan semuanya huruf kecil dan perkata dipisahkan menggunakan underscore dan dibiasakan semantic :)
```python
  nama_saya = 'Clavin June'
  umur_saya = 20
```

Agar deklarasi bisa lebih mudah dibaca, dibiasakan diantara '=' dan nama variabel atau value dari variabel diberi spasi
### Tipe Data
#### Angka
* int / long : bilangan bulat (-999999999999999999 - 9999999999999999999999)
* float : bilangan decimal (0.0)
* complex : bilangan complex matematika (angka biasa diakhiri j) -> (0j ,1j, 2j)
* hexa : bilangan hexadecimal (angka biasa diawali 0x) -> (0x1, 0x2, 0x02)
* octal : bilangan octadecimal (angka biasa diawali 0o) -> (0o1, 0o7, 0o16)
* biner : bilangan biner ( 0 / 1 diawali 0b ) -> (0b1, 0b0101)
* infinite : bilangan yang mewakili infinite pada matematika ( float('inf') )
```python
bilangan_bulat = 9999999
bilangan_decimal = 0.123413
bilangan_complex = 0j
hexa = 0x01
octal = 0o1
biner = 0b101101
infinite = float('inf')
```
#### karakter
* char : 1 karakter apa saja ('a', 'b', 'c', "d")
* string : banyak char ('ini string', "kumpulan karakter")
* byte : representasi byte dari setiap karakter (string diawali dengan b) -> (b'ini byte', b'contoh')

Didalam python untuk type data karakter ini bisa diapit menggunakan ' atau "
Tetapi agar terlihat konsisten, tolong dipilih salah satu :)

Ada beberapa karakter spesial yang dapat mewakili white space seperti 'Enter' atau 'Tab'
Enter diwakili oleh '\n', sedangkan tab diwakili oleh '\t'

Bagaimana jika ingin menuliskan karakter yang lebih dari 1 baris ? bisa menggunakan 'Multi Line String' yang diapit oleh tiga buah ' atau "

```python
satu_karakter = 'c'
strings = 'kumpulan karakter'
contoh_byte = b'contoh'
multi_line_strings = 'line 1 \n line 2'
multi_line_strings = '''line 1
line 2'''
```
#### Lain lain
* Boolean: berisi True / False
* None : type data kosong
* Ellipsis: type data yang biasa digunakan untuk slicing
```python
boolean = True
kosong = None
contoh_ellipsis = ...
```

#### Komentar
Untuk penulisan komentar di Python bisa menggunakan # untuk satu line
bisa menggunakan ''' untuk multi line
```python
# Ini single line comment
'''
 Ini Multi Line Comments
'''
"""
 Yang Ini Juga Multi Line Comments
"""
```

[<<< Chapter 2 : Variabel](chapter2.md)

[>>> Chapter 3 : Struktur Data](chapter3.md)

[Root](../README.md)

[Level 1](README.md)


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
### Variabel
[Variabel](https://en.wikipedia.org/wiki/Variable_(computer_science)) di python akan mengetahui secara otomatis apa tipe datanya saat kita melakukan [deklarasi](https://en.wikipedia.org/wiki/Declaration_(computer_programming))

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
* complex : bilangan complex matematika (angka biasa diakhii j) -> (0j ,1j, 2j)
* hexa : bilangan hexadecimal (angka biasa diawali 0x) -> (0x1, 0x2, 0x02)
* octal : bilangan octadecimal (angka biasa diawali 0o) -> (0o1, 0o7, 0o16)
* infinite : bilangan yang mewakili infinite pada matematika ( float('inf') )
```python
bilangan_bulat = 9999999
bilangan_decimal = 0.123413
bilangan_complex = 0j
hexa = 0x01
octal = 0o1
infinite = float('inf')
```
[Chapter 3 : Struktur Data](chapter3.md)

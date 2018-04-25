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

Untuk melihat type data apa yang dimiliki variabel di python kita bisa menggunakan 3 cara
* type(var) : fungsi yang return nya adalah type data dari variabel
* repr(var) : fungsi yang return nya adalah representasi dari sebuah variabel
* isinstance(var, class) : fungsi yang return nya hasil check dari variabel dan type datanya

```python
angka = 1
type(angka) # akan menghasilkan '<class 'int'>'
type('test') # akan menghasilkan '<class 'str'>'

repr(1) # akan menghasilkan '1' artinya integer
repr('a') # akan menghasilkan "'a'" diapit oleh " artinya string

isinstance(1, int) # akan menghasilkan True, karena 1 adalah integer
isinstance(1.0, int) # akan menghasilkan False, karena 1.0 adalah float
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

#### Input / Output
Untuk mengeluarkan Output di python kita bisa menggunakan fungsi print(), sedangkan untuk menerima Input di python menggunakan fungsi input()
```python
print('Hello World!') # Akan menghasilkan Hello World! di Console
tampung = input('Masukkan angka : ') # Akan menunggu user untuk menginput data, dan akan ditampung kedalam variabel 'tampung'
```
fungsi input() di python akan mengembalikan sebuah string, jadi jika misalkan kita melakukan ini
```python
angka = input('Masukkan angka : ')
print(type(angka)) # akan menghasilkan string bukan integer
```

maka jika ingin menampung sebuah integer kita melakukan Type-Casting

```python
angka = int(input('Masukkan angka : ')) # ini artinya kita mengubah hasil inputan kita kedalam bentuk integer
print(type(angka)) # akan menghasilkan integer
```

Jika kita ingin print value dari sebuah variabel, kita tinggal memasukan variabel sebagai parameter fungsi print
```python
angka = 1
print(angka) # Akan menghasilkan 1
```

fungsi print() akan selalu memberikan enter dibelakang, jadi jika kita melakukan
```python
print('a')
print('b')
'''Hasil Outputnya akan menjadi
a
b
'''
```

Jika ingin print tanpa memberikan 'enter'
```python
print('a', end='') # Kita tambahkan parameter ", end=''"
print('b')
'''Hasil Outputnya akan menjadi
ab
'''
```

Jika ingin print string dengan value dari variabel, kita bisa menggunakan formatting
```python
nama_saya = 'Clavin June'
umur_saya = 20

# Multi Line
print(''' Nama Saya Adalah {}
Umur Saya {}
'''.format(nama_saya, umur_saya)) #Disini '{}' yang pertama kali kita buat akan diisi dengan nama_saya, dan selanjutnya diisi dengan umur_saya

# Single Line
print('nama saya adalah {}'.format(nama_saya)) #formatting seperti ini akan membuat code lebih rapi
```

#### Kesimpulan
Pelajari Code dibawah ini :)
```python
'''
Program ini adalah hasil latihan dari Chapter 2 Level 1 Python 3
Author : Clavin June
Ini adalah contoh multi line comment :)
'''
nama = input('Masukkan nama anda : ') # Deklarasi isi variabel nama dengan inputan user
umur = int(input('Masukkan umur anda : ')) # Deklarasi isi variabel umur dengan inputan user dan di Type Casting kebentuk integer

print('Nama saya adalah {} dan umur saya {}'.format(nama, umur)) # Print isi variabel dengan menggunakan formatting
```

[<<< Chapter 1 : Perkenalan](chapter1.md)

[>>> Chapter 3 : Struktur Data](chapter3.md)

[Root](../README.md)

[Level 1](README.md)


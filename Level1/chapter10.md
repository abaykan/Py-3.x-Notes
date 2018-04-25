<p align='center'><img src='https://upload.wikimedia.org/wikipedia/commons/f/f8/Python_logo_and_wordmark.svg' /></p>

# Py-3.x-Notes: Level 1

## Chapter 10
### Perlu diketahui :
[Objek](https://en.wikipedia.org/wiki/Object_(computer_science)) : 	Yang dimaksud dengan Objek pada *Object-Oriented Programming / OOP*

[Modul](https://en.wikipedia.org/wiki/Modular_programming) : Fungisonalitas *Modules-Type* pada *Independent Scripting Language*

[*Standard-Library* / *std-lib*](https://en.wikipedia.org/wiki/Standard_library) : Spesifik Fungsionalitas yang akan digunakan pada project Python

<!-- TODO THE AUTHOR : References -->

## Contoh Modules

## Struktur Folder :
```
$HOME
|
|___ $USER
	|	.bashrc
	|	Desktop
	|	Images
	|	Examples
	|	Downloads
	|
	___Python Class
		|	salve_terrarum.py
		|	main.py3
		|	main2.py3
		|	salve_terrarum_with-class.py3
```

## Nama File : salve_terrarum.py
```python
def hello(): #Definisi Fungsi Hello()
	print("Hello")

def world(): #Definisi Fungsi World()
	print("World")

def terrarum(): #Definisi Fungsi Terrarum()
	return hello(), world()

salve = "Salve Terrarum adalah Hello World pada Latin" #Definisi global variabel salve salve_terrarum.py3
```

## Nama File : main.py3
```python
import salve_terrarum #Deklrasi modul python dan spesifik fungsi yang akan dipakai

salve_terrarum.hello() #Deklarasi modul python salve_terrarum fungsi hello()

salve_terrarum.world() #Deklarasi modul python salve_terrarum fungsi world()

salve_terrarum.terrarum() #Deklarasi modul python salve_terrarum fungsi terrarum()

print(salve_terrarum.salve) #Output Printing Syntax pada Deklarasi modul variable salve pada salve_terrarum
```

## Menjalankan main.py3
```
python@test-notes:~/Python Class $ python3 main.py
Hello
World
Hello
World
Salve Terrarum adalah Hello World pada Latin
python@test-notes:~/Python Class $

```

## Menajalankan *Standard-Library* main2.py3
```python
import difflib #difflib adalah Standard-Library Python yang digunakan untuk memungkinkan kesamaan string pada lebih dari 3 huruf String | difflib adalah implentasi dari program gnu diff linux <http://www.gnu.org/software/diffutils/>
difflib.get_close_matches("satu", ["satu", "atu", "dua", "3"])
```


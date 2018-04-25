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
		|	salve_terrarum_with-class.py3
		|	main.py3
		|	main2.py3
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

class Helloworld:
    def __init__(self, salve_class, terrarum_class):
        self.salve_class = salve_class
        self.terrarum_class = terrarum_class

    def fungsisalve(self):
        print(self.salve_class)

    def fungsiterrarum(self):
        print(self.terrarum_class)

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
Hello 	#keluaran dari def hello()
World 	#keluaran dari def world()
Hello 	#keluaran dari def terrarum()
World 	#keluaran dari def terrarum()
Salve Terrarum adalah Hello World pada Latin 	#keluaran dari variabel salve
python@test-notes:~/Python Class $

```

## Name File : salve_terrarum_with-class.py3
```python
from salve_terrarum import Helloworld

deklrasi_helloworld = salve_terrarum.Helloworld("Ini Dari parameter salve_class", "Ini Dari parameter terrarum_class") #inisialisasi class Helloworld(self, salve_class, terrarum_class)
deklrasi_helloworld.fungsisalve() #dari salve_terrarum(modules).Helloworld(class).fungsisalve(fungsi)
deklrasi_helloworld.fungsiterrarum() #dari salve_terrarum(modules).Helloworld(class).fingsoterrarum(fungsi)
```

## Menjalankan salve_terrarum_with-class.py3
```
python@test-notes:~/Python Class $ python3 main.py
# karena mempunyai 3 parameter dibagian self digunakan untuk utilitas dan access data pada object class, dibagian salve_class variabel = "Ini Dari parameter salve_class" , dibagian terrarum_class = "Ini Dari parameter terrarum_class"
Ini Dari parameter salve_class # dari fungsi untuk memprint parameter salve_class
Ini Dari parameter terrarum_class # dari fungsi untuk memprint parameter terrarum_class
python@test-notes:~/Python Class $ 

```

## Nama File : main2.py3
```python
import difflib #difflib adalah Standard-Library Python yang digunakan untuk memungkinkan kesamaan string pada lebih dari 3 huruf String
#difflib adalah implentasi dari program gnu diff linux <http://www.gnu.org/software/diffutils/>
difflib.get_close_matches("satu", ["satu", "atu", "dua", "3"]) #fungsi difflib get_close_matches dari string "satu" akan di mungkinkan sama pada list
```

## Menjalankan main2.py3
```python
['satu', 'atu']
```


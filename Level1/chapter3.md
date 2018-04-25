<p align='center'><img src='https://upload.wikimedia.org/wikipedia/commons/f/f8/Python_logo_and_wordmark.svg' /></p>

# Py-3.x-Notes: Level 1

## Chapter 3
### Perlu diketahui
[List](https://www.tutorialspoint.com/python/python_lists.htm) : Struktur Data yang dapat menyimpan banyak value

[Set](https://www.tutorialspoint.com/python/python_sets.htm) : Struktur Data yang hanya bisa menyimpan value yang unik (berbeda)

[Tuple](https://www.tutorialspoint.com/python/python_tuples.htm) : Struktur Data yang isinya tetap, tidak bisa diubah

[Dictionary](https://www.tutorialspoint.com/python/python_dictionary.htm) : Struktur Data yang isinya berdasarkan Key dan Value

### Struktur Data
[Struktur Data](https://en.wikipedia.org/wiki/Data_structure) di python ini diperlukan untuk menyimpan data yang banyak

```python
# Daripada kita membuat banyak variabel, misal
nilai_saya_1 = 100
nilai_saya_2 = 90
nilai_saya_3 = 80
# Ini akan memakan banyak sekali nama variabel

#Jika menggunakan Struktur Data
nilai_saya = [100, 90, 80] # List dari nilai saya
```

#### List
List ini dapat diwakilkan oleh [] seperti contoh diatas
List ini struktur data yang sangat fleksibel, bisa di tambahkan, di ubah, atau di hapus
```python
kosong = [] # Akan membuat sebuah list yang tidak ada isinya
nilai = [100,90,80,78,99] # List dari nilai
```
Cara mengakses data di list
```python
nilai = [100,90,80,78,99] # List dari nilai
'''
jika kita ingin mengakses data nilai yang bervalue 100
value 100 adalah data pertama kita
data pertama di wakilkan angka 0
data kedua diwakilkan angka 1
data ketiga diwakilkan angka 2
dan begitu seterusnya
'''

print(nilai[0]) # akan menghasilkan 100
print(nilai[3]) # akan menghasilkan nilai 78
print(nilai[10]) # error karena tidak ada data ke 9
```

[<<< Chapter 2 : Variabel](chapter2.md)

[>>> Chapter 4 : Operator](chapter4.md)

[Root](../README.md)

[Level 1](README.md)


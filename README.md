# pratikum5

# Program Menghitung Data Nilai Akhir Mahasiswa
Program ini merupakan berbasis list yang digunakan untuk menyimpan dan menghitung nilai akhir mahasiswa. 
Nilai akhir dihitung berdasarkan bobot tertentu dari nilai tugas, UTS, dan UAS.
# Deskripsi Program
Program ini dibuat menggunakan bahasa python dengan fitur:
- List dan Dictionary untuk penyimpanan data.
- Fungsi Kustom (def) untuk perhitungan nilai akhir.
- input() dan int() untuk input dan konversi data.
- while dan if untuk kontrol alur.
- append() dan break untuk menambah data ke list dan menghentikan perulangan.
- print() dan F-string untuk mencetak hasil dalam bentuk tabel yang terformat.
## Flowchart Programan
![Flowchart](https://github.com/Dwiokta10/Praktikum5/blob/main/flowchartprak5.png)
# Kode Program
```python
# Inisialisasi list untuk menyimpan data
data_mahasiswa = []

# Fungsi untuk menghitung nilai akhir
def hitung_nilai_akhir(tugas, uts, uas):
    return round((tugas * 0.3) + (uts * 0.35) + (uas * 0.35), 2)

# Input data mahasiswa
while True:
    nama = input("Nama: ")
    nim = input("NIM: ")
    tugas = int(input("Nilai Tugas: "))
    uts = int(input("Nilai UTS: "))
    uas = int(input("Nilai UAS: "))
    nilai_akhir = hitung_nilai_akhir(tugas, uts, uas)

    # Simpan data ke dalam dictionary
    data_mahasiswa.append({
        "Nama": nama,
        "NIM": nim,
        "Tugas": tugas,
        "UTS": uts,
        "UAS": uas,
        "Akhir": nilai_akhir
    })

    # Tanyakan apakah ingin menambah data lagi
    tambah = input("Tambah data (y/t)? ")
    if tambah.lower() != 'y':
        break

# Tampilkan data dalam bentuk tabel
print("\n| No | Nama     | NIM   | Tugas | UTS | UAS | Akhir |")
print("-" * 50)
for i, mhs in enumerate(data_mahasiswa, start=1):
    print(f"| {i:<2} | {mhs['Nama']:<8} | {mhs['NIM']:<5} | {mhs['Tugas']:<5} | {mhs['UTS']:<3} | {mhs['UAS']:<3} | {mhs['Akhir']:<5} |")

```
# Output Program
```
| No | Nama     | NIM   | Tugas | UTS | UAS | Akhir |
--------------------------------------------------
| 1  | Yanto     | 312410056 | 100   | 60  | 98  | 97.55 |
| 2  | Budi      | 312410085 | 90    | 80  | 99  | 95.95 |
| 3  | Agus      | 312410160 | 90    | 75  | 100 | 96.3  |
| 4  | Slamet    | 312410110 | 98    | 80  | 90  | 94.15 |
```
# Cara Kerja Program
1. Program pertama kali menginisialisasi list kosong bernama data_mahasiswa untuk menyimpan data setiap mahasiswa.
2. Fungsi hitung_nilai_akhir digunakan untuk menghitung nilai akhir berdasarkan formula:
   \[
   \text{nilai akhir} = (\text{nilai tugas} \times 0.3) + (\text{nilai UTS} \times 0.35) + (\text{nilai UAS} \times 0.35)
   \]
3. Program meminta pengguna untuk memasukkan data nama, NIM, nilai tugas, UTS, dan UAS.
4. Setelah nilai akhir dihitung menggunakan fungsi hitung_nilai_akhir, semua data tersebut disimpan dalam dictionary dan ditambahkan ke dalam list data_mahasiswa.
5. Pengguna dapat memilih untuk menambahkan data mahasiswa lain atau mengakhiri proses input.
6. Setelah input selesai, program akan mencetak data mahasiswa dalam bentuk tabel dengan kolom nomor, nama, NIM, nilai tugas, UTS, UAS, dan nilai akhir.# Program Menghitung Data Nilai Akhir Mahasiswa
Program ini merupakan berbasis list yang digunakan untuk menyimpan dan menghitung nilai akhir mahasiswa. 
Nilai akhir dihitung berdasarkan bobot tertentu dari nilai tugas, UTS, dan UAS.
# Deskripsi Program
Program ini dibuat menggunakan bahasa python dengan fitur:
- List dan Dictionary untuk penyimpanan data.
- Fungsi Kustom (def) untuk perhitungan nilai akhir.
- input() dan int() untuk input dan konversi data.
- while dan if untuk kontrol alur.
- append() dan break untuk menambah data ke list dan menghentikan perulangan.
- print() dan F-string untuk mencetak hasil dalam bentuk tabel yang terformat.
## Flowchart Programan

# Kode Program
```python
# Inisialisasi list untuk menyimpan data
data_mahasiswa = []

# Fungsi untuk menghitung nilai akhir
def hitung_nilai_akhir(tugas, uts, uas):
    return round((tugas * 0.3) + (uts * 0.35) + (uas * 0.35), 2)

# Input data mahasiswa
while True:
    nama = input("Nama: ")
    nim = input("NIM: ")
    tugas = int(input("Nilai Tugas: "))
    uts = int(input("Nilai UTS: "))
    uas = int(input("Nilai UAS: "))
    nilai_akhir = hitung_nilai_akhir(tugas, uts, uas)

    # Simpan data ke dalam dictionary
    data_mahasiswa.append({
        "Nama": nama,
        "NIM": nim,
        "Tugas": tugas,
        "UTS": uts,
        "UAS": uas,
        "Akhir": nilai_akhir
    })

    # Tanyakan apakah ingin menambah data lagi
    tambah = input("Tambah data (y/t)? ")
    if tambah.lower() != 'y':
        break

# Tampilkan data dalam bentuk tabel
print("\n| No | Nama     | NIM   | Tugas | UTS | UAS | Akhir |")
print("-" * 50)
for i, mhs in enumerate(data_mahasiswa, start=1):
    print(f"| {i:<2} | {mhs['Nama']:<8} | {mhs['NIM']:<5} | {mhs['Tugas']:<5} | {mhs['UTS']:<3} | {mhs['UAS']:<3} | {mhs['Akhir']:<5} |")

```
# Output Program
```
| No | Nama     | NIM   | Tugas | UTS | UAS | Akhir |
--------------------------------------------------
| 1  | Yanto     | 312410056 | 100   | 60  | 98  | 97.55 |
| 2  | Budi    | 312410085 | 90    | 80  | 99  | 95.95 |
| 3  | Agus   | 312410160 | 90    | 75  | 100 | 96.3  |
| 4  | Slamet    | 312410110 | 98    | 80  | 90  | 94.15 |
```
# Cara Kerja Program
1. Program pertama kali menginisialisasi list kosong bernama data_mahasiswa untuk menyimpan data setiap mahasiswa.
2. Fungsi hitung_nilai_akhir digunakan untuk menghitung nilai akhir berdasarkan formula:
   \[
   \text{nilai akhir} = (\text{nilai tugas} \times 0.3) + (\text{nilai UTS} \times 0.35) + (\text{nilai UAS} \times 0.35)
   \]
3. Program meminta pengguna untuk memasukkan data nama, NIM, nilai tugas, UTS, dan UAS.
4. Setelah nilai akhir dihitung menggunakan fungsi hitung_nilai_akhir, semua data tersebut disimpan dalam dictionary dan ditambahkan ke dalam list data_mahasiswa.
5. Pengguna dapat memilih untuk menambahkan data mahasiswa lain atau mengakhiri proses input.
6. Setelah input selesai, program akan mencetak data mahasiswa dalam bentuk tabel dengan kolom nomor, nama, NIM, nilai tugas, UTS, UAS, dan nilai akhir

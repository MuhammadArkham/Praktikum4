# Praktikum4

NAMA : Muhammad Arkhamullah Rifai Asshidiq

Mata kuliah : Bahasa pemrograman

NIM : 312410545

## Tugas Praktikum 4

## kode program
```python
# TUGAS PRAKTIKUM 4

nama = []
nim = []
nilai_tugas = []
nilai_uts = []
nilai_uas = []
nilai_akhir = []

print("\nProgram Input Nilai")
print("="*23)

while True:
    
    print("\nMasukan Data Mahasiswa")
    print("="*23)
    nama_mhs = input("Nama        : ")
    nama.append(nama_mhs)
    
    nim_mhs = input("NIM         : ")
    nim.append(nim_mhs)
    
    tugas = float(input("Nilai Tugas : "))
    nilai_tugas.append(tugas)
    
    uts = float(input("Nilai UTS   : "))
    nilai_uts.append(uts)
    
    uas = float(input("Nilai UAS   : "))
    nilai_uas.append(uas)
  
    nilai = (tugas * 0.3) + (uts * 0.35) + (uas * 0.35)
    nilai_akhir.append(nilai)
    
    lanjut = input("\nTambah data (y/t) ? ")
    if lanjut.lower() == 't':
        break

print("\n")
print("="*72)
print("|                        Daftar Nilai Mahasiswa                        |")
print("="*72)
print("| No |     Nama       |     NIM      | Tugas  |  UTS  |  UAS  | Akhir  |")
print("="*72)

for i in range(len(nama)):
    print("| {:<2} | {:<14} | {:<12} | {:<6} | {:<5} | {:<5} | {:<7.2f}|"
          .format(i+1, nama[i], nim[i], nilai_tugas[i], nilai_uts[i], nilai_uas[i], nilai_akhir[i]))

print("="*72)
```
## Hasil kode Program
![Foto](https://github.com/MuhammadArkham/Foto/blob/main/Screenshot%202024-11-16%20230237.png?raw=true)

## Penjelasan alur algoritma program
1. Membuat list kosong untuk menampung data:
```python
pythonCopynama = []
nim = []
nilai_tugas = []
nilai_uts = []
nilai_uas = []
nilai_akhir = []
```
2. Membuat perulangan untuk input data:
```python
pythonCopywhile True:
    # Input data mahasiswa
    nama_mhs = input("Nama        : ")
    nim_mhs = input("NIM         : ")
    tugas = float(input("Nilai Tugas : "))
    uts = float(input("Nilai UTS   : "))
    uas = float(input("Nilai UAS   : "))
```
3. Menghitung nilai akhir dengan bobot:

Tugas: 30%

UTS: 35%

UAS: 35%
```python
pythonCopynilai = (tugas * 0.3) + (uts * 0.35) + (uas * 0.35)
```
4. Menambahkan data ke dalam list:
```python
pythonCopynama.append(nama_mhs)
nim.append(nim_mhs)
nilai_tugas.append(tugas)
nilai_uts.append(uts)
nilai_uas.append(uas)
nilai_akhir.append(nilai)
```
5. Membuat kondisi untuk menambah data:
```python
pythonCopylanjut = input("\nTambah data (y/t) ? ")
if lanjut.lower() == 't':
    break
```
6. Menampilkan data dalam bentuk tabel:
```python
pythonCopyfor i in range(len(nama)):
    print("| {:<2} | {:<14} | {:<12} | {:<6} | {:<5} | {:<5} | {:<7.2f}|"
          .format(i+1, nama[i], nim[i], nilai_tugas[i], nilai_uts[i], nilai_uas[i], nilai_akhir[i]))
```
## Gambar Flowchart
![Foto](

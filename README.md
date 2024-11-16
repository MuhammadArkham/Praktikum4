# Praktikum4

Muhammad Arkhamullah Rifai Asshidiq

Bahasa pemrograman

312410545

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
![Foto](

# praktikum8
## Nama = Althaf Afif Faiz 
## NIM = 312410404
## Kelas = TI.24.A.3

# Tugas Praktikum 8 terdiri dari :
Buat program sederhana dengan mengaplikasikan penggunaan class. Buatlah

class untuk menampilkan daftar nilai mahasiswa, dengan ketentuan:

• Method tambah() untuk menambah data

• Method tampilkan() untuk menampilkan data

• Method hapus(nama) untuk menghapus data berdasarkan nama

• Method ubah(nama) untuk mengubah data berdasarkan nama

# Code Program

```
class NilaiMahasiswa:
    def __init__(self):
        self.daftar_nilai = {}

    def tambah(self, nama, nilai):
        """
        Menambah data mahasiswa ke dalam daftar nilai.

        Args:
            nama (str): Nama mahasiswa.
            nilai (int): Nilai mahasiswa.
        """
        self.daftar_nilai[nama] = nilai
        print(f"Data {nama} berhasil ditambahkan.")

    def tampilkan(self):
        """
        Menampilkan daftar nilai mahasiswa.
        """
        if not self.daftar_nilai:
            print("Daftar nilai kosong.")
        else:
            print("Daftar Nilai Mahasiswa:")
            for nama, nilai in self.daftar_nilai.items():
                print(f"{nama}: {nilai}")

    def hapus(self, nama):
        """
        Menghapus data mahasiswa dari daftar nilai berdasarkan nama.

        Args:
            nama (str): Nama mahasiswa.
        """
        if nama in self.daftar_nilai:
            del self.daftar_nilai[nama]
            print(f"Data {nama} berhasil dihapus.")
        else:
            print(f"Data {nama} tidak ditemukan.")

    def ubah(self, nama, nilai_baru):
        """
        Mengubah data mahasiswa dari daftar nilai berdasarkan nama.

        Args:
            nama (str): Nama mahasiswa.
            nilai_baru (int): Nilai baru mahasiswa.
        """
        if nama in self.daftar_nilai:
            self.daftar_nilai[nama] = nilai_baru
            print(f"Data {nama} berhasil diubah.")
        else:
            print(f"Data {nama} tidak ditemukan.")
```

## penjelasan Program

Class Mahasiswa: Class ini menyimpan daftar mahasiswa dalam bentuk list.

Method tambah(nama, nilai): Menambahkan data mahasiswa baru ke dalam daftar.

Method tampilkan(): Menampilkan semua data mahasiswa yang ada dalam daftar.

Method hapus(nama): Menghapus data mahasiswa berdasarkan nama yang diberikan.

Method ubah(nama, nilai_baru): Mengubah nilai mahasiswa berdasarkan nama yang diberikan.


## Flowchart 
![Flowchart](https://github.com/user-attachments/assets/95c18861-0d8c-4ac5-9928-45630a6e2caa)

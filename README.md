# pertemuan-11 
nama :agil tri iswara
kelas : IE.23.c12
nim :352310848


#SS koding



![WhatsApp Image 2024-12-09 at 01 17 15_a32c5992](https://github.com/user-attachments/assets/ae1c8217-75ca-4571-815f-1f2a80f8b842)







![WhatsApp Image 2024-12-09 at 01 18 26_c0d18ecc](https://github.com/user-attachments/assets/34ebfdae-2ab0-475e-b67e-aa42cbffa11b)







![WhatsApp Image 2024-12-09 at 01 19 14_9c2198cc](https://github.com/user-attachments/assets/bdde32a2-f2f4-45ff-9e68-85cb469f1262)









![WhatsApp Image 2024-12-09 at 01 20 09_8e6720f8](https://github.com/user-attachments/assets/7fd03f79-39ed-464c-8289-cdd01f50e06f)
















#KODING
# Daftar mahasiswa
mahasiswa = []

# Fungsi untuk menambah data mahasiswa
def tambah():
    nama = input("Masukkan nama mahasiswa: ")
    nilai = input("Masukkan nilai mahasiswa: ")
    mahasiswa.append({"nama": nama, "nilai": nilai})
    print("Data mahasiswa berhasil ditambahkan!")

# Fungsi untuk menampilkan data mahasiswa
def tampilkan():
    if not mahasiswa:
        print("Tidak ada data mahasiswa.")
    else:
        print("\nDaftar Nilai Mahasiswa:")
        for mhs in mahasiswa:
            print(f"Nama: {mhs['nama']}, Nilai: {mhs['nilai']}")

# Fungsi untuk menghapus data mahasiswa berdasarkan nama
def hapus(nama):
    global mahasiswa
    mahasiswa = [mhs for mhs in mahasiswa if mhs['nama'] != nama]
    print(f"Data mahasiswa dengan nama {nama} telah dihapus!")

# Fungsi untuk mengubah data mahasiswa berdasarkan nama
def ubah(nama):
    for mhs in mahasiswa:
        if mhs['nama'] == nama:
            nilai_baru = input(f"Masukkan nilai baru untuk {nama}: ")
            mhs['nilai'] = nilai_baru
            print(f"Data nilai mahasiswa {nama} berhasil diubah!")
            return
    print(f"Mahasiswa dengan nama {nama} tidak ditemukan!")

# Menu utama program
def main():
    while True:
        print("\nMenu:")
        print("1. Tambah Data Mahasiswa")
        print("2. Tampilkan Data Mahasiswa")
        print("3. Hapus Data Mahasiswa")
        print("4. Ubah Data Mahasiswa")
        print("5. Keluar")
        
        pilihan = input("Pilih menu (1/2/3/4/5): ")
        
        if pilihan == "1":
            tambah()
        elif pilihan == "2":
            tampilkan()
        elif pilihan == "3":
            nama = input("Masukkan nama mahasiswa yang ingin dihapus: ")
            hapus(nama)
        elif pilihan == "4":
            nama = input("Masukkan nama mahasiswa yang ingin diubah: ")
            ubah(nama)
        elif pilihan == "5":
            print("Terima kasih, program selesai.")
            break
        else:
            print("Pilihan tidak valid. Silakan coba lagi.")

if __name__ == "__main__":
    main()

#FLOW CHART





![tugas pertemuan 11 (lab 6)_page-0001](https://github.com/user-attachments/assets/27d8114a-3422-410e-a64f-45505a30a482)



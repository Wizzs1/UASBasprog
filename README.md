Nama  : Wisnu Ikhwansyah Saputra

Nim   : 312210305

Kelas : TI 22.A3

---

# UAS Bahasa Pemrograman
## Model
> tambah_data
- ```data = {}``` untuk menampung data yang akan diinput

- deklarasikan fungsi ```def tambah_data():```

- ```nama = input("Masukan nama: ")``` lalu tambahkan input nama, nim, nilai tugas, uts, uas

- ```nilai_akhir = (nilai_tugas)*30/100 + (nilai_uts)*35/100 + (nilai_uas)*35/100``` untuk nilai akhir diambil dari perhitungan 3 komponen nilai (nilai_tugas: 30%, nilai_uts: 35%, nilai_uas: 35%)

- ```data[nama] = [nama, nim, nilai_tugas, nilai_uts, nilai_uas, nilai_akhir]```  kita akan masukkan data yang tadi kita input ke dalam `data[nama]'

- lalu cetak ```print()```

> Ubah_data
- deklarasikan fungsi ```def ubah_data():```

- ```if nama in data.keys(): print("Mau mengubah apa?")``` jika 'nama' dari di dalam 'data' maka akan mengembalikan daftar menggunakan fungsi ```'keys()'``` lalu di cetak lah ```'print()```

- ```sub_data = input("(Semua), (Nama), (NIM), (Tugas), (UTS), (UAS) : "```membuat menu ubah di dalam ```sub_data```

- ```if sub_data.lower() ==``` "semua": ambil kata kunci 'semua' di dalam ```sub_data```

- lalu cetak ```print("\nBerhasil ubah data!")```

- ```else: print("'{}' tidak ditemukan.".format(nama))``` jika kita salah dalam memasukkan nama untuk mengubah data maka akan muncul 'nama tidak di temukan'

> cari_data
- deklarasikan fungsi def ```cari_data():```

- ```nama = input("Masukan nama untuk mencari data: ")``` kita akan menginput data yang nanti akan di cari

- ```if nama in data.keys():``` kita mengambil list 'nama' di dalam 'data' menggunakan pengkondisian
 
 - ```else: print("'{}' tidak ditemukan.".format(nama))``` jika data yang kita input salah/tidak ditemukan maka akan tercetak 'nama tidak di temukan'
 
 > hapus_data
- deklarasikan fungsi def ```hapus_data():```

- ```nama = input("Masukan nama untuk menghapus data : ")``` kita akan menginput data yang nanti akan di hapus

- ```if nama in data.keys():``` kita mengambil list 'nama' di dalam 'data' menggunakan pengkondisian

- ```del data[nama]``` hapus semua 'nama' yang ada di dalam 'data'

- jika sudah maka cetak ```print("sub_data '{}' berhasil dihapus.".format(nama))```

- ```else: print("'{}' tidak ditemukan.".format(nama))``` jika data yang kita input salah/tidak ditemukan maka akan tercetak 'nama tidak di temukan'

## View
>input_nilai
- menambahkan fungsi input yang nanti nya akan di deklarasikan di setiap module nya, ```def input_nama():``` ```def input_nim():```

>view_nilai
- deklarasikan fungsi ```def lihat_data():```

- lalu cetak ```print()```

Setelah semua tadi sekarang saatnya menjalankan program main.py

    from Model.daftar_nilai import *
    from View.view_nilai import *

    #Mulai
    print("===============================================================")
    print("|                           Program                           |")
    print("===============================================================")
    
     while True:
         print("\n")
         menu = input("(L) Lihat, (T) Tambah, (H) Hapus, (U) Ubah, (C) Cari, (K) Keluar\nPilih menu: ")
         print("\n")

      # menu
      if menu.lower() == 't':
          tambah_data()

      elif menu.lower() == 'c':
          cari_data()

      elif menu.lower() == 'l':
          lihat_data()

      elif menu.lower() == 'u':
          ubah_data()

      elif menu.lower() == 'h':
          hapus_data()

      # Keluar
      elif menu.lower() == 'k':
          break

      else:
          print("Upss ada yang salah, silahkan cek kembali.")



## Output Tambah data

<img width="869" alt="UAS " src="https://user-images.githubusercontent.com/110619093/211191096-9a116aeb-8cd8-42a8-af68-ea823365812a.png">

## Output Lihat data

<img width="591" alt="UAS1" src="https://user-images.githubusercontent.com/110619093/211191140-85128a63-bcc4-4377-99f2-2edb40c458bd.png">

## Output Ubah data

<img width="526" alt="UAS2" src="https://user-images.githubusercontent.com/110619093/211191183-211ac6f3-e577-4fc0-8571-7686aae15ac3.png">

## Output Cari data

<img width="557" alt="UAS3" src="https://user-images.githubusercontent.com/110619093/211191240-f9c6a710-005a-483c-a7f2-96c8c0084b2f.png">

## Output Hapus data

<img width="485" alt="UAS4" src="https://user-images.githubusercontent.com/110619093/211191282-9805e9d3-0b62-4564-934f-9594906c4d1c.png">

# Dokumentasi
## YouTube

[Ada disini](https://youtu.be/43al3inNVv8)

## PDF

[Ada disini](https://drive.google.com/file/d/1JfbO9kp4N3SlXICB7yNFujw4wQSMg8Nf/view?usp=sharing)

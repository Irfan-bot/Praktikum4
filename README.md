# praktikum4
## Program Data Mahasiswa

Pada praktikum 4, kita akan membuat program sederhana untuk menginput data ke dalam sebuah list.


## Penjelasan
1.) Pertama kita membuat variable list kosong.

nilai = []

ulang = True

Variable ulang = True digunakan untuk mengontrol perulangan.

2.) Lalu kita membuat kondisi perulangan dan statement yang akan dijalankan ketika perulangan terjadi.

while ulang:

nama = input("Masukkan Nama: ")

nim = input("Masukkan NIM: ")

tugas = int(input("Masukkan Nilai Tugas: "))

uts = int(input("Masukkan Nilai UTS: "))

uas = int(input("Masukkan Nilai UTS: "))

akhir = (tugas * 30/100) + (uts * 35/100) + (uas * 35/100)

nilai.append([nama, nim, tugas, uts, uas, int(akhir)])

Dari statement diatas, kita akan diminta untuk menginput nama, nim, nilai tugas, nilai uts, dan nilai uas, lalu system akan menjumlahkan nilai-nilai tersebut dan menghasilkan nilai akhir. Setelah menginput berbagai data atau item, inputan item tersebut akan masuk ke dalam list 'nilai'

3.) Setelah membuat perulangan, kita membuat statement untuk menghentikan atau keluar dari perulangan yang terjadi.

if (input("Tambah data (y/t)?") == 't'):

ulang = False

Untuk keluar dari perulangan kita hanya perlu menginputkan 't' apabila diminta pada saat program dijalankan. 't' akan membuat variable ulang = True menjadi ulang = False yang mana akan menghentikan perulangan yang terjadi.

4.) Terakhir kita akan mencetak hasil dari program yang telah dibuat.
print("\nDaftar Nilai Mahasiswa")

print("==================================================================")

print("|No. |     Nama     |    NIM    | Tugas |  UTS  |  UAS  |  Akhir |")

print("==================================================================")

i = 0

for item in nilai:

i += 1

print("| {no:2d} | {nama:12s} | {nim:9s} | {tugas:5d} | {uts:5d} | {uas:5d} | {akhir:6.2f} |"
          .format(no=i, nama=item[0], nim=item[1], tugas=item[2], uts=item[3], uas=item[4], akhir=item[5]))

print("==================================================================")


# Screenshot Input
![Screenshot (49)](https://user-images.githubusercontent.com/56944673/69475603-fb869700-0d83-11ea-9361-3236e0078bfc.png)


# Screenshot Output

![Screenshot (50)](https://user-images.githubusercontent.com/56944673/69475628-35f03400-0d84-11ea-823f-cb1b0438525d.png)


# Flowchart

![Flowchart](https://user-images.githubusercontent.com/56944673/69481718-7671a100-0dc8-11ea-9044-b5656c7b3dce.png)


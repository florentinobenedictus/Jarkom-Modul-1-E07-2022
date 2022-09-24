# Jarkom-Modul-1-E07-2022
| Nama                        | NRP        |
|:---------------------------:|:----------:|
| Arya Nur Razzaq             | 5025201102 |
| Florentino Benedictus       | 5025201222 |
| Muhammad Zufarrifqi Prakoso | 5025201276 |

#### [Soal](#soal)
- [Soal 1](#soal-1)
- [Soal 2](#soal-2)
- [Soal 3](#soal-3)
- [Soal 4](#soal-4)
- [Soal 5](#soal-5)
- [Soal 6](#soal-6)
- [Soal 7](#soal-7)
- [Soal 8-10](#soal-8-10)
    - [Soal 8](#soal-8)
    - [Soal 9](#soal-9)
    - [Soal 10](#soal-10)
#### [Resource Soal](Resources)
#### [Pembagian Tugas](#pembagian-tugas-1)
#### [Revisi](#revisi-1)
#### [Kendala](#kendala-1)

## Soal 1
Sebutkan web server yang digunakan pada "monta.if.its.ac.id"!
### Jawaban
- Gunakan display filter `http.host == monta.if.its.ac.id` lalu follow TCP stream salah satu paket
![image](https://user-images.githubusercontent.com/85059763/192096083-3ff7bbe1-39c7-4814-bb8a-8d68d58c6016.png)
- DItemukan server yang digunakan `nginx/1.10.3`

## Soal 2
Ishaq sedang bingung mencari topik ta untuk semester ini , lalu ia datang ke website monta dan menemukan detail topik pada website “monta.if.its.ac.id” , judul TA apa yang dibuka oleh ishaq ?
### Jawaban
- Gunakan display filter `http.host == "monta.if.its.ac.id" and http contains "monta" and http contains "detail"` lalu follow TCP stream paket yang terletak paling atas
![image](https://user-images.githubusercontent.com/85059763/192096355-3bc87271-dfb4-4336-950c-675ddeab152a.png)
- Selanjutnya show data as raw, lalu save dengan ekstensi `.rar` atau `.zip`
![image](https://user-images.githubusercontent.com/85059763/192096458-1164ece7-382a-4ddc-b040-2aa55465679d.png)
- Extract file menggunakan winrar
![image](https://user-images.githubusercontent.com/85059763/192096483-c06433df-701e-4c74-be26-2143183357b4.png)
- Ditemukan sebuah file tanpa ekstensi, lalu setelah coba dibuka dengan notepad++, file tersebut memiliki format file `.html`
![image](https://user-images.githubusercontent.com/85059763/192096552-11811de1-c76f-47ca-9270-acce6ccae1b0.png)
- Tambahkan ekstensi `.html` pada file tersebut, lalu dibuka pada browser
![image](https://user-images.githubusercontent.com/85059763/192096578-b47fb27f-6ed2-4d86-beb8-63f527ac7810.png)
- Ditemukan judul TA `Perancangan Sistem Pengendali Panas Otomatis pada
Mesin Sangrai Kopi dengan Logika Fuzzy`
![image](https://user-images.githubusercontent.com/85059763/192096594-d9518a50-1806-4762-8df3-584ff0721dce.png)

## Soal 3
Filter sehingga wireshark hanya menampilkan paket yang menuju port 80!
### Jawaban
- Buka file soal3-6 di wireshark
- Pada display filter tuliskan tcp.dstport == 80
- Paket yang menuju port 80 telah terfilter
### Screenshot Pengerjaan
<img width="1200" alt="Screen Shot 2022-09-19 at 20 53 02" src="https://user-images.githubusercontent.com/103361498/191998263-57ea3fc0-8a10-44dd-aec4-3c4ea4a68029.png">

## Soal 4
Filter sehingga wireshark hanya mengambil paket yang berasal dari port 21!
### Jawaban
- Buka file soal3-6 di wireshark
- Pada display filter tuliskan tcp.dstport == 21
- Paket yang berasal dari port 21 telah terfilter
### Screenshot Pengerjaan
<img width="1199" alt="Screen Shot 2022-09-19 at 20 56 36" src="https://user-images.githubusercontent.com/103361498/191998836-f2c74029-5d59-48e6-af18-e2e89df51e9a.png">

## Soal 5
Filter sehingga wireshark hanya mengambil paket yang berasal dari port 443!
### Jawaban
- Buka file soal3-6 di wireshark
- Pada Display filter tuliskan tcp.dstport == 443
- Paket yang berasal dari port 443 telah terfilter
### Screenshot Pengerjaan
<img width="1190" alt="Screen Shot 2022-09-19 at 20 54 45" src="https://user-images.githubusercontent.com/103361498/191999014-908af9f9-14ef-464c-9f72-97f4bc9f1fc8.png">

## Soal 6
Filter sehingga wireshark hanya menampilkan paket yang menuju ke lipi.go.id !
### Jawaban
- Buka file soal3-6 di wireshark
- Untuk mengetahui ip dari website bisa menggunakan nslookup lipi.go.id 
- Pada display filter tuliskan Ip.dst == 203.160.128.158
- Paket yang menuju website lipi.go.id akan terfilter
### Screenshot Pengerjaan
<img width="563" alt="Screen Shot 2022-09-23 at 22 39 06" src="https://user-images.githubusercontent.com/103361498/192000188-5627841a-839e-415a-b2c5-a095d1a6f5c9.png">
<img width="1113" alt="Screen Shot 2022-09-19 at 20 20 15" src="https://user-images.githubusercontent.com/103361498/192000233-706322d0-b8fa-4f3a-9190-d38b7bbec5e7.png">

## Soal 7
Filter sehingga wireshark hanya mengambil paket yang berasal dari ip kalian!
### Jawaban
- Buka terminal lalu lakukan `ipconfig` untuk mendapatkan alamat IP
- Setelah didapat IP lalu lakukan capture wifi dengan capture filter `src host <IP>` dengan IP yang didapat sebelumnya
- paket yang berasal dari IP tersebut akan terfilter
### Screenshot Pengerjaan


## Soal 8-10
Di sebuah planet bernama Viltrumite, terdapat Kementerian Komunikasi dan Informatika yang baru saja menetapkan kebijakan baru. Dalam kebijakan baru tersebut, pemerintah dapat mengakses data pribadi masyarakat secara bebas jika memang dibutuhkan, baik dengan maupun tanpa persetujuan pihak yang bersangkutan. Sebagai mahasiswa yang sedang melaksanakan program magang di kementerian tersebut, kalian mendapat tugas berupa penyadapan percakapan mahasiswa yang diduga melakukan tindak kecurangan dalam kegiatan Praktikum Komunikasi Data dan Jaringan Komputer 2022. Selain itu, terdapat sebuah password rahasia (flag) yang diduga merupakan milik sebuah organisasi bawah tanah yang selama ini tidak sejalan dengan pemerintahan Planet Viltrumite. Tunggu apa lagi, segera kerjakan tugas magang tersebut agar kalian bisa mendapatkan pujian serta kenaikan jabatan di kementerian tersebut!

### Soal 8
Telusuri aliran paket dalam file .pcap yang diberikan, cari informasi berguna berupa percakapan antara dua mahasiswa terkait tindakan kecurangan pada kegiatan praktikum. Percakapan tersebut dilaporkan menggunakan protokol jaringan dengan tingkat keandalan yang tinggi dalam pertukaran datanya sehingga kalian perlu menerapkan filter dengan protokol yang tersebut.

#### Jawaban
- Buka paket, lalu follow TCP stream paket apapun
- Ubah stream yang terletak pada bagian kanan bawah sampai ditemukan pesan yang berguna yaitu pada stream 12, dimana terdapat informasi yaitu metode enkripsi yang digunakan (des3), adanya file salt, clue password, dan protokol yang digunakan (9002).
![image](https://user-images.githubusercontent.com/85059763/192078297-ac7faceb-c1bd-4163-8d62-9179acbd4784.png)
- Setelah dicari di internet dengan keyword `9002 protocol` ditemukan bahwa port dapat menggunakan protokol TCP/UDP, karena dicari protokol yang tingkat keandalannya tinggi maka jawaban nomor 8 adalah TCP (sesuai Follow -> TCP Stream)  
![image](https://user-images.githubusercontent.com/85059763/192078365-5c4823a2-e8c4-4efe-a6be-36d32cc11ce0.png)

### Soal 9
Terdapat laporan adanya pertukaran file yang dilakukan oleh kedua mahasiswa dalam percakapan yang diperoleh, carilah file yang dimaksud! Untuk memudahkan laporan kepada atasan, beri nama file yang ditemukan dengan format [nama_kelompok].des3 dan simpan output file dengan nama “flag.txt”.

#### Jawaban
- Selanjutnya, ubah stream dengan cara yang sama sampai stream ke-29, terdapat data dengan awalan `Salted__` sehingga file salt ditemukan
![image](https://user-images.githubusercontent.com/85059763/192078538-846c1e4e-a417-425e-9179-e1d67cb8b331.png)
- Akan tetapi, data perlu diubah dengan Show data as Raw karena jika menggunakan ASCII terdapat data loss
![image](https://user-images.githubusercontent.com/85059763/192078564-bb7aceda-4f9c-4264-a25f-fdda4a40403a.png)
- Save file dengan nama `E07.des3` sesuai format dari soal. Lalu [gunakan openssl](https://osxdaily.com/2012/01/30/encrypt-and-decrypt-files-with-openssl/) dengan `openssl des3 -d -in E07.des3 -out flag.txt` agar nama output file sesuai dengan ketentuan soal.
![image](https://user-images.githubusercontent.com/85059763/192078631-a023376f-7e9d-4b12-b0e9-9243ebbc9913.png)
- Karena diminta decryption password maka clue password dicari di internet dengan keyword `karakter anime kembar lima` sampai ditemukan [halaman database](https://myanimelist.net/anime/38101/5-Toubun_no_Hanayome/) yang berisi nama karakter
![image](https://user-images.githubusercontent.com/85059763/192078773-1ccb22fe-6958-466d-92ec-d4412f57f6bc.png)
- Selanjutnya dilakukan brute force nama, lalu berdasarkan clue pada stream 90 yaitu terdapat kesamaan maka dicoba nama keluarga karakter yang memiliki frekuensi tinggi yaitu `nakano` dan `uesugi` (Jika password salah terdapat notifikasi `bad decrypt`)
![image](https://user-images.githubusercontent.com/85059763/192078805-dcfa7462-79f1-43b8-9491-90f2c84604a8.png)
- Setelah dicoba password `nakano` ternyata didapat hasil dekripsi yang readable
![image](https://user-images.githubusercontent.com/85059763/192078851-4b18616a-9ee0-47f6-9c35-763bff160559.png)

### Soal 10
Temukan password rahasia (flag) dari organisasi bawah tanah yang disebutkan di atas!
Note: Terkait soal nomor 9 dan 10, file yang didapatkan tidak perlu dikumpulkan, cukup tulis flag yang didapatkan ke dalam laporan kalian 🙏.

#### Jawaban
Flag yang ditemukan adalah `JaRkOm2022{8uK4N_CtF_k0k_h3h3h3}`

## Pembagian Tugas
| Nama                        | Nomor      |
|:---------------------------:|:----------:|
| Arya Nur Razzaq             | 3, 4, 5, 6 |
| Florentino Benedictus       | 8, 9, 10   |
| Muhammad Zufarrifqi Prakoso | 1, 2, 7    |

## Revisi
Tidak ada

## Kendala
Tidak ada


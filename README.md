# Jarkom-Modul-1-E07-2022
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

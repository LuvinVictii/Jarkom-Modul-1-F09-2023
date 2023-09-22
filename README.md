# Jarkom-Modul-1-F09-2023


## Soal 1
### User melakukan berbagai aktivitas dengan menggunakan protokol FTP. Salah satunya adalah mengunggah suatu file
> a. Berapakah sequence number (raw) pada packet yang menunjukkan aktivitas tersebut? <br> b. Berapakah acknowledge number (raw) pada packet yang menunjukkan aktivitas tersebut?

Langkah menemukan jawaban 1a dan 1b:
1.	Request “STOR” menunjukkan aktivitas awal
2.	Responsnya didapati di bawah request
3.	Lalu buka filter FTP dan cari respon pada STOR
4.	Sequence number dan acknowledgement number dapat dilihat


> c. Berapakah sequence number (raw) pada packet yang menunjukkan response dari aktivitas tersebut?<br>d. Berapakah acknowledge number (raw) pada packet yang menunjukkan response dari aktivitas tersebut?

Langkah menemukan jawaban 1c dan 1d :
1.	Buka respons
2.	Lihat sequence dan acknowledgement number


## Soal 2
### Sebutkan web server yang digunakan pada portal praktikum Jaringan Komputer!

Langkah pengerjaan : 
1.	Filter http
2.	Cari domain yang sesuai dengan domain jarkom
3.	Lihat server

## Soal 3
### Dapin sedang belajar analisis jaringan. Bantulah Dapin untuk mengerjakan soal berikut:
> a. Berapa banyak paket yang tercapture dengan IP source maupun destination address adalah 239.255.255.250 dengan port 3702? <br> b. Protokol layer transport apa yang digunakan?

1.	Filter sesuai gambar
2.	Hitung paket
3.	Lihat protokol yang digunakan (tertera UDP)

## Soal 4
### Berapa nilai checksum yang didapat dari header pada paket nomor 130?

Langkah pengerjaan: 
1.	Filter frame number 130
2.	Klik port yang muncul
3.	Cari checksum

## Soal 5
### Elshe menemukan suatu file packet capture yang menarik. Bantulah Elshe untuk menganalisis file packet capture tersebut.

Langkah pengerjaan:

> a. Berapa banyak packet yang berhasil di capture dari file pcap tersebut? <br> b. Port berapakah pada server yang digunakan untuk service SMTP? <br> c. Dari semua alamat IP yang tercapture, IP berapakah yang merupakan public IP?

1.	Filter smtp
2.	Cari yang di smtp terdapat password
3.	Decode password menggunakan base64
4.	Ditemukan 5implePas5word
5.	Buka txt dan masukan nc ke cmd
6.	Hitung paket pada pcap
7.	Lihat destination port
8.	IP 10 adalah milik ITS. Maka kita ambil yang protokolnya smtp selain 10 (source: Pak Bas)


## Soal 6
### Seorang anak bernama Udin Berteman dengan SlameT yang merupakan seorang penggemar film detektif. sebagai teman yang baik, Ia selalu mengajak slamet untuk bermain valoranT bersama. suatu malam, terjadi sebuah hal yang tak terdUga. ketika udin mereka membuka game tersebut, laptop udin menunjukkan sebuah field text dan Sebuah kode Invalid bertuliskan "server SOURCE ADDRESS 7812 is invalid". ketika ditelusuri di google, hasil pencarian hanya menampilkan a1 e5 u21. jiwa detektif slamet pun bergejolak. bantulah udin dan slamet untuk menemukan solusi kode error tersebut. <br>

## Soal 7
### Berapa jumlah packet yang menuju IP 184.87.193.88?

Langkah pengerjaan:
1.	Filter ip destination sesuai soal
2.	Hitung port yang muncul


## Soal 8
### Berikan kueri filter sehingga wireshark hanya mengambil semua protokol paket yang menuju port 80! (Jika terdapat lebih dari 1 port, maka urutkan sesuai dengan abjad)
Langkah pengerjaan:
1.	Yaa filter aja hehe

## Soal 9
### Berikan kueri filter sehingga wireshark hanya mengambil paket yang berasal dari alamat 10.51.40.1 tetapi tidak menuju ke alamat 10.39.55.34!

Langkah pengerjaan
1.  Sama kayak nomor 8

## Soal 10
### Sebutkan kredensial yang benar ketika user mencoba login menggunakan Telnet

Langkah pengerjaan:
1.	Filter telnet
2.	Cari satu-satu hehe


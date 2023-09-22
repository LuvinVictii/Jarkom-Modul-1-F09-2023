# Jarkom-Modul-1-F09-2023

# **Anggota Kelompok**

| Nama                      | NRP        |
| ------------------------- | ---------- |
| Muhammad Daffa Harits                | 5025211005 |
| Muhammad Naufal Baihaqi       | 5025211103 |

## Soal 1
### User melakukan berbagai aktivitas dengan menggunakan protokol FTP. Salah satunya adalah mengunggah suatu file
![image](https://github.com/LuvinVictii/Jarkom-Modul-1-F09-2023/assets/78089862/57411991-d8f8-4832-996c-4b0021186971)

> a. Berapakah sequence number (raw) pada packet yang menunjukkan aktivitas tersebut? <br> b. Berapakah acknowledge number (raw) pada packet yang menunjukkan aktivitas tersebut?

Langkah menemukan jawaban 1a dan 1b:
1.	Request “STOR” menunjukkan aktivitas awal
2.	Responsnya didapati di bawah request
3.	Lalu buka filter FTP dan cari respon pada STOR
4.	Sequence number dan acknowledgement number dapat dilihat
![image](https://github.com/LuvinVictii/Jarkom-Modul-1-F09-2023/assets/78089862/407196dd-fdba-4e03-a33d-9ffa9ace5dda)

> c. Berapakah sequence number (raw) pada packet yang menunjukkan response dari aktivitas tersebut?<br>d. Berapakah acknowledge number (raw) pada packet yang menunjukkan response dari aktivitas tersebut?

Langkah menemukan jawaban 1c dan 1d :
1.	Buka respons
2.	Lihat sequence dan acknowledgement number
![image](https://github.com/LuvinVictii/Jarkom-Modul-1-F09-2023/assets/78089862/e6a5dc1f-166d-4221-8551-29a8b2115f28)

## Soal 2
### Sebutkan web server yang digunakan pada portal praktikum Jaringan Komputer!
![image](https://github.com/LuvinVictii/Jarkom-Modul-1-F09-2023/assets/78089862/387b6cb0-e5a6-4297-a939-a22c01fe4ec5)

Langkah pengerjaan : 
1.	Filter http
2.	Cari domain yang sesuai dengan domain jarkom
3.	Lihat server
![image](https://github.com/LuvinVictii/Jarkom-Modul-1-F09-2023/assets/78089862/1e0a01ba-afaf-4100-b40e-082628bb3621)

## Soal 3
### Dapin sedang belajar analisis jaringan. Bantulah Dapin untuk mengerjakan soal berikut:
> a. Berapa banyak paket yang tercapture dengan IP source maupun destination address adalah 239.255.255.250 dengan port 3702? <br> b. Protokol layer transport apa yang digunakan?

![image](https://github.com/LuvinVictii/Jarkom-Modul-1-F09-2023/assets/78089862/880f214b-ceb5-4567-a6d7-9108c9176e4a)

1.	Filter sesuai gambar
2.	Hitung paket
3.	Lihat protokol yang digunakan (tertera UDP)
![image](https://github.com/LuvinVictii/Jarkom-Modul-1-F09-2023/assets/78089862/36870ea2-3a77-4738-b85a-3f92610a1d44)

## Soal 4
### Berapa nilai checksum yang didapat dari header pada paket nomor 130?
![image](https://github.com/LuvinVictii/Jarkom-Modul-1-F09-2023/assets/78089862/e1342327-0068-4fd2-8a02-dfdab283c012)

Langkah pengerjaan: 
1.	Filter frame number 130
2.	Klik port yang muncul
3.	Cari checksum
![image](https://github.com/LuvinVictii/Jarkom-Modul-1-F09-2023/assets/78089862/d423276f-b71e-4b57-bd1f-4252f04941f8)

## Soal 5
### Elshe menemukan suatu file packet capture yang menarik. Bantulah Elshe untuk menganalisis file packet capture tersebut.
> a. Berapa banyak packet yang berhasil di capture dari file pcap tersebut? <br> b. Port berapakah pada server yang digunakan untuk service SMTP? <br> c. Dari semua alamat IP yang tercapture, IP berapakah yang merupakan public IP?

![image](https://github.com/LuvinVictii/Jarkom-Modul-1-F09-2023/assets/78089862/d4ed558e-dbd8-4525-92c0-7aa9bcf29813)

Langkah pengerjaan:
1.	Filter smtp
2.	Cari yang di smtp terdapat password
3.	Decode password menggunakan base64
4.	Ditemukan 5implePas5word
5.	Buka txt dan masukan nc ke cmd
6.	Hitung paket pada pcap
7.	Lihat destination port
8.	IP 10 adalah milik ITS. Maka kita ambil yang protokolnya smtp selain 10 (source: Pak Bas)
![image](https://github.com/LuvinVictii/Jarkom-Modul-1-F09-2023/assets/78089862/f7ea71cb-9569-4780-be77-9dad37a24bc3)
![image](https://github.com/LuvinVictii/Jarkom-Modul-1-F09-2023/assets/78089862/8b8b11b7-44eb-4606-8721-6fde9dbd66bc)
![image](https://github.com/LuvinVictii/Jarkom-Modul-1-F09-2023/assets/78089862/81b5b34e-9004-45ab-9873-618cbba4c368)
![image](https://github.com/LuvinVictii/Jarkom-Modul-1-F09-2023/assets/78089862/9c0b0c5c-997b-40cb-9878-7778b6a0870b)

## Soal 6
### Seorang anak bernama Udin Berteman dengan SlameT yang merupakan seorang penggemar film detektif. sebagai teman yang baik, Ia selalu mengajak slamet untuk bermain valoranT bersama. suatu malam, terjadi sebuah hal yang tak terdUga. ketika udin mereka membuka game tersebut, laptop udin menunjukkan sebuah field text dan Sebuah kode Invalid bertuliskan "server SOURCE ADDRESS 7812 is invalid". ketika ditelusuri di google, hasil pencarian hanya menampilkan a1 e5 u21. jiwa detektif slamet pun bergejolak. bantulah udin dan slamet untuk menemukan solusi kode error tersebut. <br>

Pertama-tama, kita mencari source IP address pada packet bernomor 7812.

![image](https://user-images.githubusercontent.com/115441787/269955543-872f6907-0d26-492c-bd00-a0dc50d11cc4.png)

IP address = 104.18.14.101
Selanjutnya, diberitahu bahwa ketika ditelusuri di google, hasil pencarian hanya menampilkan a1 e5 u21. Hal ini merupakan a1z26 cipher encryption. Dengan itu, kita perlu mendecrypt IP yang kita terima dan pada hint ketiga, tertulis bahwa rentang huruf yang digunakan hanya Huruf A-R, 1-18. Maka dari itu, untuk angka diatas 18, kita perlu memisahnya menjadi 2 angka, sehingga IP menjadi = 10 4 18 14 10 1.

![image](https://user-images.githubusercontent.com/115441787/269955752-9cbab65c-2980-4110-b145-62d8c7cdb359.png)


## Soal 7
### Berapa jumlah packet yang menuju IP 184.87.193.88?
![image](https://github.com/LuvinVictii/Jarkom-Modul-1-F09-2023/assets/78089862/9ac3d655-4f53-465d-99be-b6d08b475e6a)

Langkah pengerjaan:
1.	Filter ip destination sesuai soal
2.	Hitung port yang muncul
![image](https://github.com/LuvinVictii/Jarkom-Modul-1-F09-2023/assets/78089862/b9d79362-ebc3-40f4-ae38-7c9dd3a79e2f)

## Soal 8
### Berikan kueri filter sehingga wireshark hanya mengambil semua protokol paket yang menuju port 80! (Jika terdapat lebih dari 1 port, maka urutkan sesuai dengan abjad)
![image](https://github.com/LuvinVictii/Jarkom-Modul-1-F09-2023/assets/78089862/23922cf5-cd0d-4968-8cfd-9b851fe71cdf)

Hasil kueri:
![image](https://github.com/LuvinVictii/Jarkom-Modul-1-F09-2023/assets/78089862/338c67d5-12f5-4642-88cb-06e262eba030)

## Soal 9
### Berikan kueri filter sehingga wireshark hanya mengambil paket yang berasal dari alamat 10.51.40.1 tetapi tidak menuju ke alamat 10.39.55.34!
![image](https://github.com/LuvinVictii/Jarkom-Modul-1-F09-2023/assets/78089862/f9cdb056-2fd4-4add-b7d4-9394040a2d59)

Hasil kueri:
![image](https://github.com/LuvinVictii/Jarkom-Modul-1-F09-2023/assets/78089862/150700d9-6e80-455c-8513-a6ca3c9c22bf)

## Soal 10
### Sebutkan kredensial yang benar ketika user mencoba login menggunakan Telnet
![image](https://github.com/LuvinVictii/Jarkom-Modul-1-F09-2023/assets/78089862/fc9d6a2d-3690-452d-be90-75be59eb3523)

Langkah pengerjaan:
1.	Filter telnet
2.	Bruteforce
![image](https://github.com/LuvinVictii/Jarkom-Modul-1-F09-2023/assets/78089862/c355aa34-77dd-46bd-840d-adbcaddfc2d8)




# KENDALA 

1. Susah untuk connect dengan VPN ITS sehingga mengurangi waktu praktikum
2. Lambatnya koneksi wifi





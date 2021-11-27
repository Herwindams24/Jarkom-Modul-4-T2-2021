# Lapres Modul 4 Jarkom 2021 - T02
Laporan Hasil Praktikum Modul 4 Jarkom 2021
Kelompok T02
  * Herwinda Marwaa Salsabila (05311940000009)
  * Dian Arofati N. Z. (05311940000011)
  * Dava Aditya Jauhar (05311940000030)

---

## Persiapan

   **Soal**
    
   Pertama-tama buatlah pembagian subnet terhadap topologi soal. Berikut merupakan gambar topologi yang telah dibagi subnet:
   
<img src="https://user-images.githubusercontent.com/57520495/143676636-69f4fc74-86ea-4ef4-aa87-86b3663df461.png" width="500">

Hasil pembagian subnet yang kami dapat adalah **15 Subnet**. Dengan Subnet A1 kami ambil dari yang paling jauh dari Foosha.

   **Jawaban**

## VLSM
   
   **Perhitungan dan pembagian IP**
   
Tentukan jumlah IP address yang dibutuhkan per subnet dari total subnet yang sebelumnya telah ditentukan, yaitu 15 subnet.
   
| Subnet | Jumlah IP | Netmask |
| --- | --- | --- |
| A1 | 721 | /22 |
| A2 | 252 | /24 |
| A3 | 2 | /30 |
| A4 | 521 | /22 |
| A5 | 13 | /28 |
| A6 | 502 | /23 |
| A7 | 2 | /30 |
| A8 | 2 | /30 |
| A9 | 1001 | /22 |
| A10 | 701 | /22 |
| A11 | 2 | /30 |
| A12 | 2021 | /21 |
| A13 | 101 | /25 |
| A14 | 2 | /30 |
| A15 | 2 | /30 |
| Total | 5845 | /19 |


Total jumlah IP addres didapatkan adalah 5845, sehingga masuk ke dalam netmask /19. Setelah itu, kami bentuk subnet paling besar dengan NID 192.212.0.0 dan netmask /19. Lalu, lakukan pembagian IP dengan bantuan IP tree seperti gambar berikut:
   
   <img src="https://user-images.githubusercontent.com/57520495/143677310-079eaa6a-d172-4c4c-8704-8e5bb5305373.png" width="500">
   
Dapatkan perhitungan broadcast dari IP tree (Network ID dan Netmask). Pada contoh ini, kami tunjukan perhitungan Broadcast Addr seperti pada gambar menggunakan NID A1 yaitu 192.212.26.0 dan Netmask /24:
  
   <img src="https://user-images.githubusercontent.com/57980125/143682739-cb092233-eb73-4535-866a-1e0f2db12b37.png" width="500">

Berikut merupakan tabel rangkuman untuk sebuah subnet yang memiliki NID, Netmask, dan Broadcast Address yang berhasil kami dapatkan:

   <img src="https://user-images.githubusercontent.com/57520495/143677234-6af41b07-ef6a-4c29-83da-811b15704605.png" width="500">
   
Setting IP pada tiap interface yang ada di setiap device sesuai dengan pembagian subnet pada pohon VLSM. Sebagi berikut:
   
   1. Pada Foosha
  
  - Konfigurasi Foosha
  
  <img src="image/routing foosha ke a11&a3.jpg" width="500">
  
   - Uji coba ping `Foosha` ke `chiper`
   
   <img src="image/foosha ke chiper.png" width="500">

   - Uji coba ping `Foosha` ke `Elena`
   
   <img src="image/foosha ke elena.png" width="500">
   
   - Uji coba ping `Foosha` ke `Jipangu`
   
   <img src="image/foosha ke jipangu.png" width="500">
   
   - Uji coba ping `Foosha` ke `Jorge`
   
   <img src="image/foosha ke jorge.png" width="500">
        
   - Uji coba ping `Foosha` ke `Oimo`
   
   <img src="image/foosha ke oimo.png" width="500">
        
   - Uji coba ping `Foosha` ke `Google`
   
   <img src="image/foosha ping google.jpg" width="500">

   2. Pada Blueno
   
        <img src="https://user-images.githubusercontent.com/57980125/143683389-270397d0-8ef8-40fe-a173-b9c070420acc.png)" width="500">
   
   3. Pada Water7
   
   - Konfigurasi Water7 Static
   
     ![PacketTracer_5QcB5cOlxg](https://user-images.githubusercontent.com/57980125/143683443-83ece41e-2c9f-4a1d-8cd2-c661f39af7a9.png)
     
   - Konfigurasi Water7 Interface
   
   <img src="image/cpt_water7_fa01.jpg" width="500">
   
   ![PacketTracer_JhOwCdBsLA](https://user-images.githubusercontent.com/57980125/143683460-0951cf34-aa08-4a5c-8448-5bb342751b2d.png)
   
   ![PacketTracer_FYJOswy9qo](https://user-images.githubusercontent.com/57980125/143683461-f55f4a01-f021-411f-a9a0-67d7f29c4bf1.png)

   
   4. Pada Chiper
    
        <img src="https://user-images.githubusercontent.com/57980125/143683482-2b35546c-3de5-45c4-8fa6-b01cc1d5cd52.png" width="500">
   
   5. Pada Pucci
   
   -Konfigurasi Pucci Static
   
   ![PacketTracer_7QJp7rV0nA](https://user-images.githubusercontent.com/57980125/143683512-99a5228c-ce65-420d-a1ca-5c1606a57f1c.png)

   -Konfigurasi Pucci Interface
   
   ![PacketTracer_a3Efn5axym](https://user-images.githubusercontent.com/57980125/143683529-2cc8dec4-ba79-478e-9517-0e452321cb6e.png)
   
   ![PacketTracer_0SPKMmfzEO](https://user-images.githubusercontent.com/57980125/143683532-7ba0cc27-19b0-4d23-94e8-1cc65ed62387.png) 
   
   <img src="image/cpt_pucci_fa00.jpg" width="500">
   
   6. Pada Calmbelt
   
        <img src="https://user-images.githubusercontent.com/57980125/143683557-6d498d8f-e483-474c-b3cb-50984b723a42.png" width="500">
   
   7. Pada Courtyard
   
        <img src="https://user-images.githubusercontent.com/57980125/143683574-8a326fb4-afc3-40d0-a540-2ea0dc7bcf59.png" width="500">
   
   8. Pada Jipangu
   
   - Uji coba ping `jipangu` ke `Jorge`
   
   <img src="image/jipangu ke jorge.png" width="500">

   - Uji coba ping `jipangu` ke `Elena`
   
   <img src="image/jipangu ke Elena.png" width="500">
   
   - Uji coba ping `jipangu` ke `Google`
   
   <img src="image/jipangu ke google.png" width="500">
   
   9. Pada Doriki
   
        <img src="https://user-images.githubusercontent.com/57980125/143683609-8b135fc0-93eb-4d2b-b395-597f3a640e6f.png" width="500">
   
   10. Pada Guanhao
   
   -  Konfigurasi Guanhao Static
   
       ![PacketTracer_kZhSnUDefc](https://user-images.githubusercontent.com/57980125/143683668-33a9627a-b676-4aae-8b6e-3dde92209ca0.png)

       ![PacketTracer_4cu7kFgiRW](https://user-images.githubusercontent.com/57980125/143683675-841bff35-c714-4135-9b17-56b68aafdf5a.png)

   
   -  Konfigurasi Guanhao Interface
   
        <img src="https://user-images.githubusercontent.com/57980125/143683699-32c409a3-e4ea-40f1-afc4-34abd780594d.png" width="500">
        
        <img src="https://user-images.githubusercontent.com/57980125/143683700-31456ab6-1fdd-41dd-a94e-61f6d0da8cfa.png" width="500">
        
        <img src="https://user-images.githubusercontent.com/57980125/143683704-7ac40611-04de-40a7-85c3-633626534541.png" width="500">
        
        <img src="https://user-images.githubusercontent.com/57980125/143683705-6e9fe233-d77b-45eb-a0df-21b0ab5db996.png" width="500">
   
   11. Pada Jabra
   
        <img src="https://user-images.githubusercontent.com/57980125/143683740-104764d1-0334-47fe-b3da-fbed0390accd.png" width="500">
   
   12. Pada Maingate
   
        <img src="https://user-images.githubusercontent.com/57980125/143683753-277d3bbf-6f35-4d09-88ef-44f340164602.png" width="500">
   
   13. Pada Alabasta
   
   - Konfigurasi Alabasta Static
        
        <img src="https://user-images.githubusercontent.com/57980125/143683845-4fabd114-007e-466c-b4bf-91cf041f3887.png" width="500">
   
   - Konfigurasi Alabasta Interface
        
        <img src="https://user-images.githubusercontent.com/57980125/143683842-5e8375ab-67ad-49eb-ba82-7240f33d8d0a.png" width="500">
        
        <img src="https://user-images.githubusercontent.com/57980125/143683839-77246c26-fd8a-40b4-bc14-4eea7ea02ba4.png" width="500">
        
   14. Pada Jorge
   
        <img src="https://user-images.githubusercontent.com/57980125/143683876-4dd9081d-9262-476d-a8b0-d4846ef6d3fc.png" width="500">
   
   15. Pada Oimo
   
   - Uji coba ping `Oimo` ke `Chiper`

        <img src="https://user-images.githubusercontent.com/57520495/143682374-f98daf97-7a7c-45f6-8637-947e1892e340.png" width="500">
        
   - Uji coba ping `Oimo` ke `Pucci`

        <img src="https://user-images.githubusercontent.com/57520495/143682419-45e27eaf-5872-478b-98ea-3828ee98c4bb.png" width="500">
   
   16. Pada Fukurou
   
        <img src="https://user-images.githubusercontent.com/57980125/143683935-98e7fe71-721a-498b-a39f-8acb9ff88070.png" width="500">
   
   17. Pada EniesLobby
   
        <img src="https://user-images.githubusercontent.com/57980125/143683925-18ff7d3e-ddf9-4192-b8a1-9686150c0fe5.png" width="500">
   
   18. Pada Seastone
   
        <img src="![PacketTracer_20IN6aEFeH](https://user-images.githubusercontent.com/57980125/143683998-78e1b439-78c6-48a4-bebe-16bf9adb2e0b.png)
" width="500">
       
        ![PacketTracer_EhDXH5N8pQ](https://user-images.githubusercontent.com/57980125/143684005-cda661b7-f846-48dc-ab70-d2878a3c78d8.png)

        ![PacketTracer_ETrIGZbmQD](https://user-images.githubusercontent.com/57980125/143684017-f12aaff7-0aec-4cbf-846b-5786881d1664.png)

   
   19. Pada Elena
   
   ![PacketTracer_n1Jw99MDEC](https://user-images.githubusercontent.com/57980125/143683929-1634748a-76c3-476c-9001-1cf58b06c840.png)

        
       
---
## CIDR

Pertama, buat satu node yang terhubung dengan internet dengan nama NAT1 dan sambungkan dengan router foosha melalui interface `nat0` menuju interface `eth0`.
Selanjutnya, tempatkan node-node yang lain seperti pada soal.

Tentukan subnet yang ada dalam topologi dan melakukan labelling netmask terhadap masing-masing subnet. Gabungkan subnet paling bawah di dalam topologi. Paling bawah berarti subnet yang paling jauh dari internet.
Penggabungan dan pengelompokkan subnet dapat dilihat pada gambar berikut:

   <img src="https://user-images.githubusercontent.com/57520495/143677792-55fd3842-a3fb-45a4-9892-4866b84c043d.png" width="500">
      
   <img src="https://user-images.githubusercontent.com/57520495/143677842-e8183a64-9502-4556-9ebf-00210e1ae116.png" width="500">

   <img src="https://user-images.githubusercontent.com/57520495/143678077-80752831-45fe-4b5b-a090-6a67fc250e0b.png" width="500">
   
Subnet C akan digabungkan menjadi 2 subnet yang lebih besar yang dinamakan **D1** dan **D2**. **D1** dan **D2** menjadi **E1**   

   <img src="https://user-images.githubusercontent.com/57520495/143678161-4c12c744-6035-4b84-b284-4cdf04fd3571.png" width="500">

   **Perhitungan dan pembagian IP**
   List subnet-nestmask ada setelah penggabungan ini didapatkan dengan menggunakan teknik CIDR subnet gabungan yang akan memiliki netmask yang 1 tingkat di atas subnet terbesar yang digabungkan
   
| Subnet | Jumlah IP | Netmask |
| --- | --- | --- |
| A1 | 721 | /22 |
| A2 | 252 | /24 |
| A3 | 2 | /30 |
| A4 | 521 | /22 |
| A5 | 13 | /28 |
| A6 | 502 | /23 |
| A7 | 2 | /30 |
| A8 | 2 | /30 |
| A9 | 1001 | /22 |
| A10 | 701 | /22 |
| A11 | 2 | /30 |
| A12 | 2021 | /21 |
| A13 | 101 | /25 |
| A14 | 2 | /30 |
| A15 | 2 | /30 |
| Total | 5845 | /19 |

   Tabel penggabungan subnet

| Subnet | Asal Subnet | Netmask |
| --- | --- | --- |
| B1 | A1 + A2 | /21 |
| B2 | A3 + A14 | /29 |
| B3 | A7 + A4 | /21 |
| B4 | A6 + A5 | /22 |
| B5 | A12 + A13 | /20 |
| B6 | A10 + A11 | /21 |
| B7 | A8 + A9 | /21 |
| C1 | B1 + B2 | /20 |
| C2 | B3 + B4 | /20 |
| C3 | B5 + B6 | /19 |
| C4 | B7 + A15 | /20 |
| D1 | C1 + C2 | /19 |
| D2 | C3 + C4 | /18 |
| E1 | D1 + D2 | /17 |
   
   Tabel pembagian IP
   
   Buat Tree CIDR dengan cara penggabungan Subnet seperti pada gambar Topologi yang telah dikelompokkan dan ip addres netmask dari masing-masing subnet:
   
   <img src="https://user-images.githubusercontent.com/57980125/143683224-4292ebf0-54f4-4ca2-b564-8726f874fa69.jpg" width="500">

   Berikut merupakan tabel hasil perhitungan Broadcast Address dari setiap subnet A1-A15:
   
   <img src="https://user-images.githubusercontent.com/57520495/143677745-64fc543b-5153-4e81-b085-3633bfef72fe.png" width="500">
  
 Selanjutnya, lakukan konfigurasi terlebih dahulu disetiap router, server, dan PC:
   
   **Pengaturan pada tiap node**
   1. Pada Foosha

        <img src="" width="500">

   2. Pada Blueno
   
        <img src="" width="500">
   
   3. Pada Water7
   
       <img src="" width="500">
   
   4. Pada Chiper
    
        <img src="" width="500">
   
   5. Pada Pucci
   
        <img src="" width="500">
   
   6. Pada Calmbelt
   
        <img src="" width="500">
   
   7. Pada Courtyard
   
        <img src="" width="500">
   
   8. Pada Jipangu
   
        <img src="" width="500">
   
   9. Pada Doriki
   
        <img src="" width="500">
   
   10. Pada Guanhao
   
        <img src="" width="500">
   
   11. Pada Jabra
   
        <img src="" width="500">
   
   12. Pada Maingate
   
        <img src="" width="500">
   
   13. Pada Alabasta
   
        <img src="" width="500">
   
   14. Pada Jorge
   
        <img src="" width="500">
   
   15. Pada Oimo
   
        <img src="" width="500">
   
   16. Pada Fukurou
   
        <img src="" width="500">
   
   17. Pada EniesLobby
   
        <img src="" width="500">
   
   18. Pada Seastone
   
        <img src="" width="500">
   
   19. Pada Elena
   
   - Uji coba ping `Elena` ke `Doriki`
   
   <img src="image/elena ke doriki.png" width="500">

   - Uji coba ping `Elena` ke `Fukurou`
   
   <img src="image/elena ke fukurou.png" width="500">
   
   - Uji coba ping `Elena` ke `Jipangu`
   
   <img src="image/elena ke jipangu.png" width="500">
        
   - Uji coba ping `Elena` ke `Jorge`
   
   <img src="image/elena ping jorge.jpg" width="500">
        
   - Uji coba ping `Elena` ke `Google`
   
   <img src="image/elena ping google.jpg" width="500">
   
   
---

## Kendala

1. Awalnya kesulitan saat menggabungkan tiap subnet pada metode CIDR dan sempat menyentuh subnet /15 yang mana harus menambah oktet ke-2.
2. Sudah sulit, mengerjakannya juga kurang teliti, ya mengulang deh jadinya.
3. Ada ketidakjelasan informasi pada soal sehingga cukup kebingungan saat mengerjakan.
4. Salah satu anggota kelompok kebetulan ada keperluan mendesak (lomba) yang menyebabkan ketidaklengkapan anggota kelompok yang mengerjakan.
5. Saat dijalankan ada beberapa konfigurasi yang kurang tepat sehingga tidak sesuai harapan.

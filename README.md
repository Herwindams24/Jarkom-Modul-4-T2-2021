# Lapres Modul 4 Jarkom 2021 - T02
Laporan Hasil Praktikum Modul 4 Jarkom 2021
Kelompok T02
  * Herwinda Marwaa Salsabila (05311940000009)
  * Dian Arofati N. Z. (05311940000011)
  * Dava Aditya Jauhar (05311940000030)

---

## Persiapan

   **Soal**
    
   Buatlah topologi seperti berikut dan tentukan subnetting serta routingnya
   
<img src="https://user-images.githubusercontent.com/57520495/143676636-69f4fc74-86ea-4ef4-aa87-86b3663df461.png" width="500">

---

Link miro: https://miro.com/welcomeonboard/SmtrWnF2VDZ6SzBseHhSbmJzeU16SWlvaDhOM1FVOXJGeng5WVd4Z1NtRzZKUE5QNTUybEZOU1oyaXh2NlBGRXwzMDc0NDU3MzYwMzk1NTk1NDg2?invite_link_id=708907599398
Pakek email its yaa

---

   **Jawaban**

## VLSM
   
   **Perhitungan dan pembagian IP**
   
   Tabel jumlah IP dibutuhkan pada tiap subnet
   
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
   
   Tabel pembagian IP
   
   <img src="https://user-images.githubusercontent.com/57520495/143677234-6af41b07-ef6a-4c29-83da-811b15704605.png" width="500">
   
   Topologi VLSM
   
   <img src="https://user-images.githubusercontent.com/57520495/143677310-079eaa6a-d172-4c4c-8704-8e5bb5305373.png" width="500">
   
   **Pengaturan pada tiap node**
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
   
        <img src="" width="500">
   
   3. Pada Water7
   
   - Konfigurasi Water7
   
   <img src="image/cpt_water7_fa01.jpg" width="500">
   
   4. Pada Chiper
    
        <img src="" width="500">
   
   5. Pada Pucci
   
   -Konfigurasi Pucci
   
   <img src="image/cpt_pucci_fa00.jpg" width="500">
   
   6. Pada Calmbelt
   
        <img src="" width="500">
   
   7. Pada Courtyard
   
        <img src="" width="500">
   
   8. Pada Jipangu
   
   - Uji coba ping `jipangu` ke `Jorge`
   
   <img src="image/jipangu ke jorge.png" width="500">

   - Uji coba ping `jipangu` ke `Elena`
   
   <img src="image/jipangu ke Elena.png" width="500">
   
   - Uji coba ping `jipangu` ke `Google`
   
   <img src="image/jipangu ke google.png" width="500">
   
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
   
   - Uji coba ping `Oimo` ke `Chiper`

        <img src="https://user-images.githubusercontent.com/57520495/143682374-f98daf97-7a7c-45f6-8637-947e1892e340.png" width="500">
        
   - Uji coba ping `Oimo` ke `Pucci`

        <img src="https://user-images.githubusercontent.com/57520495/143682419-45e27eaf-5872-478b-98ea-3828ee98c4bb.png" width="500">
   
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
## CIDR
   
   **Perhitungan dan pembagian IP**
   Tabel jumlah IP dibutuhkan pada tiap subnet
   
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
   
   <img src="https://user-images.githubusercontent.com/57520495/143677745-64fc543b-5153-4e81-b085-3633bfef72fe.png" width="500">
   
   Topologi CIDR
   
   <img src="https://user-images.githubusercontent.com/57520495/143677792-55fd3842-a3fb-45a4-9892-4866b84c043d.png" width="500">
      
   <img src="https://user-images.githubusercontent.com/57520495/143677842-e8183a64-9502-4556-9ebf-00210e1ae116.png" width="500">
   
   <img src="https://user-images.githubusercontent.com/57520495/143678077-80752831-45fe-4b5b-a090-6a67fc250e0b.png" width="500">
   
   <img src="https://user-images.githubusercontent.com/57520495/143678161-4c12c744-6035-4b84-b284-4cdf04fd3571.png" width="500">
   
   
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
   
        <img src="" width="500">
       
---

## Kendala

1. Awalnya kesulitan saat menggabungkan tiap subnet pada metode CIDR dan sempat menyentuh subnet /15 yang mana harus menambah oktet ke-2.
2. Sudah sulit, mengerjakannya juga kurang teliti, ya mengulang deh jadinya.
3. Ada ketidakjelasan informasi pada soal sehingga cukup kebingungan saat mengerjakan.
4. Salah satu anggota kelompok kebetulan ada keperluan mendesak (lomba) yang menyebabkan ketidaklengkapan anggota kelompok yang mengerjakan.
5. Saat dijalankan ada beberapa konfigurasi yang kurang tepat sehingga tidak sesuai harapan.

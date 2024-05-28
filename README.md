# Praktikum-4

## TUGAS PRAKTIKUM 4 (TABEL PEGAWAI)
1.	Tampilkan pegawai yang gajinya bukan 2.000.000 dan 1.250.000 !
2.	Tampilkan pegawai yang tunjangannya NULL!
3.	Tampilkan pegawai yang tunjangannya tidak NULL!
4.	Tampilkan/hitung jumlah baris/record tabel pegawai!
5.	Tampilkan/hitung jumlah total gaji di tabel pegawai!
6.	Tampilkan/hitung rata-rata gaji pegawai!
7.	Tampilkan gaji terkecil!
8.	Tampilkan gaji terbesar!

PENJELASAN


### 1.	Tampilkan pegawai yang gajinya bukan 2.000.000 dan 1.250.000 !

Jawab :

Untuk perintahnya bisa menggunkan perintah seperti ini :

`SELECT * FROM pegawai WHERE gajih NOT IN (2000000, 1250000);`

Dan hasilnya akan seperti ini :

![1](https://giths://github.com/RakaMuzakki/Raka_Muzakki/assets/170961426/81a7c3be-1eb7-457c-a882-633b25ec9be8)

### 2.	Tampilkan pegawai yang tunjangannya NULL!

Jawab :

Untuk perintahnya bisa menggunkan perintah seperti ini :

`SELECT * FROM pegawai WHERE tunjangan IS NULL; `

Dan hasilnya akan seperti ini :

![Screenshot 2024-05-28 104941](https://github.com/RakaMuzakki/Raka_Muzakki/assets/170961426/461d862d-f084-43de-bd86-b28363517592)

### 3.	Tampilkan pegawai yang tunjangannya tidak NULL!

Jawab :

Untuk perintahnya bisa menggunkan perintah seperti ini :
	
`SELECT * FROM pegawai WHERE tunjangan IS NOT NULL;`

Dan hasilnya akan seperti ini :

![Screenshot 2024-05-28 104948](https://github.com/RakaMuzakki/Raka_Muzakki/assets/170961426/f2eec9d4-e345-4dc3-aa8c-ee293814bc02)

## HASIL DARI 1 - 3

![Screenshot 2024-05-28 105002](https://github.com/RakaMuzakki/Raka_Muzakki/assets/170961426/36b58b48-96f9-40cc-bcfe-67c8b30db63c)

### 4.	Tampilkan/hitung jumlah baris/record tabel pegawai!

Jawab :

Untuk perintahnya bisa menggunkan perintah seperti ini :

`SELECT COUNT(*) AS jumlah_baris FROM pegawai;`

Dan hasilnya akan seperti ini :

![Screenshot 2024-05-28 105010](https://github.com/RakaMuzakki/Raka_Muzakki/assets/170961426/68270679-824f-4c7b-84f7-1669df1deb7c)

### 5.	Tampilkan/hitung jumlah total gaji di tabel pegawai!

Jawab :

Untuk perintahnya bisa menggunkan perintah seperti ini :


`SELECT SUM(gaji) AS total_gaji FROM pegawai; `

Dan hasilnya akan seperti ini :

![Screenshot 2024-05-28 105028](https://github.com/RakaMuzakki/Raka_Muzakki/assets/170961426/596caa7e-e2ee-40e6-8c1e-2c54d2fe1f84)

### 6.	Tampilkan/hitung rata-rata gaji pegawai!

Jawab 

Untuk perintahnya bisa menggunkan perintah seperti ini :

`SELECT AVG(gaji) AS rata_gaji FROM pegawai`

Dan hasilnya akan seperti ini :

![Screenshot 2024-05-28 105037](https://github.com/RakaMuzakki/Raka_Muzakki/assets/170961426/fd68ab30-a462-4890-a333-9506b4b2b9b2)

### 7.	Tampilkan gaji terkecil!

Jawab :

Untuk perintahnya bisa menggunkan perintah seperti ini :

`SELECT MIN(gaji) AS gaji_terkecil FROM pegawai;`

Dan hasilnya akan seperti ini :

![Screenshot 2024-05-28 105045](https://github.com/RakaMuzakki/Raka_Muzakki/assets/170961426/b4666015-370e-4746-90ec-7e61fd20cc67)

### 8.	Tampilkan gaji terbesar!

Jawab 

Untuk perintahnya bisa menggunkan perintah seperti ini :

`SELECT MAX(gaji) AS gaji_terbesar FROM pegawai;`

Dan hasilnya akan seperti ini :

![Screenshot 2024-05-28 105057](https://github.com/RakaMuzakki/Raka_Muzakki/assets/170961426/5d10352b-d52c-4b41-ae98-694989c8cf68)

## TUGAS PRAKTIKUM 4 (TABEL HEWAN)
1.	Tampilkan jumlah hewan yang dimiliki setiap owner
2.	Tampilkan jumlah hewan berdasarkan spesies
3.	Tampilkan jumlah hewan berdasarkan jenis kelamin
4.	Tampilkan jumlah hewan berdasarkan spesies dan jenis kelamin
5.	Tampilkan jumlah hewan berdasarkan spesis (cat dan dog saja) dan jenis kelamin
6.	Tampilkan jumlah hewan berdasarkan jenis kelamin yang diketahui saja

PENJELASAN

### 1. Tampilkan jumlah hewan yang dimiliki setiap owner

Jawab :

Untuk perintahnya bisa menggunkan perintah seperti ini :

`SELECT owner, COUNT(*) AS Jumlah_hewan_setiap_owner FROM hewan GROUP BY owner; `

Dan hasilnya akan seperti ini :

![Screenshot 2024-05-28 105107](https://github.com/RakaMuzakki/Raka_Muzakki/assets/170961426/8f4034f4-8d7a-4210-a692-6590eac5b419)

### 2.	Tampilkan jumlah hewan berdasarkan spesies

Jawab :

Untuk perintahnya bisa menggunkan perintah seperti ini :

`SELECT Species, COUNT(*) AS Jumlah_hewan_berdasarkan_Species FROM hewan GROUP BY Species; `

Dan hasilnya akan seperti ini :

![Screenshot 2024-05-28 105144](https://github.com/RakaMuzakki/Raka_Muzakki/assets/170961426/61354d2b-45bb-4947-b1cd-35fb6068c4bc)

### 3.	Tampilkan jumlah hewan berdasarkan jenis kelamin

Jawab :

Untuk perintahnya bisa menggunkan perintah seperti ini :

`SELECT sex, COUNT(*) AS Jumlah_hewan_berdasarkan_jenis_kelamin FROM hewan GROUP BY sex; `

Dan hasilnya akan seperti ini :

![image](https://github.com/Heryantokurnia/Praktikum-4/assets/141998024/2dba9be5-ee55-4bf0-b742-b4231492f3d0)

### 4.	Tampilkan jumlah hewan berdasarkan spesies dan jenis kelamin

Jawab :

Untuk perintahnya bisa menggunkan perintah seperti ini :

` SELECT species, sex, COUNT(*) AS jumlah FROM hewan GROUP BY species, sex;  `

Dan hasilnya akan seperti ini :

![Screenshot 2024-05-28 105155](https://github.com/RakaMuzakki/Raka_Muzakki/assets/170961426/455cd25d-e2a3-494f-9ce0-87829321ec68)

### 5.	Tampilkan jumlah hewan berdasarkan spesis (cat dan dog saja) dan jenis kelamin

Jawab :

Untuk perintahnya bisa menggunkan perintah seperti ini :

` SELECT species, sex, COUNT(*) AS jumlah FROM hewan WHERE species IN ('cat', 'dog') GROUP BY species, sex;  `

Dan hasilnya akan seperti ini :

![image](https://github.com/Heryantokurnia/Praktikum-4/assets/141998024/2c3dc657-a23a-4053-befe-1e91a888b8cc)

### 6.	Tampilkan jumlah hewan berdasarkan jenis kelamin yang diketahui saja

Jawab :

Untuk perintahnya bisa menggunkan perintah seperti ini :

` SELECT sex, COUNT(*) AS jumlah FROM hewan GROUP BY sex;   `

Dan hasilnya akan seperti ini :

![Screenshot 2024-05-28 105225](https://github.com/RakaMuzakki/Raka_Muzakki/assets/170961426/c615cb93-925c-4b2e-a66b-f5d1ed65f2a0)


# Database Kuliah
Database ini dibuat untuk melatih skill atau pemahaman tentang Database MySQL/MariaDB.

## Tampilan Awal  
![tampilan awal](https://github.com/user-attachments/assets/6bc59937-95f4-49af-bd16-3d555a31ea42)

## No 1
__Perintah__: Update alamat mahasiswa dengan NIM ‘123456’ menjadi ‘Jl. Raya No.5’.  
_UPDATE mahasiswa SET alamat = "Jl. Raya No. 5" WHERE nim = "123456";_   

![no1](https://github.com/user-attachments/assets/195f5d3b-9602-4282-9f72-89a3ba10bb7d)

## No 2  
__Perintah__: Tampilkan nim, nama, dan jurusan dari mahasiswa yang memiliki jurusan ‘Teknik Informatika’, serta tampilkan nama dosen pembimbingnya.  
_SELECT mhs.nim, mhs.nama, mhs.jurusan, mk.dosen_pengajar FROM mahasiswa mhs JOIN mata_kuliah mk ON mhs.nim = mk.nim WHERE mhs.jurusan = "Teknik Informatika";_  

![no2](https://github.com/user-attachments/assets/1a8ceb77-fce4-4c7a-b8e8-7c47ea67e111)  

## No 3  
__Perintah__: Tampilkan 5 nama mahasiswa dengan umur tertua.  
_SELECT nama, umur FROM mahasiswa ORDER BY umur DESC LIMIT 5;_  

![no3](https://github.com/user-attachments/assets/8743b1c6-e916-4abb-a97e-7d4c9066d16a)

## No 4  
__Perintah__: Tampilkan nama mahasiswa, mata kuliah yang diambil, dan nilai yang diperoleh untuk setiap mata kuliah. Hanya tampilkan data mahasiswa yang memiliki nilai lebih bagus dari 70.  
_SELECT mhs.nim, mhs.nama, mhs.alamat, mhs.jurusan, mhs.umur, mk.mata_kuliah, mk.nilai FROM mahasiswa mhs JOIN mata_kuliah mk ON mhs.nim = mk.nim WHERE mk.nilai > 70;_    

![no4](https://github.com/user-attachments/assets/32b212aa-853e-4aef-a3c5-2432bd464bf0)


# Simulasi Pet Cafe

ini adalah program simulasi sederhana Pet Cafe berbasis teks yang memungkinkan pengguna mengelola aktivitas dari 2 jenis karakter  yaitu Pegawai, dan Pet (hewan). Program dengan bahasa pemrograman C ini, memungkinkan pengguna untuk melakukan beberapa aktivitas pada setiap karakter dan melihat status atributnya. Simulasi akan terus berjalan hingga pengguna memutuskan untuk menghentikannya.
## Fitur Utama 
- **Pegawai** : karakter manusia yang dapat melakukan aktivitas istirahat untuk menambah *energy*.
- **Pet** : Hewan peliharaan (anjing atau kucing) yang dapat melakukan aktivitas seperti berjalan-jalan dan berpelukan untuk meningkatkan *loves* dan mempengaruhi *energy*.
- **Memberi makan** : Memberi makan hewan peliharaan untuk meningkatkan *energy*.
- **Menampilkan atribut** : Untuk melihat atribut status dari karakter tertentu.



## Struktur Data
Program menggunakan struct untuk mendefinisikan karakter.

1. Pegawai
- nama : Nama pegawai.
- energy : Tingkat energi pegawai 
- loves : Tingkat kasih sayang yang diterima pegawai.

2. Pet
- nama : Nama hewan peliharaan.
- energy : Tingkat energi hewan peliharaan.
- loves : Tingkat kasih sayang hewan peliharaan.
- Jenis : jenis hewan peliharaan ("anjing" atau "kucing")


## Cara Menggunakan Program 
Program menggunakan perintah berbasis teks. Berikut daftar perintah beserta fungsinya.
- **REST** <nama_pegawai>
  Pegawai beristirahat, *energy* meningkat sebesar 5.
- **ACTIVITY** <nama_pet>
  Memicu aktivitas untuk hewan peliharaan berdasarkan jenisnya.
   - Anjing : Berjalan-jalan, meningkat kan loves sebesar 3 dan mengurangi energy sebesar 2.
   - Kucing : cuddle, meningkatkan loves sebesar 4.
- **FEED** <nama_pet>
  Memberi makan hewan peliharaan, energy meningkat sebesar 5.
- **ATTR** <nama_karakter> 
  Menampilkan atribbut terkini dari pegawai atau hewan peliharaan yang disebutkan.
- **EXIT** 
  Mengakhiri simulasi program.
  
## Karakter Awal
Program dilengkapi dengan empat karakter default untuk setiap jenis karakter:

- Pegawai: Alice, Bob, Charlie, Diane
- Pet:
   - Anjing: Buddy, Rocky
   - Kucing: Luna, Bella
     
## Contoh Penggunaan
**REST Alice**
Pegawai Alice beristirahat dan energy-nya meningkat.

**ACTIVITY Buddy**
Anjing Buddy berjalan-jalan, meningkatkan loves dan mengurangi energy.

**FEED Luna**
Memberi makan kucing Luna, meningkatkan energy-nya.

**ATTR Bob**
Menampilkan status atribut pegawai Bob.

**EXIT**
Mengakhiri program.
## Struktur Program 
**Struct Definitions** : Mendefinisikan struktur data Pegawai dan Pet.

**Function Implementations** : Berisi fungsi-fungsi aktivitas dan tampilan atribut.

**Main Loop** : Perulangan untuk menerima dan memproses perintah pengguna hingga simulasi dihentikan.

## Cara Komplikasi dan Menjalankan Program
Komplikasi program menggunakan perintah

gcc main.c -o petcafe

jalankan program dengan perintah

./petcafe

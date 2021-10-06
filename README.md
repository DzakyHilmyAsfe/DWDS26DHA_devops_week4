# Dokumentasi Perintah

### Git

* Pertama kita akan menginstall git terlebih dahulu menggunakan perintah `sudo apt install git -y` dan setelah itu kita cek versi nya menggunakan perintah `git --version`

![Screenshot from 2021-10-07 01-37-14](https://user-images.githubusercontent.com/90166624/136264458-e9aec9cf-9b18-4777-b8ad-e317a23ba3a1.png)

* Lalu kita akan mendaftar akun git baru menggunakan perintah `git config --global user.name "dzakyhilmyasfe"`
`git config --global user.email dzakyhilmyasfe@gmail.com`

* Setelah itu kita check menggunakan perintah `git --version`

![Screenshot from 2021-10-07 01-37-51](https://user-images.githubusercontent.com/90166624/136265776-7c05ce46-b51b-4df4-a159-ab6c1d2b26ac.png)

### Manipulasi Teks

**1. Cat**

Cat merupakan akronim dari concatenate, cat berfungsi untuk membuka isi file, membuat file baru,menggabungkan 2 file atau lebih, serta dapat mengonversi file menggunakan huruf besar atau kecil

* contoh perintah membuka isi file :

![Screenshot from 2021-10-01 01-24-00](https://user-images.githubusercontent.com/90166624/135512139-36bae2b7-9b3a-4049-a6f3-27db38e39523.png)

* contoh perintah membuat file baru :

![Screenshot from 2021-10-01 01-24-25](https://user-images.githubusercontent.com/90166624/135512226-c7e896e0-0d6f-4fd0-9e9e-e1ad5462994a.png)

* contoh perintah menggabung 2 file :

![Screenshot from 2021-10-01 01-25-49](https://user-images.githubusercontent.com/90166624/135512250-9e8eb3b6-0073-417f-9cce-c869464b17c2.png)

* contoh perintah mengonversi huruf pada file :

![Screenshot from 2021-10-01 01-34-06](https://user-images.githubusercontent.com/90166624/135512278-d1206aed-d0fc-4376-aa5e-580acc4ebf0e.png)


**2. Less**

* Gunakan perintah less ini untuk memberikan penomoran baris pada file.
```less -N filegabungan``` 

![Screenshot from 2021-10-01 01-28-23](https://user-images.githubusercontent.com/90166624/135512852-b0082882-d88f-4ea1-9c84-882b32765dfa.png)

**3. Sort**

Perintah sort digunakan untuk mengurutkan.

* `sort namafile` digunakan untuk mengurutkan secara A-Z dan 1-10.
* `sort -r namafile` digunakan untuk mengurutkan secara Z-A dan 10-1.

![Screenshot from 2021-10-01 01-52-07](https://user-images.githubusercontent.com/90166624/135514256-12db0824-68ab-46da-aadf-5ec9df115050.png)

**4. Head**

Perintah head digunakan untuk melihat baris pertama dari semua file teks. Secara default, perintah ini akan menampilkan sepuluh baris pertama. Namun, jumlah baris tersebut dapat diubah sesuai keinginan Anda. Misalnya, jika kita hanya ingin menampilkan lima baris pertama, ketik `head -n 5 filename.ext`

![Screenshot from 2021-10-01 02-09-37](https://user-images.githubusercontent.com/90166624/135516115-b90705b1-07cb-4a98-93d2-aeef6ab6c320.png)

**5. Tail**

Sedangkan perintah tail digunakan untuk melihat baris terakhir.

![Screenshot from 2021-10-01 02-12-23](https://user-images.githubusercontent.com/90166624/135516426-3332cc8f-c686-4c14-8d84-8befd514d675.png)

**6. Sed**

Sed adalah akronim dari stream editor, sed berfungsi untuk mensubtitusi atau mengganti teks pada suatu file.

* contoh perintahnya ialah `sed -i 's/baris/line/g' filehurufbesar`

![Screenshot from 2021-10-01 02-18-54](https://user-images.githubusercontent.com/90166624/135517288-1fa8bed4-100b-4d1d-8f3e-c320858bb429.png)

**7. Grep**

Grep berguna untuk mencari kalimat dalam sebuah file.

* contoh untuk mencari kata yaitu `grep INI filehurufbesar`

![Screenshot from 2021-10-02 01-10-05](https://user-images.githubusercontent.com/90166624/135667935-87d77ed5-7c30-40c4-9a23-99f9a3475cae.png)

* contoh untuk menghitung jumlah kata pada file `grep -c line filehurufbesar`

![Screenshot from 2021-10-02 01-16-03](https://user-images.githubusercontent.com/90166624/135668340-856e54d6-0b60-418f-bc68-de1bc0d98ecb.png)

**8. Diff**

Diff berasal dari kata different, berfungsi untuk membandingkan isi dua file, secara baris perbaris.

* contoh penggunaannya adalah `diff file.txt filehurufbesar`

![Screenshot from 2021-10-02 01-23-18](https://user-images.githubusercontent.com/90166624/135668892-2ef4dc8b-66e8-4a68-8d10-1c91b2cef08d.png)

**9. Echo**

Echo digunakan untuk mencetak kata, serta bisa juga digunakan untuk menginput kata.

* Contoh penggunaan kata untuk mecetak kata `echo "Hello world"` , untuk menginput kata pada file kita menggunakan `Hello world >> filehurufbesar`:

![Screenshot from 2021-10-02 01-30-54](https://user-images.githubusercontent.com/90166624/135669926-9ade335d-1cd8-4ca2-aa73-6b3e5d7e5449.png)

* Contoh penggunaan kata untuk menginput kata tersebut sebagai pengganti pada file `Hello world > filehurufbesar`:

![Screenshot from 2021-10-02 01-32-08](https://user-images.githubusercontent.com/90166624/135669965-672f3529-16ff-4e3f-9587-f8ff156e4015.png)

### Perintah Lain Yang Dapat Membantu 

Gunakan command clear untuk membersihkan terminal jika di dalamnya sudah terdapat banyak sekali command.

Coba tombol TAB untuk mengisi secara otomatis (autofill) apa yang sedang kita ketikkan. Sebagai contoh, jika ingin mengetik Documents, mulailah dengan menambahkan command terlebih dulu (misalnya cd Docu, kemudian tekan tombol TAB) dan terminal akan melengkapinya. Hasilnya akan seperti ini: cd Documents.

Ctrl+C dan Ctrl+Z digunakan untuk memberhentikan command apa pun yang saat ini sedang dijalankan. Ctrl+C akan memberhentikan command dengan aman, sedangkan CTRL+Z akan memaksa command untuk berhenti.

Bila kita secara tidak sengaja ‘membekukan’ terminal dengan menekan Ctrl+S, untuk membatalkan ‘pembekuan’ tersebut cukup tekan Ctrl+Z.

Ctrl+A membawa Anda ke awal baris, sedangkan Ctrl+E mengarahkan Anda ke akhir baris.

kita bisa menjalankan banyak command atau perintah di dalam satu command dengan menggunakan “;” untuk memisahkan command-command tersebut. Misalnya, Command1; Command2; Command3. Atau gunakan && jika Anda hanya ingin menjalankan command selanjutnya setelah command pertama berhasil dijalankan.

 `shift + PgUp` dan `shift + PgDn` berfungsi untuk menscroll keatas dan kebawah terminal.

### Monitoring

**1. Htop**

Htop digunakan untuk monitoring penggunaan RAM, sama hal nya seperti task manager pada windows.

![Screenshot from 2021-10-02 01-54-53](https://user-images.githubusercontent.com/90166624/135672408-68213ea5-2eb5-48c2-b746-6c8e17d49a4e.png)


**2. Lsof**

Lsof artinya list open file, perintah ini digunakan untuk melihat file yang sedang berjalan/dibuka.

* `lsof` berguna untuk melihat seluruh file yang sedang dibuka

![Screenshot from 2021-10-02 02-23-23](https://user-images.githubusercontent.com/90166624/135675582-4e5a1714-2979-4d36-bb5c-a60e0352acaa.png)

* `lsof -u dzakyha` berguna untuk melihat seluruh file yang dibuka pada user dzakyha

![Screenshot from 2021-10-02 02-25-09](https://user-images.githubusercontent.com/90166624/135675782-f970d8f0-f462-408e-98ad-15d1b283ffca.png)

**3. Ps**

Process Status (PS) digunakan untuk melihat proses yang sedang berjalan.

* `ps -f -u dzakyha` berguna untuk melihat seluruh proses yang berjalan pada user dzakyha

![Screenshot from 2021-10-02 02-30-08](https://user-images.githubusercontent.com/90166624/135676346-75bb51d1-9c37-4113-b1dc-ad79baed4239.png)

* `ps -aux` berguna untuk melihat seluruh proses yang berjalan secara lengkap

![Screenshot from 2021-10-02 02-30-56](https://user-images.githubusercontent.com/90166624/135676377-be5896ee-481e-41d5-bffd-64ed8f894957.png)

### Network Firewall

Firewall digunakan untuk mengamankan server.

* `sudo ufw default deny incoming` digunakan untuk menolak akses yang datang.

* `sudo ufw default allow outgoing` digunakan untuk membolehkan akses keluar.

![Screenshot from 2021-10-03 01-20-50](https://user-images.githubusercontent.com/90166624/135727744-8ae026a4-77b0-491f-8a70-fcf9b7d639e6.png)

* `sudo ufw app list` digunakan untuk melihat list aplikasi yang didukung ufw.

* `sudo ufw allow "Nginx Full"` digunakan untuk membolehkan akses pada aplikasi Nginx.

![Screenshot from 2021-10-03 02-31-34](https://user-images.githubusercontent.com/90166624/135729666-07057829-9321-4db2-9acc-2fba927cf29c.png)

* `sudo ufw allow 80` digunakan untuk membolehkan akses port 80.

* `sudo ufw allow 80/tcp` digunakan untuk membolehkan akses port 80 dengan tipe koneksi tcp.

* `sudo ufw allow 80/udp` digunakan untuk membolehkan akses port 80 dengan tipe koneksi udp.

* `sudo ufw deny 80` digunakan untuk menolak  akses port 80.

* `sudo ufw deny 80` digunakan untuk menghapus konfigurasi perintah yang telah dilakukan, pada contoh kita akan menghapus perintah pembolehan aksen port 80.

![Screenshot from 2021-10-03 02-41-52](https://user-images.githubusercontent.com/90166624/135729872-e0325fc8-caf8-4315-9f57-da0bd94fbbad.png)


### System Performance

**1. Vmstat**

* Untuk menjalankan vmstat kita tinggal mengetik `vmstat` pada terminal, maka akan muncul informasi performa sistem, dari penggunaan memori, kecepatan CPU,kecepatan I/O, dan sebagainya. 

* Gunakan perintah `vmstat -sSM` agar informasi sistem lebih mudah dibaca.

* Jika perintah vmstat tak bisa dijalankan, maka install system status terlebih dahulu menggunakan `sudo apt install sysstat -y`

![Screenshot from 2021-10-03 03-04-13](https://user-images.githubusercontent.com/90166624/135730414-f5696fa1-84d4-4c22-af3f-88d380c2a502.png)

![Screenshot from 2021-10-03 02-46-18](https://user-images.githubusercontent.com/90166624/135730116-e3c1bea5-d405-4c3e-8aeb-6db5895c4abe.png)

* Gunakan perintah `vmstat 2 10` agar informasi sistem dapat dibaca setiap 2 detik dengan 10 data yang terbaca, sehingga kita dapat memonitor secara real time.

![Screenshot from 2021-10-03 02-57-28](https://user-images.githubusercontent.com/90166624/135730293-91b0bed2-3d65-4be6-a7f1-e0c23e2d1f6f.png)

**2. Iostat**

Iostat digunakan untuk memonitor input dan output pada sistem, untuk menjalankannya kita akan menggunakan `iostat`.

![Screenshot from 2021-10-03 03-14-52](https://user-images.githubusercontent.com/90166624/135730674-c34ab3ba-8342-408f-8a43-5c38217083bd.png)

**3. Nmon**

Nmon dapat digunakan sebagai alternatif lain karena kita dapat memonitoring data secara lengkap dan real time.

* Untuk menginstall nmon : `sudo apt install nmon -y`

![Screenshot from 2021-10-03 03-16-29](https://user-images.githubusercontent.com/90166624/135730884-9d73f455-5617-411c-8dbc-66a377ba1dc8.png)

* Untuk menjalankan nmon : `nmon`

![Screenshot from 2021-10-03 03-16-54](https://user-images.githubusercontent.com/90166624/135730886-e762be6a-4b91-4dcc-9d7e-03d19f17399e.png)

* Untuk menjalankan perintah monitoring pada nmon, kita cukup menekan tombol keyboard tertentu contohnya key C untuk melihat penggunaan CPU, key D untuk melihat penggunaan disk, dan key N untuk melihat keadaan network.

![Screenshot from 2021-10-03 03-18-52](https://user-images.githubusercontent.com/90166624/135730892-71496c1e-89dc-40c7-9e73-78a5581d37a1.png)

### CMS Manajer

Cadabra Multi Server Manajer merupakan platform buatan yang ditemukan oleh Mas Sugeng Agung Suganda, yang sekaligus menjadi CEO. Pada CMS manajer kita dapat memanajemen server server dengan mudah secara one click hanya menggunakan satu dashboard. CMS Manajer juga mampu mengoptimasasi konfigurasi kernel, keamanadan dan performa pada server.

![Screenshot from 2021-10-04 01-21-02](https://user-images.githubusercontent.com/90166624/135766548-db4e5571-a7d4-4eca-a77c-d6f8d51597c0.png)

* Pertama kita perlu membuat akun kita pada https://cmsmanajer.com/register

![Screenshot from 2021-10-03 03-25-25](https://user-images.githubusercontent.com/90166624/135731034-80e5b3c5-6128-4ebf-8d48-538d97a1fd62.png)

* Untuk verifikasi email, coba kita lihat pada folder spam

* Setelah itu kita akan login

![Screenshot from 2021-10-03 03-27-49](https://user-images.githubusercontent.com/90166624/135731059-51f938f1-6c55-46a1-933e-a7e1c3618f78.png)

* Dilanjutkan dengan menghubungkan server kita ke cms manajer

![Screenshot from 2021-10-04 01-16-18](https://user-images.githubusercontent.com/90166624/135766676-e4f3e811-c29b-4ddb-abfd-0f37561a8cf9.png)

![Screenshot from 2021-10-04 01-18-27](https://user-images.githubusercontent.com/90166624/135766679-08805d2a-216e-4518-b7c8-ee13a57a782e.png)

* Server name dapat diisi dengan kemauan masing-masing,sedangkan ip address, username, serta SSH key dapat diperoleh setelah kita membuat virtual server menggunakan platform penyedia server seperti AWS.

* Setelah koneksi server berhasil dibuat, kita dapat membuat berbagai macam aplikasi seperti docker, mangoDB, wordpress, dan sebagainya.

![Screenshot from 2021-10-04 01-32-57](https://user-images.githubusercontent.com/90166624/135766954-f5191ea1-20fa-405d-a501-b0925dd99ada.png)

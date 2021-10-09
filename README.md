# Dokumentasi Perintah

## Git

### Instalasi dan Konfigurasi Git

* Pertama kita akan menginstall git terlebih dahulu menggunakan perintah `sudo apt install git -y` dan setelah itu kita cek versi nya menggunakan perintah `git --version`

![Screenshot from 2021-10-07 01-37-14](https://user-images.githubusercontent.com/90166624/136264458-e9aec9cf-9b18-4777-b8ad-e317a23ba3a1.png)

* Lalu kita akan mendaftar akun git baru menggunakan perintah `git config --global user.name "dzakyhilmyasfe"`
`git config --global user.email dzakyhilmyasfe@gmail.com`. Untuk melihat pendaftaran berhasil atau tidak, kita verifikasi menggunakan perintah `git config --list`

![Screenshot from 2021-10-07 01-37-51](https://user-images.githubusercontent.com/90166624/136265776-7c05ce46-b51b-4df4-a159-ab6c1d2b26ac.png)

* Selanjutnya kita akan membuat SSH keygen untuk menghubungkan git kita dengan github dengan menjalankan perintah `ssh-keygen`, masukkan nama file serta passphrase untuk membuat ssh keygen :

![Screenshot from 2021-10-07 02-12-40](https://user-images.githubusercontent.com/90166624/136268271-81b40c26-912e-4a68-8f02-99a90fdadc7b.png)

* Lalu kita buka file dari ssh keygen menggunakan `cat keygen.pub`, dan isi file tersebut kita copy.

![Screenshot from 2021-10-07 02-22-52](https://user-images.githubusercontent.com/90166624/136269629-989eeb25-3733-4843-b9df-f2120d2a0884.png)

* paste key baru tersebut pada alamat web https://github.com/settings/keys 

![Screenshot from 2021-10-07 02-23-00](https://user-images.githubusercontent.com/90166624/136269650-932cae83-8b5a-403f-a971-686767c8a4a3.png)

*   Setelah dimasukkan maka tampilannya akan menjadi seperti ini.

![Screenshot from 2021-10-07 02-23-18](https://user-images.githubusercontent.com/90166624/136269665-f4b014fa-84e1-46aa-8af2-db2b35251560.png)

### Repository 

Repository ini berfungsi sebagai direktori atau folder yang akan menyimpan perubahan pada git. Untuk membuat repository kita bisa menggunakan perintah `git init` atau `git init belajargit` agar git terbuat didalam direktori belajargit.

![Screenshot from 2021-10-07 14-59-53](https://user-images.githubusercontent.com/90166624/136343987-abd7893e-b05b-4dcf-9d44-59bcdca87d6e.png)

### .gitignore

`.gitignore` merupakan file yang akan membuat file atau directory yang bila daftar namanya dimasukkan kedalam file .gitignore, maka file atau directory tersebut akan diabaikan oleh git ketika melakukan push/upload ke database git. Pada contoh yang penulis buat,penulis membuat 4 file baru, terdiri dari, .gitignore, file1, file2.html, dan file3. Penulis memasukkan 2 file ke .gitignore, yaitu file1 dan file2.html. Ketika di cek menggunakan perintah `git status` maka file1 dan file2.html tidak akan ada pada list, karena sudah di ignore.

![Screenshot from 2021-10-07 15-07-40](https://user-images.githubusercontent.com/90166624/136346264-888cbbde-7bf1-4a43-b8fb-2895518ca6c3.png)

![Screenshot from 2021-10-07 15-10-32](https://user-images.githubusercontent.com/90166624/136346274-b691e2f8-17c2-4a8d-b0cc-a071a10bc7b4.png)

### Git Add dan Commit

Terdapat 3 kondisi file dalam git, yang pertama adalah kondisi modified, artinya file suda di modifikasi tapi perubahan belum ditandai, lalu yang kedua adalah kondisi staged dimana file yang sudah di modifikasi akan ditandai perubahannya, perintah yang digunakan adalah `git add`, dan yang ketiga adalah kondisi commited yaitu kondisi ketika file yang sudah ditandai perubahannya disimpan dalam database git,perintah yang digunakan adalah `git commit`.

Ada 3 cara untuk menggunakan perintah git add :

* `git add namafile.ext` untuk menambahkan satu file yakni namafile.ext.
* `git add *.ext` untuk menambahkan semua file dengan akhiran extension ".ext".
* `git add .` untuk menambahkan semua file dari repository.

![Screenshot from 2021-10-07 16-25-57](https://user-images.githubusercontent.com/90166624/136357758-1a3177f0-d22c-4f23-a4f5-d383f68b6536.png)


Untuk menjalankan perintah commit, kita menggunakan perintah `git commit -m "my first commit"`

![Screenshot from 2021-10-07 16-27-34](https://user-images.githubusercontent.com/90166624/136358001-bf28fc6f-b211-4c1a-8b6f-80162ceb4c3d.png)

### Git Remote

Untuk menggunakan git remote kita akan menggunakan github, pertama tama kita harus membuat akun github, lalu kita membuat repository baru.

![Screenshot from 2021-10-07 16-36-20](https://user-images.githubusercontent.com/90166624/136359621-02aa241b-daad-45df-90c2-a6cf0c86a2b7.png)

* Selanjutnya kita akan menjalankan perintah berikut untuk mem push atau mengupload repository yang telah kita buat.

`git remote add origin https://github.com/DzakyHilmyAsfe/belajargit.git`
`git branch -M main`
`git push -u origin main`

![Screenshot from 2021-10-07 16-59-02](https://user-images.githubusercontent.com/90166624/136365238-40015955-303e-48db-94ba-89441b7deaf7.png)

* Karena untuk login nya kita memerlukan Personal Access Token, maka terlebih dahulu kita bikin PAT pada halaman web https://github.com/settings/tokens

![Screenshot from 2021-10-07 17-00-10](https://user-images.githubusercontent.com/90166624/136365669-7f7f4bf6-943e-4298-987d-1ef4a0912d5c.png)

![Screenshot from 2021-10-07 17-01-40](https://user-images.githubusercontent.com/90166624/136365690-441cf9e8-481d-4b34-bd71-db2cb47126ca.png)

* Masukkan PAT sebagai password untuk mempush repository yang telah kita buat, maka hasilnya adalah :

![Screenshot from 2021-10-07 17-01-51](https://user-images.githubusercontent.com/90166624/136365778-a7e908d9-d97f-43e9-91dd-8571b9c7aebe.png)

![Screenshot from 2021-10-07 17-02-14](https://user-images.githubusercontent.com/90166624/136366106-ffa41ad3-c4cc-4489-b524-a0bbec5536be.png)


### Git Branch

Git Branch adalah perintah yang digunakan untuk membuat cabang baru, dengan adanya cabang ini, setiap anggota tim bisa melakukan pekerjaannya masing masing, tanpa mengganggu penulisan kode dari anggota lain, contohnya pada gambar pada branch pertama si A akan membuat fitur register dan si B akan membuat fitur upload.

![image](https://user-images.githubusercontent.com/90166624/136368663-59ff71a3-d6db-4545-80b4-f2917a670bc1.png)

Berikut merupakan perintah untuk git branch :

* `git branch development` untuk membuat branch baru dengan nama development
* `git branch -M main` untuk membuat branch baru dengan nama main
* `git branch -a` untuk melihat list branch yang telah dibuat
* `git branch -M main staging` untuk mengubah nama branch main menjadi staging 

![Screenshot from 2021-10-07 17-53-37](https://user-images.githubusercontent.com/90166624/136370985-f3a33198-d688-4f5f-9cb4-4982eb0e7477.png)

### Git Checkout

Git checkout digunakan untuk berpindah branch.gunakan `git branch` untuk mengetahui kita berada di branch mana, setelah itu gunakan `git checkout` untuk merubah

![Screenshot from 2021-10-07 17-58-40](https://user-images.githubusercontent.com/90166624/136371523-2969637a-5d9d-4a9b-abf0-871ef27cef0c.png)


### Git Push

Git push berguna untuk meng upload data dari database lokal git kita ke data server github. Untuk melakukan git kita perlu men add dan men commit file terlebih dahulu.

tahapnya adalah :

* `git remote -v` digunakan untuk melihat remote dan repository yang telah di buat
* `git add .`
* `git commit -m "update data"`
* `git push origin staging` digunakan untuk melakukan push data pada branch staging

![Screenshot from 2021-10-07 20-41-06](https://user-images.githubusercontent.com/90166624/136396163-505f0876-b21f-455c-ae7a-7b0263b8edb4.png)

![Screenshot from 2021-10-07 20-40-58](https://user-images.githubusercontent.com/90166624/136396195-dc8836ff-0f8c-42a1-812e-c633ea4cfd14.png)

### Git Pull

Git pull digunakan untuk menarik kode dari database server git ke database lokal kita, berfungsi untuk menyamakan perubahan seperti update kode yang telah dilakukan oleh user lain.

Perintahnya adalah

* `git pull` digunakan untuk menarik semua data dari semua branch
* `git pull origin staging` digunakan untuk  menarik semua data dari branch staging

![Screenshot from 2021-10-07 20-47-59](https://user-images.githubusercontent.com/90166624/136397324-624fb964-469e-4493-951e-659cd57ce7db.png)

### Git Merge

Git merge digunakan untuk menggabungkan branch. Penulis merubah nama branch utama yaitu `main` menjadi `production` pada alamat browser https://github.com/DzakyHilmyAsfe/belajargit/settings/branches . Lalu mengubah branch utama pada lokal database dengan perintah :

`git branch -m main production`

`git fetch origin`

`git branch -u origin/production production`

`git remote set-head origin -a`

![Screenshot from 2021-10-07 21-31-34](https://user-images.githubusercontent.com/90166624/136405828-aeead630-5188-4ff8-9a17-c28c6e0eb031.png)

* Setelah itu penulis menambahkan branch baru bernama development dengan sebuah filedevelopment didalamnya

![Screenshot from 2021-10-07 21-38-42](https://user-images.githubusercontent.com/90166624/136407286-b83f4030-539d-443e-b60f-bf0e4f86dc25.png)

* Saat ini penulis memiliki 3 branch yaitu, production, staging, dan development yang memiliki file-file yang berbeda disetiap branch nya.

![Screenshot from 2021-10-07 21-41-48](https://user-images.githubusercontent.com/90166624/136411311-e661068f-95b6-4ef5-a10d-9c12e1f0b237.png)

* Branch production terdiri dari file :

![Screenshot from 2021-10-07 21-42-14](https://user-images.githubusercontent.com/90166624/136411342-6abbecf6-b1ca-45ee-9121-5c2bb1513a5b.png)

* Branch staging terdiri dari file :

![Screenshot from 2021-10-07 21-43-11](https://user-images.githubusercontent.com/90166624/136411413-a31cb8c8-baa2-407b-9c0e-2193f54bb9c5.png)

* Branch development terdiri dari file :

![Screenshot from 2021-10-07 21-42-44](https://user-images.githubusercontent.com/90166624/136411441-fc537486-005f-447e-9662-47fedea01fa8.png)

* Untuk melakukan merging atau penggabungan branch development ke staging, kita terlebih dahulu pindah ke branch staging menggunakan perintah `git checkout staging` lalu jalankan perintah `git merge development`

![Screenshot from 2021-10-07 22-29-16](https://user-images.githubusercontent.com/90166624/136416859-a81b1e3e-67b0-4e85-8028-8ba047eeb7a9.png)

![Screenshot from 2021-10-07 22-32-07](https://user-images.githubusercontent.com/90166624/136416879-e28ea948-0ab2-4268-b76b-f2345cf0c1e7.png)

* Setelah itu kita push branch staging, dan kita check pada github. Dari screenshot diatas dapat kita lihat file dari branch development akan bergabung ke branch staging

![Screenshot from 2021-10-07 22-35-19](https://user-images.githubusercontent.com/90166624/136417213-bef77733-aad5-43d3-b4a5-f94843d2c0c6.png)

![Screenshot from 2021-10-07 22-35-53](https://user-images.githubusercontent.com/90166624/136417245-b513fe6f-dd30-4164-8085-14bd690de837.png)

* Untuk melakukan merging branch staging ke production, kita akan melakukan hal yang sama seperti sebelumnya. Pindah ke branch production menggunakan perintah `git checkout production` lalu jalankan perintah `git merge staging`. Setelah itu kita push branch staging, dan kita check pada github. 

![Screenshot from 2021-10-07 23-11-16](https://user-images.githubusercontent.com/90166624/136423267-9dba6369-fffc-4e9b-844d-c3ae6963001f.png)

![Screenshot from 2021-10-07 23-11-34](https://user-images.githubusercontent.com/90166624/136423290-4eb744d4-6b14-4311-b390-77c285d77001.png)



## Reverse Proxy

Reverse proxy digunakan untuk mengamankan server dari serangan malware, dengan menggunakan reverse proxy, user tidak bisa langsung mengakses aplikasi secara langsung, sehingga harus melewati web server (nginx) sebagai jembatan.

![image](https://user-images.githubusercontent.com/90166624/136671978-4298f488-91c9-4a18-b94e-0c6433d2d16f.png)

Untuk menggunakan reverse proxxy pada nginx, berikut langkah yang akan kita lakukan :

* Install nginx menggunakan perintah `sudo apt install nginx` lalu jalankan dengan perintah `sudo systemctl enable nginx` agar nginx selalu berjalan di startup.
* Pindah ke direktori nginx `cd /etc/nginx`
* Buat direktori baru bernama nodejs dengan perintah `sudo mkdir nodejs`
* Lalu tambahkan direktori yang telah kita buat agar konfigurasi yang kita buat bisa terbaca nginx pada file `sudo nano etc/nginx/nginx.conf`

![Screenshot from 2021-10-09 14-12-57](https://user-images.githubusercontent.com/90166624/136672215-002273e7-93a3-48fd-924e-c1541274ebad.png)

![Screenshot from 2021-10-09 14-11-08](https://user-images.githubusercontent.com/90166624/136672220-bdbdf1d0-f491-4eb0-904c-dd8c3c36d105.png)

* Pindah ke direktori yang baru kita buat `cd /nodejs`
* Lalu buat file baru `sudo nano nodejs-reverse-proxy.conf`
* Masukkan kode berikut :

```
server {
        listen 80
        server_name domainaplikasi.xyz ;
        location /aplikasi1 {
                proxy_pass http://127.0.0.1:3000 ;
}
```

* Untuk local server kita perlu mengubah domain pada nginx pada file `sudo nano /etc/hosts`
* Lakukan tes konfigurasi nginx menggunakan `sudo nginx -t`
* Jika tidak terdapat error maka kita bisa menerapkan konfigurasi menggunakan perintah `sudo systemctl restart nginx` atau `sudo systemctl reload nginx`

* Ketika kita membuka alamat bla bla akan memunculkan bla bla
* Jika kita membuka alamat nbla alb akan membuka aksjdksad

# LATIHAN

## Login Akun Docker

![](img/01.png)

Lakukan proses login terlebih dahulu menggunakan akun Docker kita untuk dapat mengakses terminal linux pada web ini.

## Task 0: Prerequisites
Meng-clone repo dari github dengan nama linux_tweet_app pada akun dockersamples.

![](img/02.png)

## Task 1: Run some simple Docker containers
## Run a single task in an Alpine Linux container
1. Memulai container baru dengan image alpine

![](img/03.png)

2. Melihat daftar semua container yang ada

![](img/04.png)

## Run an interactive Ubuntu container
1. Menjalankan Docker container dan mengakses terminal ubuntu

![](img/05.png)

2. Menjalankan perintah berikut.

![](img/06.png)

Jalankan perintah $ ls / untuk menampilkan daftar folder atau file yang ada.

Jalankan perintah $ ps aux untuk menampilkan proses container yang sedang berjalan.

Jalankan perintah $ cat /etc/issue untuk menampilkan distro linux yang container yang digunakan.

3. Keluar dari terminal ubuntu

![](img/07.png)

4. Cek versi host VM

![](img/08.png)

## Run a background MySQL container
1. Menjalankan MySQL container

![](img/09.png)

2. Melihat daftar container

![](img/10.png)

3. Cek log dan proses yang berjalan didalam container

![](img/11.png)

![](img/12.png)

4. Melihat versi MySQL yang digunakan

![](img/13.png)

5. Menghubungkan terminal ke sh

![](img/14.png)

## Task 2: Package and run a custom app using Docker
## Build a simple website image
1. Berpindah ke direktori repo yang telah di-clone sebelumnya

![](img/15.png)

Jalankan perintah $ cat Dockerfile untuk melihat isi dari Dockerfile.

2. Mengexport variabel dockerid dengan isian id docker kita

![](img/16.png)

Jalankan perintah $ echo $DOCKERID untuk menampilkan isi dari variabel dockerid.

3. Membuat docker image

![](img/17.png)

4. Menjalankan container untuk menghosting image yang telah dibuat

![](img/18.png)

5. Mengecek hasilnya dengan menekan link yang telah disediakan

![](img/19.png)

6. Menghentikan dan menghapus container lalu mengeceknya

![](img/20.png)

## Task 3: Modify a Running Website
## Start our web app with a bind mount
1.Menjalankan container untuk meng-hosting image yang telah dibuat

![](img/21.png)

2. Mengecek bahwasanya image berhasil di hosting dengan menekan link yang telah disediakan

![](img/22.png)

## Modify the running website
1. Meng-copy index.html container dan merefresh web untuk melihat hasilnya

![](img/23.png)

![](img/24.png)

2. Menghentikan dan menghapus container dan mengeceknya

![](img/25.png)

![](img/26.png)

## Update the image
1. Membuat image baru

![](img/27.png)

2. Melihat daftar image yang ada

![](img/28.png)

## Test the new version
1. Menjalankan container dan melihat hasilnya

![](img/29.png)

![](img/30.png)

2. Menjalankan container lainnya dan melihat hasilnya

![](img/31.png)

![](img/32.png)

## Push your images to Docker Hub
1. Melihat daftar image yang telah di hosting

![](img/33.png)

2. Sebelumnya login menggunakan akun docker kita agar tepat dan lancar di push atau upload pada akun docker kita

![](img/34.png)

3. Push image versi 1.0 dan 2.0

![](img/35.png)

4. Melihat hasil image yang telah di push pada akun docker hub kita masing-masing, dengan cara: https://hub.docker.com/r/<your docker id>/

![](img/36.png)
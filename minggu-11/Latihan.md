# LATIHAN

## Login Akun Docker

![](img/01.png)

Login terlebih dahulu menggunakan akun Docker kita untuk dapat mengakses terminal linux pada web ini.


## Stage Setup

![](img/02.png)

$ git clone https://github.com/ibnesayeed/linkextractor.git
Merupakan perintah untuk meng-clone repository dari url github.

$ cd linkextractor
Perintah untuk berpindah ke direktori linkextractor.

$ git checkout demo
Perintah untuk berpindah ke branch demo.


## Step 0 : Basic Link Extractor Script

![](img/03.png)

$ git checkout step0
Merupakan perintah untuk berpindah ke branch step0.

$ tree
Perintah untuk menampilkan struktur folder.

![](img/04.png)

$ cat linkextractor.py
Merupakan perintah untuk menampilkan isi file linkextractor.py.

$ ./linkextractor.py http://example.com/
Perintah untuk menjalankan file linkextractor.py.

![](img/05.png)

$ ls -l linkextractor.py
Merupakan perintah untuk melihat hak/izin akses file linkextractor.py.

$ python linkextractor.py
Perintah untuk menjalankan file linkextractor.py.


## Step 1 : Containerized Link Extractor Script

![](img/06.png)

$ git checkout step1
Merupakan perintah untuk berpindah ke branch step1.

$ tree
Perintah untuk menampilkan struktur folder.

![](img/07.png)

![](img/08.png)

![](img/09.png)

$ cat Dockerfile
Merupakan perintah untuk menampilkan isi file Dockerfile.

$ docker image build -t linkextractor:step1 .
Perintah untuk membuat image.

$ docker image ls
Perintah untuk menampilkan daftar image.

$ docker container run -it --rm linkextractor:step1 http://example.com/
Perintah untuk menjalankan container.

![](img/10.png)

$ docker container run -it --rm linkextractor:step1 https://training.play-with-docker.com/
Merupakan perintah untuk menjalankan container.


## Step 2 : Link Extractor Module with Full URI and Anchor Text

![](img/11.png)

$ git checkout step2
Merupakan perintah untuk berpindah ke branch step2.

$ tree
Perintah untuk menampilkan struktur folder.

![](img/12.png)

$ cat linkextractor.py
Merupakan perintah untuk menampilkan isi file linkextractor.py.

![](img/13.png)

$ docker image build -t linkextractor:step2 .
Merupakan perintah untuk membuat image.

![](img/14.png)

$ docker image ls
Perintah untuk menampilkan daftar image.

![](img/15.png)

$ docker container run -it --rm linkextractor:step2 https://training.play-with-docker.com/
Merupakan perintah untuk menjalankan container.

![](img/16.png)

$ docker container run -it --rm linkextractor:step1 https://training.play-with-docker.com
Perintah untuk menjalankan container.


## Step 3 : Link Extractor API Service

![](img/17.png)

$ git checkout step3
Merupakan perintah untuk berpindah ke branch step3.

$ tree
Perintah untuk menampilkan struktur folder.

![](img/18.png)

$ cat Dockerfile
Merupakan perintah untuk menampilkan isi file Dockerfile.

![](img/19.png)

$ cat main.py
Merupakan perintah untuk menampilkan isi file main.py.

![](img/20.png)

$ docker image build -t linkextractor:step3 .
Merupakan perintah untuk membuat image.

![](img/21.png)

$ docker container run -d -p 5000:5000 --name=linkextractor linkextractor:step3
Merupakan perintah untuk menjalankan container.

$ docker container ls
Perintah untuk menampilkan daftar container.

![](img/22.png)

$ curl -i http://localhost:5000/api/http://example.com/
Merupakan perintah untuk membuat permintaan HTTP.

![](img/23.png)

$ docker container logs linkextractor
Merupakan perintah untuk melihat catatan container.

$ docker container rm -f linkextractor
Perintah untuk menghapus container.


## Step 4 : Link Extractor API and Web Front End Services

![](img/24.png)

$ git checkout step4
Merupakan perintah untuk berpindah ke branch step4.

$ tree
Perintah untuk menampilkan struktur folder.

![](img/25.png)

$ cat docker-compose.yml
Merupakan perintah untuk menampilkan isi file docker-compose.yml.

![](img/26.png)

$ cat www/index.php
Merupakan perintah untuk menampilkan isi file www/index.php

![](img/27.png)

$ docker-compose up -d –build
Merupakan perintah untuk menjalankan layanan docker compose.

![](img/28.png)

$ docker container ls
Merupakan perintah untuk menampilkan daftar container.

![](img/29.png)

$ curl -i http://localhost:5000/api/http://example.com/
Perintah untuk menghubungakan dengan layanan API.


Mengakses web link extractor

![](img/30.png)

![](img/31.png)

$ sed -i 's/Link Extractor/Super Link Extractor/g' www/index.php
Perintah untuk memodifikasi index file link extractor.

![](img/32.png)

![](img/33.png)

$ git reset --hard
Merupakan perintah untuk me-reset atau mengembalikan perubahan.

$ docker-compose down
Perintah untuk menghentikan layanan.


## Step 5 : Redis Service for Caching

![](img/34.png)

$ git checkout step5
Merupakan perintah untuk berpindah ke branch step5.

$ tree
Perintah untuk menampilkan struktur folder.

![](img/35.png)

$ cat www/Dockerfile
Perintah untuk menampilkan isi file www/Dockerfile.

![](img/36.png)

$ cat api/main.py
Merupakan perintah untuk menampilkan isi file api/main.py.

![](img/37.png)

$ cat docker-compose.yml
Perintah untuk menampilkan isi file docker-compose.yml.

![](img/38.png)

$ docker-compose up -d –build
Perintah untuk menjalankan layanan.


Mengakses web Link Extractor

![](img/39.png)

![](img/40.png)

![](img/41.png)

$ docker-compose exec redis redis-cli monitor
Merupakan perintah untuk membuaka client redis.

$ sed -i 's/Link Extractor/Super Link Extractor/g' www/index.php
Perintah untuk memodifikasi index file link extractor.

$ git reset --hard
Merupakan perintah untuk mereset atau mengembalikan perubahan.

$ docker-compose down
Perintah untuk menghentikan layanan.


## Step 6 : Swap Python API Service with Ruby

![](img/42.png)

$ git checkout step6
Merupakan perintah untuk berpindah ke branch step6.

$ tree
Perintah untuk menampilkan struktur folder.

![](img/43.png)

$ cat api/linkextractor.rb
Perintah untuk menampilkan isi file api/linkextractor.rb.

![](img/44.png)

$ cat api/Dockerfile
Merupakan perintah untuk menampilkan isi file api/Dockerfile.

![](img/45.png)

$ cat docker-compose.yml
Perintah untuk menampilkan isi file docker-compose.yml.

![](img/46.png)

$ docker-compose up -d –build
Merupakan perintah untuk menjalankan layanan.

![](img/47.png)

$ curl -i http://localhost:4567/api/http://example.com/
Merupakan perintah untuk menghubungkan layanan.


Mengakses web link extractor

![](img/48.png)


Menguji sebuah url untuk di extract

![](img/49.png)

![](img/50.png)

![](img/51.png)

$ docker-compose down
Merupakan perintah untuk menghentikan layanan.

$ cat logs/extraction.log
Perintah untuk melihat catatan sebuah web yang telah di extract.
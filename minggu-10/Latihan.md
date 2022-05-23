# LATIHAN

## Login Akun Docker

![](img/01.png)

Login terlebih dahulu menggunakan akun Docker kita untuk dapat mengakses terminal linux pada web ini.


## Section #1 - Networking Basics

Step 1: The Docker Network Command

![](img/02.png)

$ docker network
Merupakan perintah utama untuk konfigurasi dan mengelola container networks.

Step 2: List networks

![](img/03.png)

$ docker network ls
Merupakan perintah untuk menampilkan daftar container networks.

Step 3: Inspect a network

![](img/04.png)

$ docker network inspect bridge
Merupakan perintah untuk melihat detail konfigurasi jaringan.

Step 4: List network driver plugins

![](img/05.png)

$ docker info
Merupakan perintah untuk melihat informasi mengenai installasi Docker.


## Section #2 - Bridge Networking

Step 1: The Basics

![](img/06.png)

$ docker network ls
Merupakan perintah untuk menampilkan daftar container networks.

![](img/07.png)

$ apk update
Merupakan perintah untuk meng-update dan install packages bridge-utils.

![](img/08.png)

$ apk add bridge
Merupakan perintah untuk menambahkan packages bridge-utils.

![](img/09.png)

$ brctl show
Merupakan perintah untuk menampilkan daftar bridges pada Docker host.

![](img/10.png)

$ ip a
Merupakan perintah untuk melihat detail bridge.

Step 2: Connect a container

![](img/11.png)

$ docker run -dt ubuntu sleep infinity
Merupakan perintah untuk membuat container baru.

![](img/12.png)

$ docker ps
Merupakan perintah untuk melihat spek container network.

![](img/13.png)

$ brctl show
Merupakan perintah untuk menampilkan daftar bridges pada Docker host.

![](img/14.png)

$ docker network inspect bridge
Merupakan perintah untuk menampilkan lampiran pada container bridge.

Step 3: Test network connectivity

![](img/15.png)

$ ping -c5 172.17.0.2
Tes jaringan (ping).

![](img/16.png)

$ docker ps
Merupakan perintah untuk melihat spek container network.

![](img/17.png)

$ docker exec -it yourcontainerid /bin/bash
Merupakan perintah untuk masuk terminal ubuntu.

$ apt-get update && apt-get install -y iputils-ping
Menginstall program ping.

![](img/18.png)

$ ping -c5 www.github.com
Tes jaringan (ping).

$ exit
Merupakan perintah untuk keluar dari terminal ubuntu.

![](img/19.png)

$ docker stop (id container)
Menghentikan container yang sedang berjalan.

Step 4: Configure NAT for external connectivity

![](img/20.png)

$ docker run --name web1 -d -p 8080:80 nginx
Menjalankan container baru dari official NGINX image.

![](img/21.png)

$ docker ps
Merupakan perintah untuk melihat spek container network.

![](img/22.png)

$ curl 127.0.0.1:8080
Merupakan perintah untuk menghubungkan ke docker host.


## Section #3 - Overlay Networking

Step 1: The Basics

![](img/23.png)

$ docker swarm init --advertise-addr $(hostname -i)
Merupakan perintah untuk menginisialisasi docker swarm baru.

![](img/24.png)

$ docker swarm join \
> --token SWMTKN-1-69b2x1u2wtjdmot0oqxjw1r2d27f0lbmhfxhvj83chln1l6es5-37ykdpul0vylenefe2439cqpf \
> 192.168.0.47:2377
Menggabungkan node.

![](img/25.png)

$ docker node ls
Merupakan perintah untuk melihat daftar node.

Step 2: Create an overlay network

![](img/26.png)

$ docker network create -d overlay overnet
Membuat sebuah overlay network.

![](img/27.png)
![](img/28.png)

$ docker network ls
Mengecek/menampilkan network.

![](img/29.png)

$ docker network inspect overnet
Merupakan perintah untuk melihat lebih detail informasi mengenai overnet network.

Step 3: Create a service

![](img/30.png)

$ docker service create --name myservice \
--network overnet \
--replicas 2 \
Membuat layanan baru.

![](img/31.png)

$ docker service ls
Merupakan perintah untuk cek/menampilkan daftar layanan.

![](img/32.png)

$ docker service ps myservice
Merupakan perintah untuk melihat daftar layanan yang sedang berjalan.

![](img/33.png)

$ docker network ls
Mengecek/menampilkan network.

Step 4: Test the network

![](img/34.png)

$ docker network inspect overnet
Merupakan perintah untuk melihat lebih detail informasi mengenai overnet network.

![](img/35.png)

$ docker ps
Melihat spek container network.


## Cleaning Up

![](img/36.png)

$ docker service rm myservice
Merupakan perintah untuk menghapus layanan.

![](img/37.png)

$ docker ps
Merupakan perintah untuk melihat spek container network.

![](img/38.png)

$ docker swarm leave --force
Merupakan perintah untuk menghapus node.
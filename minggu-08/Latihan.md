# LATIHAN

1. Proses instalasi docker dekstop

![](img/latihan/01.png)

Tunggu sampai proses instalasi selesai. Apabila sudah selesai maka selanjutnya klik	finish.

![](img/latihan/02.png)


2. Selanjutnya masuk pada command prompt lalu jalankan perintah berikut :

![](img/latihan/03.png)


3. Build and run image

![](img/latihan/04.png)

//mengcloning repo berdasarkan url
$ git clone https://github.com/dockersamples/node-bulletin-board

![](img/latihan/05.png)

//berpindah direktori
$ cd node-bulletin-board/bulletin-board-app

![](img/latihan/06.png)

![](img/latihan/07.png)

![](img/latihan/08.png)

//build image docker
$ docker image build -t bulletinboard:1.0

![](img/latihan/09.png)

![](img/latihan/10.png)

menjalankan container untuk melihat docker image nantinya secara local yakni pada localhost:8000

4. Share image on Docker Hub

![](img/latihan/11.png)

Buat akun docker hub terlebih dahulu, jika sudah kita membuat repo baru dengan nama bulletinboard.

![](img/latihan/12.png)

//share image kita ke docker hub
$docker image tag bulletinboard:1.0 soholeh/bulletinboard:1.0

![](img/latihan/13.png)

//push image kita ke docker hub
$docker image push soholeh/bulletinboard:1.0


Untuk melihat hasilnya kita dapat membuka tab baru dan isikan url dengan localhost:8000

![](img/latihan/14.png)
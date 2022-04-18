# LATIHAN

1. Membuat direktori proyek

![](img/01.png)

Jalankan perintah $ mkdir composetest pada git bash seperti gambar diatas untuk membuat folder baru dengan nama composetest.
Jalankan perintah $ cd composetest/ pada git bash seperti gambar diatas untuk berpindah ke folder composetest.
Jalankan perintah $ code pada git bash seperti gambar diatas untuk membuka code editor vscode.

2. Membuat file app.py

![](img/02.png)

3. Membuat file requirements.txt

![](img/03.png)

4. Membuat Dockerfile.

![](img/04.png)

5. Define services pada Compose file.

![](img/05.png)

6. Menjalankan perintah docker-compose up.

![](img/06.png)

![](img/07.png)

![](img/08.png)

Jalankan aplikasi dengan cara:
Masukkan perintah $ docker-compose up.

7. Membuka url http://localhost:5000/ untuk melihat hasilnya.

![](img/09.png)

8. Refresh halaman.

![](img/10.png)

9. Membuka terminal lain dan menjalankan perintah $ docker image ls.

![](img/11.png)

10. Edit Compose file untuk menambahkan bind mount.

![](img/12.png)

11. Re-build and run the app with Compose dengan menjalankan perintah docker-compose up.

![](img/13.png)

12. Cek pada browser.

![](img/14.png)

13. Update the application dan merubah file app.py

![](img/15.png)

14. Mengecek hasilnya pada browser.

![](img/16.png)

15. Experiment with some other commands dan menjalankan perintah docker lainnya.

![](img/17.png)

Jalankan perintah $ docker-compose up -d seperti gambar diatas untuk menjalankan aplikasi pada latar belakang.
Jalankan perintah $ docker-compose ps sperti gambar diatas untuk melihat aplikasi yang sedang berjalan.

16. Menjalankan perintah docker lainnya.

![](img/18.png)

Jalankan perintah $ docker-compose run web env seperti gambar diatas untuk menjalankan dan melihat variabel yang tersedia.
Jalankan perintah $ docker-compose stop seperti gambar diatas untuk menghentikan aplikasi.
Jalankan perintah $ docker-compose down –volumes seperti gambar diatas untuk menghapus containers.
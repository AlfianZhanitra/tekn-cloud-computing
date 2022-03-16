# Latihan

## Install dan Menjalankan Apache OFBiz

Apache OFBiz adalah sistem perencanaan sumber daya perusahaan sumber terbuka. Apache OFBiz menyediakan seperangkat aplikasi perusahaan yang mengintegrasikan dan mengotomatisasi banyak proses bisnis suatu perusahaan. OFBiz adalah proyek tingkat atas Apache Software Foundation.

1. Download dan extract file Apache OFBiz.

![](img/01.png)

![](img/02.png)


2. Pastikan java sudah terinstall.
   Cek instalasi java menggunakan command prompt.

![](img/03.png)


3. Buka command prompt, kemudian masuk ke direktori instalasi ofbiz.
   Masukkan perintah “init-gradle-wrapper” untuk mendownload gradle wrapper.

![](img/04.png)


Kemudian masukkan perintah “gradlew cleanAll loadAll” dan tunggu hingga proses load selesai.

![](img/05.png)


4. Masukkan perintah “gradlew ofbiz” untuk menjalankan ofbiz.

![](img/06.png)


5. Uji coba server local ofbiz dengan cara mengakases server local ofbiz melalui alamat https://localhost:8443/demo.

![](img/07.png)


Lakukan proses login, kemudian akan muncul tampilan berikut

![](img/08.png)
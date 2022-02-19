TUGAS
1. Fork Fork adalah membuat clone dari suatu repo di GitHub milik upstream author, diletakkan ke milik kontributor. Fork hanya dilakukan sekali saja. Pada dasarnya, proses untuk fork ini meliputi:
a. Fork repo di web GitHub.
b. Clone fork tersebut di komputer lokal. Kontributor harus mem-fork repo upstream author sehingga di repo kontributor muncul repo tersebut.
Proses forking ini dijelaskan dengan langkah-langkah berikut:
- Login ke GitHub
- Akses repo yang akan di fork:https://github.com/dwiendahsulistyowati/playground

Pada sisi kanan atas, klik Fork

![](image/tugas/001.png)

![](image/tugas/002.png)

Setelah proses tersebut, clone ke komputer lokal

![](image/tugas/003.png)

Setelah itu, konfigurasikan repo lokal kontributor. Pada kondisi saat ini, di komputer lokal sudah terdapat repo playground yang berada pada direktori dengan nama yang sama.
Untuk keperluan berkontribusi, ada 2 nama repo yang harus diatur:

a. origin: menunjuk ke repo milik kontributor di GitHub, hasil dari fork.

b. upstream: menunjuk ke repo milik upstream author (repo asli) di account oldstager. Repo origin sudah dituliskan konfigurasinya pada saat melakukan proses clone dari repo kontributor. Konfigurasi repo upstream harus dibuat.

![](image/tugas/004.png)

Tambahkan remote upstream

![](image/tugas/005.png)

Mengirimkan Pull Request Setiap kali melakukan perubahan, kirim perubahan tersebut. Pengiriman ini disebut dengan Pull Request. Pada posisi ini, kontributor bisa mengirimkan kontribusi dengan cara mengirimkan pull request (PR) ke upstream author. Secara umum, langkahlangkahnya adalah sebagai berikut:
a. Kontributor akan bekerja di repo lokal (create, update, delete isi)
b. Commit
c. Push ke repo kontributor
d. Kirimkan PR ke repo upstream author.
e. Upstream author me-review dan kemudian menyetujui (merge) ke master atau menolak PR.
f. Jika disetujui dan di-merge ke repo master dari upstream author, sinkronkan repo di komputer lokal dan repo GitHub kontributor.

Membuat Perubahan di Repo Lokal Sebelum melakukan perubahan, pastikan:
1. Sudah ada koordinasi secara manual tentang perubahan-perubahan yang akan dilakukan.
2. Setelah melakukan perubahan-perubahan, pastikan bahwa isi repo lokal tersinkronisasi dengan repo dari upstream author.
3. Lakukan perubahan-perubahan, setelah itu push ke origin (milik kontributor)
Setelah itu, buka halaman Web dari repo kontributor. Pada halaman tersebut akan ditampilkan isi yang kita push. Pilih Compare and pull request, kemudian isikan deskripsi PR dan klik pada Create pull request.

Pada repo upstream author, muncul angka 1 (artinya jumlahnya 1) pada Pull requests di bagian atas.
g. Upstream author bisa menyetujui setelah melakukan review: klik pada Pull requests, akan muncul PR dengan message seperti yang ditulis oleh kontributor (Add: contributor). Klik pada PR tersebut, review kemudian klik Merge pull request diikuti dengan Confirm merge. Setelah itu, status akan berubah menjadi Merged.
h. Sinkronkan semua repo (lokal maupun GitHub kontributor

Ada kemungkinan, jika satu orang mengirimkan PR untuk satu atau lebih file dan sementara itu ada lainnya juga yang mengirimkan PR pada satu atau lebih file yang sama, maka akan terjadi konflik karena ada satu atau lebih file yang sama yang di- edit dan akan di-merge. Jika sampai terjadi kasus seperti ini, maka upatream author harus menolak semua PR dan kemudian masing-masing kontributor diharapkan menyelesaikan secara manual (offline) kemudian memutuskan siapa yang akan mengirimkan PR.
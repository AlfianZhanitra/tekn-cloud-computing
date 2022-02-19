Latihan Instalasi GIT di windows
Sebelum install Git di Windows, anda harus sudah mempunyai editor teks yang didukung oleh Windws. Editor yang bisa dipilih banyak, tetapi disarankan menggunakan Notepad++ atau Visual Studion Code atau Vim.

1. Setelah selesai mendownload Git, lalu double click pada file yang telah di download. Kemudian muncul lisensi. Klik next untuk melanjutkan.

![](image/latihan/001.png)

2. Setelah itu, pilih lokasi instalasi. Secara default akan terisi C:\Program Files\Git. Ganti lokasi jika memang anda menginginkan lokasi lain, klik Next.

![](image/latihan/002.png)

3. Pilih komponen. Tidak perlu diubah-ubah, sesuai dengan default saja. Klik pada Next.

![](image/latihan/003.png)

4. Mengisi shortcut untuk menu Start. Gunakan default (Git), ganti jika ingin mengganti - misalnya Git VCS.

![](image/latihan/004.png)

5. Pilih editor yang akan digunakan bersama dengan Git. Pada pilihan ini, digunakan Notepad++.

![](image/latihan/005.png)

6. Pada saat instalasi, Git menyediakan akses git melalui Bash maupun command prompt. Pilih pilihan kedua supaya bisa menggunakan dari dua antarmuka tersebut. Bash adalah shell di Linux. Dengan menggunakan bash di Windows, pekerjaan di command line Windows bisa dilakukan menggunakan bash - termasuk ekskusi dari Git.

![](image/latihan/006.png)

7. Pilih OpenSSL untuk HTTPS. Git menggunakan https untuk akes ke repo GitHub atau repo-repo lain (GitLab, Assembla).

![](image/latihan/007.png)

8. Pilih pilihan pertama untuk konversi akhir baris (CR-LF).

![](image/latihan/008.png)

9. Pilih PuTTY untuk terminal yang digunakan untuk mengakses Git Bash.

![](image/latihan/009.png)

10. Untuk opsi ekstra, pilih yang bagian atas.

![](image/latihan/010.png)

11. Pilih default untuk git pull, pilih yang default.

![](image/latihan/011.png)

12. Pilih bantuan mandat, pilih Git credential Manager.

![](image/latihan/012.png)

13. Uncheck opsi konfigurasi experimental.

![](image/latihan/013.png)

14. Setelah itu proses instalasi akan dilakukan.

![](image/latihan/014.png)

15. Jika selesai akan muncul dialog pemberitahuan. Klik pada Finish.

![](image/latihan/015.png)

16. Untuk menjalankan, dari Start menu, ketikkan "Git", akan muncul beberapa pilihan. Pilih "Git Bash" atau "Git GUI”.

![](image/latihan/016.png)

17. Tampilan jika akan menggunakan "Git Bash".

![](image/latihan/017.png)

18. Tampilan jika akan menggunakan "Git GUI".

![](image/latihan/018.png)

19. Untuk mencoba dari command prompt, masuk ke command prompt, setelah itu eksekusi "git --version" untuk melihat apakah sudah terinstall atau belum.

![](image/latihan/019.png)


Konfigurasi GIT

Secara minimal, user harus memberitahu Git tentang username serta email yang digunakan setiap kali terjadi perubahan pada repo Git.
Username serta email ini yang akan dimasukkan oleh Git ke catatan perubahan di repo.
Di sistem operasi Linux atau sejanis (UNIX), konfigurasi ini nantinya akan disimpan di $HOME/.gitconfig.
Untuk sistem operasi Windows, konfigurasi ini akan disimpan di C:\Document and Settings\NamaUser dengan nama file .gitconfig.
Secara minimal, ada 2 hal yang perlu dikonfigurasi yaitu username dan email. Gunakan perintah berikut:

![](image/latihan/020.png)

Isian di atas harus disesuaikan dengan nama serta email yang digunakan untuk mendaftar di GitHub.
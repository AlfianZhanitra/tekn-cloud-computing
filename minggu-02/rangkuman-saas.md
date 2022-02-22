# Apa perbedaan antara IaaS, SaaS, dan Paas?

## SaaS: Software as a Service

Menjalankan aplikasi di cloud publik. Pengguna menggunakan aplikasi ini melalui Internet. Aplikasi ini dikelola oleh Penyedia Layanan, beberapa misalkan SalesForce, Microsoft (Office 365), Oracle, Google (Google Apps), dan lain-lain. Salesforce adalah perusahaan pertama yang mengubah dunia Saas.

## Iaas: Infrastruktur sebagai Layanan

Ini menyediakan lingkungan bagi pengembang untuk membangun aplikasi yang dapat digunakan pengguna. IaaS termasuk: 

1. Pengguna membuat mesin virtual (VM) sesuai permintaan.
2. Dari perpustakaan gambar VM.
Amazon (AWS) adalah vendor terkemuka dalam menyediakan IaaS.

## PaaS: Platform sebagai Layanan

Ini agak mirip dengan IaaS tetapi perbedaannya adalah:

Pengembang menyediakan aplikasi yang dijalankan oleh platform. Mereka tidak secara langsung membuat VM.
Anda akan berpikir bahwa PaaS sederhana dan itulah sebabnya banyak digunakan. Tapi ini tidak benar. IaaS 10 kali lebih populer dari PaaS. Pengembang ingin memiliki kontrol lebih besar atas sumber daya.


# SAAS (Software as a Service) Platform Architecture


Perangkat lunak sebagai layanan adalah lisensi perangkat lunak dan model pengiriman di mana perangkat lunak dilisensikan secara berlangganan dan di-host secara terpusat. Pengguna dapat mengaksesnya dengan bantuan web browser.

SaaS adalah model pengiriman umum untuk banyak aplikasi bisnis, termasuk perangkat lunak perkantoran dan perpesanan, perangkat lunak manajemen, virtualisasi, dll. Ini adalah bagian dari nomenklatur komputasi awan, bersama dengan infrastruktur sebagai layanan (IaaS), platform sebagai layanan (PaaS) , desktop sebagai layanan (DaaS).

Ini terkait dengan penyedia layanan aplikasi (ASP) yang menyediakan aplikasi "shrink-wrap" untuk pengguna bisnis melalui Internet. Perangkat lunak berbasis Internet awal memiliki fitur yang mirip dengan aplikasi lokal dibandingkan dengan aplikasi SaaS. Karena ini awalnya dibangun sebagai aplikasi penyewa tunggal, kemampuan mereka untuk berbagi data terbatas. Aplikasi SaaS adalah arsitektur instans tunggal, multi-penyewa yang memberikan pengalaman kaya fitur yang kompetitif dengan aplikasi di lokasi. Aggregator menggabungkan penawaran SaaS dari vendor yang berbeda dan menawarkannya sebagai bagian dari platform aplikasi terpadu.

Penyedia SaaS menghosting aplikasi dan data secara terpusat — menyebarkan patch . Mereka meningkatkan ke aplikasi secara transparan, memberikan akses ke pengguna akhir melalui Internet. Banyak vendor menyediakan API yang digunakan pengembang untuk membuat aplikasi komposit. Ini berisi berbagai mekanisme keamanan untuk keamanan Data selama transmisi dan penyimpanan.

Arsitektur SAAS:

Dengan model ini, satu versi aplikasi, dengan konfigurasi tunggal digunakan untuk semua pelanggan. Aplikasi diinstal pada beberapa mesin untuk mendukung skalabilitas (disebut penskalaan horizontal). Dalam beberapa kasus, versi kedua dari aplikasi diatur untuk menawarkan sekelompok pelanggan tertentu dengan akses ke versi pra-rilis aplikasi untuk tujuan pengujian. Dalam model tradisional ini, setiap versi aplikasi didasarkan pada kode unik. Meskipun pengecualian , beberapa solusi SaaS tidak menggunakan multitenancy, untuk mengelola sejumlah besar pelanggan dengan biaya yang efektif. Apakah multitenancy merupakan komponen yang diperlukan untuk software-as-a-service adalah topik kontroversi.

Ada dua jenis utama SaaS:

- SaaS Vertikal
Perangkat Lunak yang menjawab kebutuhan industri tertentu (misalnya, perangkat lunak untuk perawatan kesehatan, pertanian, real estat, industri keuangan)
- SaaS Horizontal
Produk yang berfokus pada kategori perangkat lunak (pemasaran, penjualan, alat pengembang, SDM) tetapi agnostik industri.

## Manfaat SAAS:

Ini menawarkan peluang besar bagi organisasi dari semua ukuran untuk mengalihkan risiko akuisisi perangkat lunak, dan untuk memindahkan TI dari pusat biaya reaktif menjadi bagian perusahaan yang proaktif dan menghasilkan nilai. Secara tradisional, menyebarkan sistem perangkat lunak skala besar telah menjadi usaha besar. Menyebarkan sistem ini di perusahaan besar membutuhkan biaya lebih. Persyaratan waktu, staf, dan anggaran untuk penyebaran sebesar ini mewakili risiko yang signifikan bagi organisasi dengan ukuran berapa pun, dan sering kali menempatkan perangkat lunak tersebut di luar jangkauan organisasi yang lebih kecil yang jika tidak dapat memperoleh banyak manfaat darinya. kegunaan. Model pengiriman sesuai permintaan mengubah beberapa hal ini. Aplikasi SaaS tidak memerlukan penyebaran infrastruktur besar di lokasi klien. Ini menghilangkan atau secara drastis mengurangi komitmen sumber daya di muka.

Integrasi dapat direncanakan dan dijalankan dengan sedikit usaha, menciptakan salah satu interval waktu-ke-nilai sesingkat mungkin untuk investasi TI besar. Ini juga memungkinkan sejumlah vendor SaaS untuk menawarkan “test drive” bebas risiko (dan seringkali benar-benar gratis) dari perangkat lunak mereka untuk jangka waktu terbatas, seperti 30 hari. Memberi pelanggan kesempatan untuk mencoba perangkat lunak sebelum mereka membelinya membantu menghilangkan banyak risiko seputar pembelian perangkat lunak.

## Bagaimana SaaS Mempengaruhi TI?

Setelah Anda membuat keputusan untuk mengejar SaaS, langkah selanjutnya adalah mempersiapkan transisi dengan menilai bagaimana penerapan akan memengaruhi aset TI yang ada. Melakukan uji tuntas adalah bagian rutin dari setiap proyek penyebaran infrastruktur TI yang sukses. Beberapa area yang harus diperhatikan dalam daftar periksa uji tuntas meliputi,Standar keamanan data : Memindahkan data bisnis penting "di luar tembok" menimbulkan risiko kehilangan data atau paparan informasi sensitif yang tidak disengaja. Nilai kebutuhan keamanan data Anda, dan pastikan penyedia memiliki langkah-langkah untuk memenuhi standar yang Anda tetapkan. Layanan pelaporan : Karena SaaS melibatkan penyerahan kendali langsung atas beberapa data Anda, pelaporan yang akurat dan bermanfaat sangat penting. Tentukan layanan pelaporan apa yang ditawarkan penyedia, dan apakah mereka kompatibel dengan persyaratan intelijen bisnis Anda.

## Dampak pada Peran dan Tanggung Jawab TI

Menambahkan SaaS dapat menyebabkan perubahan mendasar dalam peran departemen TI sebagai penyedia layanan informasi. Di masa lalu, sifat penyebaran perangkat lunak telah menempatkan petugas informasi kepala sebagai penjaga gerbang. Mereka dapat menggunakan hak veto dengan menyatakan bahwa mereka tidak akan menyimpannya di pusat data. Dengan SaaS , kontrol pusat data tidak harus sama dengan kontrol atas seluruh lingkungan komputasi perusahaan. Hal ini dapat menyebabkan penjaga gerbang takut kehilangan kendali.

## Kesimpulan

Perusahaan sebaiknya mempertimbangkan fleksibilitas dan implikasi manajemen risiko dari penambahan SaaS ke portofolio layanan TI mereka. Integrasi dan komposisi adalah komponen penting dalam strategi arsitektur Anda untuk menggabungkan SaaS dengan sukses sebagai anggota yang berpartisipasi penuh dari infrastruktur TI yang berpusat pada layanan Anda. Kami percaya bahwa masa depan komputasi perusahaan tidak akan murni di lokasi. Sebaliknya, mereka akan ada dalam harmoni simbiosis.

# Software as a Service SaaS Platform Architecture

SaaS juga merupakan salah satu pilar utama komputasi awan. Ledakan dalam komputasi Cloud, didorong oleh penyedia layanan cloud seperti Microsoft dengan Azure, Amazon Web Services (AWS), Oracle, dan IBM, telah melihat pertumbuhan produk dan layanan lain yang dikirimkan melalui internet termasuk model SaaS berikut:

- Infrastruktur sebagai Layanan
- Platform sebagai Layanan
- Pembelajaran Mesin sebagai Layanan
- dan masih banyak lagi

## Mengapa Menggunakan Arsitektur SaaS?
Infografio yang menunjukkan apa itu SaaS, PaaS, dan IaaS dan kegunaannya perangkat lunak telah didistribusikan ke pelanggan di berbagai saluran selama beberapa dekade terakhir. Saluran distribusi yang lebih baru di Software as a Service (atau SaaS).


# Cara membangun aplikasi SaaS berbasis cloud

1. Bangun untuk cloud

Saat membangun aplikasi SaaS (global), kemungkinan besar Anda sedang membangunnya di cloud. Cloud memiliki banyak keuntungan – pikirkan skalabilitas – berbeda dengan lingkungan server lokal.

Oleh karena itu posting ini, dan yang akan mengikuti fokus pada perangkat lunak yang dibangun dan direkayasa di cloud. Berikut cara membangun arsitektur SaaS berbasis cloud.

2. Bagaimana cara memulai aplikasi SaaS Anda?

3. Bahasa pemrograman yang mana?

Membangun produk untuk cloud berarti membangun produk dengan bahasa pemrograman modern.

Selain kemampuan dan keterampilan pribadi, pilihan bahasa pemrograman Anda akan dipengaruhi oleh kemungkinan setiap bahasa. Ada berbagai bahasa pemrograman (modern) di luar sana sehingga sulit untuk memilih yang tepat.

Python.
Python adalah bahasa pemrograman yang banyak digunakan, dirancang untuk menekankan pada keterbacaan kodenya.Python dapat melakukan banyak hal. Aplikasi web apa pun yang ingin Anda buat, kemungkinan besar ada kerangka kerja untuknya dengan Python.


Sumber Referensi :

https://www.quora.com/What-is-the-difference-between-IaaS-SaaS-and-Paas
https://hackernoon.com/saas-software-as-a-service-platform-architecture-757a432270f5
https://usersnap.com/blog/cloud-based-saas-architecture-fundamentals/
https://www.devteam.space/blog/saas-software-as-a-service-platform-architecture/
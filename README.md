**Analisis Keuntungan dan Diskon Penjualan Produk**

**Deskripsi Proyek**

Proyek ini bertujuan untuk menganalisis faktor-faktor yang menyebabkan kerugian dalam penjualan produk perusahaan dan memberikan rekomendasi untuk meningkatkan profitabilitas. Analisis ini dilakukan dengan menggunakan data penjualan dan diskon dari berbagai transaksi untuk mengidentifikasi pola kerugian serta menentukan strategi untuk memperbaikinya.

**Tujuan**

1. Menentukan faktor-faktor yang menyebabkan kerugian dalam transaksi penjualan produk.
2. Menganalisis pengaruh diskon terhadap keuntungan dan penjualan.
3. Memberikan rekomendasi untuk mengurangi kerugian dan meningkatkan profitabilitas.

**Data**

Dataset yang digunakan dalam analisis ini adalah SaaS-Sales.csv, yang mencakup informasi transaksi penjualan, seperti:

Row ID: Identifikasi unik untuk setiap transaksi.

Order ID: Identifikasi unik untuk setiap pesanan.

Order Date: Tanggal saat pesanan ditempatkan.

Date Key: Representasi numerik dari tanggal pesanan.

Contact Name: Nama orang yang melakukan pesanan.

Country: Negara tempat pesanan dilakukan.

City: Kota tempat pesanan dilakukan.

Region: Wilayah tempat pesanan dilakukan.

Subregion: Subwilayah tempat pesanan dilakukan.

Customer: Nama perusahaan yang melakukan pesanan.

Customer ID: Identifikasi unik untuk setiap pelanggan.

Industry: Industri yang dimiliki pelanggan.

Segment: Segmen pelanggan (SMB, Strategis, Enterprise, dll.).

Product: Produk yang dipesan.

License: Kunci lisensi untuk produk.

Sales: Jumlah total penjualan untuk transaksi.

Quantity: Jumlah total barang dalam transaksi.

Discount: Diskon yang diterapkan pada transaksi.

Profit: Keuntungan dari transaksi.

**Metodologi**

1. Pembersihan Data

* Pemeriksaan Data Kosong: Memastikan tidak ada nilai kosong atau duplikat dalam dataset.

* Pembersihan Data: Menghapus kolom yang tidak relevan untuk analisis seperti Row ID, Order ID, Order Date, Date Key, Contact Name, dan Customer ID.

2. Analisis Deskriptif

* Proporsi Transaksi Merugi: Menghitung persentase transaksi yang mengalami kerugian.

* Uji Normalitas: Menggunakan uji Shapiro-Wilk untuk menentukan apakah data distribusi normal.

* Korelasi: Menganalisis korelasi antara variabel Profit, Sales, Quantity, dan Discount menggunakan metode Spearman.

3. Analisis Korelasi dan Hubungan

* Analisis Korelasi: Menggunakan korelasi Spearman untuk menentukan hubungan antara variabel.

* Visualisasi: Membuat scatter plot dan grafik untuk menggambarkan hubungan antara variabel.

4. Uji Chi-Square

* Uji Hubungan Kategori: Menggunakan uji Chi-Square untuk menguji hubungan antara Profit dengan atribut kategori seperti Country, City, Region, Subregion, Customer, Industry, Segment, dan Product.

5. Analisis Kombinasi Atribut

* Identifikasi Kerugian: Menganalisis kombinasi atribut yang berkontribusi pada kerugian terbesar.

* Visualisasi Kerugian: Membuat bar chart untuk menggambarkan total kerugian berdasarkan kombinasi atribut.

6. Analisis Diskon

* Rata-Rata Diskon: Menghitung rata-rata diskon yang diterapkan pada transaksi yang merugi.

* Pengaruh Diskon: Menilai bagaimana diskon mempengaruhi keuntungan dan penjualan.

**Kesimpulan:**

1. Dampak Diskon pada Transaksi yang Merugi:
Setiap transaksi produk yang merugi selalu menerapkan diskon dengan rata-rata diskon sebesar 37.43%. Penerapan diskon, terutama di atas 30%, justru berdampak kecil pada penurunan sales dan  menyebabkan kerugian pada profit secara signifikan.

2. Potensi Peningkatan Sales dan Profit:
Menghilangkan diskon pada transaksi produk di kota-kota yang merugi dapat meningkatkan penjualan sebesar 29.33% dan profit sebesar 118.45%. Dengan menghindari diskon, penghematan uang dapat mencapai 140.423, dan profit yang didapat bisa meningkat menjadi 339.240.

**Rekomendasi:**

1. Hindari Diskon yang Berlebihan:
Untuk meningkatkan profitabilitas, hindari pemberian diskon yang besar. Jika ingin memberikan Discount, berikanlah diantara 0-10%, Hal ini berpotensi meningkatkan Sales tapi tidak menutup kemungkinan untuk mendatangkan kerugian seperti pada point ke-2.

2. Evaluasi Diskon di Kota-Kota yang Merugi:
Evaluasi dan hapus diskon untuk transaksi produk di kota-kota yang menunjukkan kerugian. Langkah ini berpotensi meningkatkan sales dan profit secara signifikan, serta mengurangi kerugian.

**Visualisasi**

Grafik dan plot yang menunjukkan hubungan antara diskon dan keuntungan.

Bar chart yang menggambarkan total kerugian berdasarkan atribut seperti City dan Product.

**Menggunakan**

1. Unduh Dataset: Pastikan SaaS-Sales.csv ada di direktori kerja.
2. Jalankan Skrip: Eksekusi skrip Python untuk melakukan analisis. Pastikan semua pustaka yang diperlukan telah terinstal.
3. Lihat Hasil: Periksa hasil analisis dan visualisasi yang dihasilkan untuk wawasan lebih lanjut.

**Instalasi dan Persyaratan**

Pastikan Anda telah menginstal pustaka berikut:
1. pandas
2. matplotlib
3. seaborn
4. scipy
5. numpy

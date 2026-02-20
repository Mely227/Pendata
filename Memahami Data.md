---
title: Memahami Data

---

##### Memahami Data

1. Pengertian Data
    Data adalah sekumpulan fakta atau informasi mentah yang dapat diolah menjadi informasi yang lebih bermakna. Dalam penambangan data (data mining), memahami jenis dan karakteristik data sangat penting sebelum melakukan analisis.

    Data bisa berasal dari berbagai sumber seperti manusia, mesin, sensor, media sosial, transaksi online, dan lain-lain.
    
2. Jenis-Jenis Data
* Data Terstuktur
Data terstruktur adalah data yang tersusun rapi dalam bentuk tabel (baris dan kolom), seperti di Excel atau database.Contohnya Data nilai mahasiswa,Data pelanggan,Data transaksi penjualan. Pada data terstruktur, setiap kolom disebut **atribut atau variabel**.
**Jenis Atribut pada Data Terstruktur:**
 **a. Nominal**
    Data berupa kategori tanpa urutan.
    Contoh: jenis kelamin, warna, jurusan.

   **b. Biner**
    Data yang hanya memiliki dua nilai.
    Contoh: Ya/Tidak, 0/1, Lulus/Tidak.

    **c. Ordinal**
    Data yang memiliki urutan, tetapi jarak antar nilainya tidak bisa dihitung.
    Contoh: kecil – sedang – besar.

    **d. Numerik**
    Data berupa angka yang bisa dihitung.
    Contoh: umur, tinggi badan, nilai ujian.
    
    
* Data Tidak Terstruktur
Data tidak terstruktur adalah data yang tidak memiliki format tetap dan tidak tersusun dalam tabel.Contohnya Email,Artikel,Chat,Dokumen teks.
Data jenis ini biasanya perlu diproses terlebih dahulu sebelum dianalisis.
* Data Bahasa Alami 
Data dalam bentuk bahasa manusia, seperti teks Bahasa Indonesia atau Bahasa Inggris.Contohnya Komentar media sosial,Review produk,Berita.
Untuk mengolah data ini biasanya digunakan teknik Pemrosesan Bahasa Alami (NLP).
* Data yang Dibuat oleh Mesin
Data yang dihasilkan otomatis dari alat atau mesin, misalnya log server atau sensor Internet of Things.
* Data Berbasis Graph
Data yang menggambarkan hubungan antar objek seperti jaringan pertemanan di media sosial.
* Data Multimedia
Data seperti audio, video, atau gambar yang biasanya berasal dari media digital dan memerlukan teknik khusus untuk diproses.
* Data Streaming
Data yang terus datang secara berurutan misalnya setiap detik data sensor atau transaksi online dan sering diproses secara berkelanjutan.

3. Distribusi Data
Distribusi data menunjukkan bagaimana data tersebar.
Salah satu distribusi yang sering ditemui adalah distribusi normal (berbentuk kurva lonceng), di mana sebagian besar nilai berada di sekitar rata-rata.
**Rumus Distribusi Normal:**
$$
f(x) = \frac{1}{\sigma \sqrt{2\pi}} 
e^{-\frac{(x - \mu)^2}{2\sigma^2}}
$$
Keterangan:
    - $\mu$ = mean (rata-rata)
    - $\sigma$ = standar deviasi (sigma)
    - $\sigma^2$ = variansi (sigma kuadrat)
    - $\pi$ = konstanta 3.14159
    - $e$ = bilangan Euler (≈ 2.718)
    
    Distribusi membantu kita memahami:
    * Apakah data seimbang
    * Apakah data miring ke kiri atau kanan
    * Apakah terdapat nilai yang tidak wajar
    
4. Statistik Deskriptif
Statistik deskriptif digunakan untuk merangkum dan menjelaskan data numerik.
    * Ukuran Pusat
**Mean (Rata-rata)**
Jumlah seluruh nilai dibagi banyaknya data.
Rumusnya:
$$
\text{Mean} = \bar{x} = \frac{1}{n} \sum_{i=1}^{n} x_i
$$
**Median**
Nilai tengah setelah data diurutkan.
Rumus:
Jika jumlah data ganjil:
$$
\text{Median} = x_{\frac{n+1}{2}}
$$
Jika jumlah data genap:
$$
\text{Median} = \frac{x_{\frac{n}{2}} + x_{\frac{n}{2}+1}}{2}
$$
Median Data Berkelompok (interval)
$$
Me = x_{ij} + \left( \frac{\frac{n}{2} - f_{kij}}{f_i} \right) p
$$
 Keterangan:

        - $Me$ = Median  
        - $x_{ij}$ = Batas bawah kelas median  
        - $n$ = Jumlah seluruh data  
        - $f_{kij}$ = Frekuensi kumulatif data di bawah kelas median  
        - $f_i$ = Frekuensi data pada kelas median  
        - $p$ = Panjang interval kelas  

        **Modus**
Nilai yang paling sering muncul.
Rumusnya:
$$
\text{Modus} = \text{nilai } x \text{ dengan frekuensi terbesar}
$$
    * Ukuran Sebaran
    Ukuran penyebaran digunakan untuk mengetahui seberapa jauh data menyebar dari nilai pusat (mean atau median).
        1.  Rentang (Range)
        $$
\text{Range} = X_{\text{maks}} - X_{\text{min}}
$$

            Range adalah selisih antara nilai terbesar dan nilai terkecil dalam data. 
Semakin besar range, semakin lebar penyebaran data.

        2.  Kuartil
        Kuartil membantu melihat posisi dan penyebaran data secara lebih rinci.
        Kuartil membagi data yang telah diurutkan menjadi empat bagian:
$Q_1 = \text{Kuartil bawah}$
$Q_2 = \text{Median}$  
$Q_3 = \text{Kuartil atas}$  

        3.  Interquartile Range (IQR)
        $$
IQR = Q_3 - Q_1
$$
IQR menunjukkan penyebaran 50% data tengah dan tidak terlalu dipengaruhi oleh nilai ekstrem.

        4.  Variansi
        Variansi dan standar deviasi adalah ukuran penyebaran data. Nilai-nilai tersebut menunjukkan bagaimana penyebaran distribusi data. Standar Deviasi yang rendah berarti bahwa pengamatan data cenderung sangat dekat dengan rata-rata, sedangkan deviasi standar yang tinggi menunjukkan data tersebar di sejumlah nilai-nilai besarVariansi mengukur rata-rata kuadrat penyimpangan data terhadap mean.

        2.  Standar Deviasi
        Populasi:
        $$
\sigma = \sqrt{\sigma^2}
$$
Sampel:
$$
s = \sqrt{s^2}
$$
Standar deviasi menunjukkan seberapa jauh data menyimpang dari rata-rata dalam satuan asli data.
Semakin besar nilainya, semakin menyebar datanya.

5. Skewness (Kemencengan)
        Skewness adalah ukuran yang menunjukkan arah dan tingkat kemiringan distribusi data terhadap rata-rata.
    * Skewness Positif (Miring ke Kanan)
    Ciri:
        - Ekor distribusi lebih panjang di sebelah kanan
        - Mean lebih besar dari median
$$
\text{Mean} > \text{Median} > \text{Modus}
$$
Distribusi condong ke kanan karena terdapat beberapa nilai yang sangat besar.
    * Skewness Negatif (Miring ke Kiri)
    Ciri:
        - Ekor distribusi lebih panjang di sebelah kiri
        - Mean lebih kecil dari median
$$
\text{Mean} < \text{Median} < \text{Modus}
$$
Distribusi condong ke kiri karena terdapat beberapa nilai yang sangat kecil.
    * Distribusi Simetris
    Ciri:
        - Bentuk kiri dan kanan sama
        - Tidak memiliki kemiringan

$$
\text{Mean} = \text{Median} = \text{Modus}
$$
**Rumus Skewness (Populasi)**

$$
\gamma_1 = \frac{\frac{1}{N} \sum_{i=1}^{N} (x_i - \mu)^3}{\sigma^3}
$$

Keterangan:
- $\gamma_1$ = Koefisien skewness
- $\mu$ = Mean populasi
- $\sigma$ = Standar deviasi
- $N$ = Jumlah data
- $x_i$ = Nilai data ke-i

Jika:
- $\gamma_1 > 0$ → Skewness positif  
- $\gamma_1 < 0$ → Skewness negatif  
- $\gamma_1 = 0$ → Distribusi simetris
    
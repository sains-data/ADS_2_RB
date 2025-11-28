# Tugas Besar ADS 2025 Kelompok 2 RB
# Analisis Perbedaan Rata-Rata Indeks Prestasi Kumulatif (IPK) Mahasiswa ITERA Menggunakan Uji Hipotesis Satu Populasi dan Dua Populasi
# Anggota Kelompok :
1. Muhammas Syafiqul Falakh_124450099
2. Hani Qurrota Aini_124450020
3. Adinda Deswita Maharani_124450083
4. Ayake Alfatih Ramadan_124450108
   
# Deskripsi Singkat Proyek
Proyek ini berfokus pada analisis IPK mahasiswa ITERA berdasarkan beberapa faktor demografis dan sosial akademik. Tujuan utamanya adalah mengetahui apakah terdapat perbedaan signifikan pada IPK berdasarkan:
1. Program Studi (Sains Data vs Non–Sains Data)
2. Status Beasiswa (Penerima Beasiswa vs Non-Beasiswa)
3. Rata-rata populasi tunggal (menguji apakah IPK mahasiswa > 3.00)

Analisis dilakukan menggunakan uji statistik parametrik (t-test), visualisasi data, pembersihan data, dan pemetaan kategorikal.
Variabel utama yang dianalisis:
1. IPK mahasiswa
2. Program studi
3. Status penerima beasiswa

# Paket R yang Digunakan
Script menggunakan beberapa library berikut:
1. library(readr)
2. library(dplyr)
3. library(stringr)
4. library(ggplot2)

# Struktur Repositori
1. data : Dataset Tugas Besar ADS 2025.csv
2. src : analysis.Rmd #Source code utama (R Markdown)
3. output : grafik #Semua hasil visualisasi, hasil_analisis # Hasil uji statistik dan interpretasi
4. README.md # Dokumentasi proyek

# Cara Menjalankan Script
1. Clone repositori : git clone https://github.com/username/Tugas-Besar-ADS-2025.git
2. Buka file R Markdown : Jalankan di RStudio, Pastikan dataset berada di folder data
4. Knit / Render file .Rmd : Output berupa HTML otomatis dihasilkan.

# Penjelasan Singkat Dataset
Dataset berisi data mahasiswa ITERA dengan beberapa variabel terkait akademik dan demografis.
Kolom yang digunakan dalam analisis ini:
1. Program Studi dikategorikan menjadi: Sains Data dan Non–Sains Data
2. IPK melalui proses pembersihan: Mengganti koma menjadi titik, Mengambil angka valid, Membuang nilai tidak wajar (≤0 atau >4)
3. Status Beasiswa diolah menjadi: Penerima Beasiswa, Non-Beasiswa

# Metode Analisis
1. Pembersihan Data : Standarisasi penulisan IPK, Penanganan karakter non alfabet pada nama prodi, Pengelompokan “Sains Data vs Non Sains Data”
2. Eksplorasi Data & Visualisasi : Histogram IPK, Boxplot IPK tiap kelompok, Violin plot, Density plot, QQ Plot (cek normalitas residual)
3. Uji Hipotesis : Uji t satu sampel, Menguji apakah rata-rata IPK mahasiswa > 3.00, Uji t dua sampel (independen), IPK Sains Data vs Non Sains Data, IPK Penerima Beasiswa vs Non Beasiswa, Visualisasi kurva distribusi t dan daerah p-value

# Ringkasan Temuan (isi setelah analisis jadi)
Tambahkan ringkasan hasilmu, contoh format: Rata-rata IPK mahasiswa ITERA adalah, Tidak atau ada perbedaan signifikan pada IPK berdasarkan kelompok prodi, Tidak atau ada perbedaan signifikan pada IPK berdasarkan status beasiswa, Rata-rata IPK terbukti lebih besar dari 3.00 gagal dibuktikan

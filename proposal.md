
# PROPOSAL PROYEK AKHIR
## Perancangan Proyek Rekap dan Analisis Nilai Matematika

### 1. Latar Belakang

Pengolahan nilai merupakan salah satu kegiatan untuk mengetahui hasil belajar. Proses pengolahan nilai secara manual membutuhkan waktu, terutama ketika harus menghitung rata-rata, nilai tertinggi, nilai terendah, serta menentukan jumlah nilai yang tuntas dan belum tuntas.

Oleh karena itu, dibuat program sederhana menggunakan bahasa pemrograman Python untuk membantu proses rekap dan analisis nilai secara lebih cepat dan terstruktur. Program ini diharapkan dapat mengurangi kesalahan perhitungan serta menghasilkan laporan yang mudah dibaca.

### 2. Tujuan

Tujuan pembuatan program ini adalah:
1. Mempermudah proses rekap data nilai.
2. Menghitung total, rata-rata, nilai minimum, dan nilai maksimum secara otomatis.
3. Menentukan jumlah nilai tuntas dan belum tuntas berdasarkan KKM.
4. Memvalidasi nilai agar berada dalam rentang 0–100.
5. Menghasilkan laporan analisis nilai yang dapat disimpan dalam file teks.

### 3. Deskripsi Program

Program Rekap dan Analisis Nilai Matematika merupakan program berbasis teks yang dibuat menggunakan bahasa pemrograman Python. Program membaca data nilai yang disimpan dalam file teks. Data tersebut kemudian diproses untuk menghasilkan informasi statistik dan status ketuntasan berdasarkan KKM 75.

Hasil pengolahan ditampilkan melalui terminal dan disimpan dalam file laporan agar dapat dibaca kembali.

### 4. Rancangan Program

Program dirancang menggunakan beberapa modul agar setiap bagian memiliki tugas yang jelas.

**Input:** File `data/nilai_contoh.txt` yang berisi angka nilai, dengan satu nilai pada setiap baris.

**Proses:**
1. Membaca data nilai dari file.
2. Memvalidasi data dan memastikan nilai berupa angka.
3. Memastikan nilai berada dalam rentang 0–100.
4. Menghitung jumlah data, total, rata-rata, nilai minimum, dan maksimum.
5. Menentukan status ketuntasan berdasarkan KKM 75.
6. Menyusun hasil perhitungan menjadi laporan.

**Output:** Laporan yang ditampilkan di terminal dan disimpan ke `output/laporan_nilai.txt`.

**Pembagian modul:**
- `main.py`: menjalankan alur utama program.
- `data_io.py`: membaca data dan menyimpan laporan.
- `analisis.py`: menghitung statistik dan ketuntasan.
- `utilitas.py`: menyusun laporan agar mudah dibaca.

**Algoritma program:**
1. Mulai.
2. Membaca data nilai dari file.
3. Memvalidasi setiap nilai.
4. Jika tidak ada data valid, tampilkan pesan.
5. Jika ada data valid, hitung statistik dan ketuntasan.
6. Tampilkan hasil analisis.
7. Simpan laporan ke file teks.
8. Selesai.

### 5. Data Masukan

Data masukan berupa file teks bernama `nilai_contoh.txt` yang berada dalam folder `data`. Setiap baris berisi satu angka nilai tanpa nama atau kode identitas.

Contoh data masukan:

    85
    78
    90
    65
    75
    100
    0

Data contoh terdiri atas tujuh nilai. Program menerima nilai dari 0 sampai 100. Data yang bukan angka atau memiliki nilai di luar rentang tersebut akan ditolak dan diberikan pesan peringatan.

### 6. Keluaran Program

Keluaran program berupa laporan rekap dan analisis nilai yang ditampilkan di terminal serta disimpan dalam file `output/laporan_nilai.txt`.

Laporan memuat:
1. Jumlah data valid.
2. Total nilai.
3. Rata-rata nilai.
4. Nilai minimum dan maksimum.
5. KKM yang digunakan.
6. Jumlah nilai tuntas dan belum tuntas.
7. Rincian setiap nilai beserta status ketuntasannya.

Nilai dinyatakan tuntas apabila mencapai KKM 75 atau lebih. Nilai di bawah 75 dinyatakan belum tuntas.

### 7. Pengujian

Pengujian dilakukan untuk memastikan program berjalan sesuai kebutuhan. Pengujian mencakup kondisi normal, batas, dan input tidak valid.

| ID | Kategori | Input/Kondisi | Hasil yang Diharapkan |
|---|---|---|---|
| TC01 | Normal | Nilai 80, 70, 90 | Rata-rata 80 |
| TC02 | Batas | Nilai 0 | Diterima sebagai nilai valid |
| TC03 | Batas | Nilai 100 | Diterima sebagai nilai valid |
| TC04 | Invalid | Nilai 105 | Ditolak dengan peringatan |
| TC05 | Invalid | Nilai berupa teks `abc` | Baris ditolak |
| TC06 | Invalid | File tidak ditemukan | Pesan kesalahan ditampilkan |
| TC07 | Normal | Semua nilai minimal 75 | Semua nilai dinyatakan tuntas |
| TC08 | Batas | Nilai 75 dan 74 | 75 tuntas, 74 belum tuntas |

Pengujian dilakukan dengan menjalankan program di VS Code, mengganti data masukan sesuai skenario, kemudian membandingkan hasil aktual dengan hasil yang diharapkan. Hasil pengujian dicatat setelah setiap skenario benar-benar dijalankan.

### 8. Penutup

Program Rekap dan Analisis Nilai Matematika dirancang untuk membantu proses pengolahan nilai secara sederhana, cepat, dan terstruktur. Program ini menerapkan konsep dasar Python, struktur data, modularisasi, validasi, serta pengujian program.

Melalui proyek ini, diharapkan proses rekap dan analisis nilai menjadi lebih mudah dilakukan. Program juga dapat dikembangkan lebih lanjut dengan menambahkan fitur pengurutan nilai atau pengolahan data dalam jumlah yang lebih besar.

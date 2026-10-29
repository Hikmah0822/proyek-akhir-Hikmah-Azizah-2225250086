
# Proyek Rekap dan Analisis Nilai Matematika

## Identitas Mahasiswa
- **Nama:** Hikmah Azizah

- **NIM:** 2225250086

- **Kelas:** 3B

## Deskripsi Proyek
Program Python untuk membaca data nilai matematika, memvalidasi nilai, dan menghitung statistik nilai mahasiswa.

## Fitur Program
- Membaca data nilai dari file teks.
- Memvalidasi nilai dalam rentang 0–100.
- Menghitung jumlah data, total, rata-rata, nilai minimum, dan maksimum.
- Menentukan ketuntasan berdasarkan KKM 75.
- Menyimpan laporan hasil analisis ke dalam file teks.

## Struktur Folder
- `src/main.py`: menjalankan program utama.
- `src/data_io.py`: membaca data dan menyimpan laporan.
- `src/analisis.py`: menghitung statistik dan ketuntasan.
- `src/utilitas.py`: menyusun laporan.
- `data/nilai_contoh.txt`: menyimpan data nilai.
- `tests/test_case.md`: berisi skenario pengujian.
- `output/`: menyimpan hasil laporan.

## Cara Menjalankan Program
1. Buka folder proyek di Visual Studio Code.
2. Buka terminal.
3. Jalankan perintah berikut:

```bash
python src/main.py
```

## Data Contoh
Data nilai disimpan dalam `data/nilai_contoh.txt`, dengan satu nilai pada setiap baris.

## Hasil yang Diharapkan
Program menampilkan jumlah data, total nilai, rata-rata, nilai minimum, nilai maksimum, jumlah mahasiswa tuntas, dan jumlah mahasiswa belum tuntas. Hasilnya juga disimpan dalam `output/laporan_nilai.txt`.

## Pengujian
Pengujian dilakukan menggunakan skenario pada file `tests/test_case.md`, termasuk nilai valid, nilai di luar rentang, data bukan angka, dan file yang tidak ditemukan.

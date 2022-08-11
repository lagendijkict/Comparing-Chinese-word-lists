# Dapat kata baru di daftar kosa kata

## Pengantar
Waktu belajar Bahasa Mandarin, saya sering nemu kosakata baru yang ingin saya simpan.
Aplikasi favorit saya adalah [Quizlet](https://quizlet.com/latest) yang mudah digunakan di komputer dan hp.

Salah satu website yang saya pakai untuk mencari kosakata & bahan latihan adalah [Mandarin Corner](https://mandarincorner.org/).
Mereka punya beragam bahan latihan dalam Bahasa Cina dengan harga yang terjangkau.
Mereka juga punya daftar kosakata yang panjang, dan saya pikir, berapa dari kosakata ini yang sudah ada di daftar Quizlet saya?
Saya bisa baca satu persatu, tapi agak membosankan karena saya sudah tahu banyak dari daftar kosakata tersebut.

## Sasaran proyek ini
* Memasukkan konten sumber data Excel (tua)
* Memasukkan konten sumber data Excel (baru)
* Membandingkan dua-duanya
* Menerjemahkan konten baru

## Modul yang diperlui
* [pandas](https://pypi.org/project/pandas/) (semua versi terkini)
* [googletrans](https://pypi.org/project/googletrans/) versi 4.0.0-rc1 (atau lebih baru)

Instalasi lewat pip

## Selangkah demi selangkah

0. Untuk menghindari hasil ganda di daftar, punya dokumen Excel yang mengandung semua kata (hanya Bahasa sumber: Cina).
Jika belum punya, tapi masih ingin menyusul README ini, harus mengekspor daftar Quizlet. Info lebih lanjut disini:
[Mengekspor daftar](https://help.quizlet.com/hc/id/articles/360034345672-Mengekspor-set)
Tempel hasilnya dalam kolom Excel dengan nama kolom Term
1. Salin data dari halaman web kosa kata sesuai dengan kebutuhan Anda. Tempel hasil dalam new_data.csv
Jangan sampai lupa hak cetak ya, hanya _scraping_ jika nggak ada aturan yang melarang.

Untuk tahap yang lain, jalankan setiap sel di Jupyter Notebook.

## Info lain
Jika ingin ganti Bahasa tujuan, tolong baca [Googletrans docs](https://py-googletrans.readthedocs.io/en/latest/) untuk dapat pengertian lebih dalam dan mengubah save_new_vocab_into_list fungsi.

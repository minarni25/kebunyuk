KEBUNYUK / PEKARANGTANI — versi responsif dengan foto tanaman yang diperbaiki

MENJALANKAN
1. Ekstrak ZIP.
2. Pastikan index.html, HEADER1.png, dan folder assets berada di lokasi yang sama seperti struktur ZIP.
3. Buka index.html dengan Chrome/Edge.
4. Untuk hosting, unggah semua isi folder secara utuh.

FITUR
- Header gambar awal dipertahankan.
- Form menggunakan pilihan radio/tombol, bukan dropdown.
- Enam kriteria: media tanam, matahari, perawatan, tujuan, kategori, waktu panen.
- Hasil rekomendasi Top 3 berdasarkan bobot pada kode awal.
- Tombol Ubah Kriteria dan Ulangi Rekomendasi.
- Kartu hasil lebih seimbang dan responsif.
- Foto tanaman dibersihkan dari sebagian bingkai katalog lama, dibuat latar putih, dan disimpan dalam format 1200 x 900 piksel.
- Foto jahe memakai sumber HD yang baru dibuat; cabai rawit dan kencur menggunakan sumber foto terpisah jika tersedia.

CATATAN FOTO
Resolusi keluaran aset diseragamkan menjadi 1200 x 900 piksel, tetapi gambar lama yang sumbernya beresolusi rendah tidak otomatis memperoleh detail fotografi baru hanya dengan diperbesar. Sebelum publikasi final, foto tanaman lain sebaiknya diganti dengan foto asli/berlisensi atau sumber HD masing-masing.


PANDUAN KATEGORI
- Tombol "Lihat penjelasan dan daftar tanaman" membuka/menutup penjelasan kategori.
- Panel tertutup saat halaman pertama dibuka agar tidak membuat halaman penuh.
- Kategori: Sayuran Daun, Sayuran Buah, Bumbu Dapur, Tanaman Rimpang, dan Bebas.
- Nama tanaman pada kartu hasil diperjelas: Kangkung Darat, Bayam Hijau, Sawi Hijau, Pakcoy Hijau, Cabai Rawit Merah-Hijau, Tomat Merah, dan Terong Ungu.


PANDUAN KATEGORI — DAFTAR LENGKAP KATALOG
Panduan kategori kini mencantumkan seluruh 14 tanaman pada katalog aplikasi:
- Sayuran Daun: Kangkung Darat, Bayam Hijau, Sawi Hijau, Pakcoy Hijau.
- Sayuran Buah: Cabai Rawit Merah-Hijau, Tomat Merah, Terong Ungu.
- Bumbu Dapur: Serai, Daun Bawang, Bawang Merah, Bawang Putih, Kemangi.
- Tanaman Rimpang: Jahe, Kunyit, Kencur, Lengkuas, Temulawak.
Setiap tanaman dilengkapi keterangan bagian yang dimanfaatkan dan estimasi panen sesuai data katalog.
Panel panduan tetap tersembunyi sampai tombol diklik.


REVISI TATA LETAK DAN TUJUAN MENANAM
- Kartu "Bebas — Semua Kategori" ditampilkan sebagai satu kotak full-width di bagian atas panduan kategori.
- Pada desktop, pilihan "Seberapa cepat ingin panen?" ditempatkan tepat di bawah "Apa tujuanmu menanam?".
- Pada layar kecil, posisi pertanyaan kembali mengikuti alur responsif.
- Label tujuan diperjelas:
  * Konsumsi Keluarga: tanaman untuk dimakan keluarga.
  * Stok Bumbu Dapur: tanaman untuk persediaan bumbu masak.
  * Hobi: berkebun untuk kesenangan atau aktivitas.
  * Dijual / Penghasilan: tanaman untuk hasil panen yang ingin dipasarkan.


LOGIKA TUJUAN MENANAM DINAMIS
- Pilihan tujuan dibangun berdasarkan kategori yang dipilih.
- Sayuran/sayuran buah: konsumsi keluarga, dijual/penghasilan, hobi, bebas.
- Bumbu/rimpang: persediaan dapur, dijual/penghasilan, hobi, bebas.
- Bebas/semua kategori: semua tujuan umum.
Catatan: periksa kesesuaian nama radio kategori di HTML dengan fungsi kategoriAktif() jika kategori tidak terdeteksi saat pengujian.


REVISI FILTER KATEGORI DAN JUMLAH HASIL
- Kategori pilihan menjadi filter wajib: kategori sayuran hanya menampilkan tanaman berkategori "sayuran"; sayuran buah hanya "sayuran_buah"; bumbu hanya "bumbu"; rimpang hanya "rimpang".
- Pilihan "Bebas" tetap dapat menampilkan tanaman dari semua kategori.
- Sistem mengurutkan hasil yang lolos filter berdasarkan skor kecocokan.
- Maksimal 7 rekomendasi ditampilkan: 3 teratas dalam kartu besar dan maksimal 4 pilihan tambahan dalam kartu ringkas.
- Jika katalog kategori memiliki kurang dari 7 tanaman, sistem hanya menampilkan tanaman yang tersedia di kategori tersebut.
- Jika foto gagal dimuat, gambar disembunyikan agar tidak menampilkan foto tanaman lain yang salah.


REVISI SKOR DAN PANEN
- Skor akhir mempertimbangkan kecocokan kondisi pekarangan serta prioritas waktu panen.
- Jika memilih panen cepat, tanaman yang lebih cepat dipanen dalam kategori tersebut mendapat prioritas lebih tinggi.
- Urutan akhir menggunakan skor akhir; jika seri, tanaman dengan perkiraan panen lebih cepat didahulukan.
- Hasil dibatasi maksimal 7 tanaman. Kategori Sayuran Buah saat ini memiliki 3 tanaman dalam katalog sehingga hanya 3 hasil dapat ditampilkan. Untuk menampilkan 7 pilihan, katalog perlu ditambah dengan komoditas/varietas lain yang sesuai dan foto akurat.
- Gambar yang gagal dimuat disembunyikan; tidak memakai foto jahe sebagai gambar pengganti.


RESPONSIVITAS TOP 7
- Desktop: 3 kartu rekomendasi utama dalam tiga kolom; rekomendasi peringkat 4–7 tampil sebagai kartu ringkas dalam empat kolom.
- Tablet/laptop kecil: kartu utama tersusun dua kolom, kartu ketiga dipusatkan agar proporsional; rekomendasi tambahan dua kolom.
- HP: kartu utama satu kolom; rekomendasi tambahan satu kolom berbentuk ringkas dengan foto kecil; tombol tindakan memenuhi lebar layar.
- HP sangat kecil: ukuran foto dan jarak diperkecil untuk mencegah overflow horizontal.
Catatan: tampilan akhir tetap perlu diuji pada browser/perangkat nyata.


REVISI PERINGKAT TOP 7 DAN TUJUAN
- Label tujuan ekonomi disederhanakan menjadi "Dijual".
- Kartu hasil ke-4 sampai ke-7 menampilkan label peringkat secara eksplisit.
- Judul bagian hasil tambahan menjadi "Peringkat 4–7".
- Jika kategori memiliki kurang dari 4 tanaman, aplikasi memberi penjelasan jumlah tanaman yang tersedia dan tidak mencampur kategori lain.
- Untuk kategori Sayuran Buah saat ini tersedia 3 tanaman, sehingga diperlukan penambahan komoditas yang benar-benar berbeda agar dapat menampilkan peringkat 4–7 pada kategori tersebut.


REVISI TUJUAN MENANAM RINGKAS
- Label tujuan Dijual dipertahankan singkat.
- Deskripsi "buah atau polong" dihapus karena tidak sesuai untuk semua tanaman.
- Keterangan pilihan dipersingkat agar kartu tidak melebar atau turun ke baris berikutnya secara berlebihan.
- Contoh deskripsi: "Untuk dijual", "Untuk dimakan keluarga", "Untuk persediaan bumbu", "Untuk hobi berkebun".


REVISI PILIHAN TUJUAN DAN KATALOG
- Pilihan tujuan hanya: Dijual, Konsumsi, Hobi, Bebas; tanpa penjelasan di bawah tombol.
- Menambahkan Kacang Panjang sebagai komoditas Sayuran Buah.
- Kacang Panjang memakai aset lokal assets/tanaman/kacang-panjang.jpg yang sudah ada.
- Keterangan katalog menyebut panen sekitar 45–60 hari dan kebutuhan ajir/rambatan.
- Jumlah tanaman katalog menjadi 15. Kategori Sayuran Buah kini memiliki 4 tanaman.


PERBAIKAN FOTO DAN ESTIMASI RIMPANG
- Foto Serai diperbarui menjadi foto serai segar dengan batang pangkal yang tebal dan daun panjang.
- Foto Temulawak dipisahkan dari foto Kunyit; gambar menunjukkan rimpang berwarna kuning-oranye.
- Foto Lengkuas dipisahkan dari foto Kencur; gambar menunjukkan rimpang besar berkulit krem-kemerahan.
- Estimasi panen Temulawak diperbarui menjadi sekitar 9–10 bulan, sedangkan Kunyit tetap 8–10 bulan.
- Peringkat ditentukan oleh skor kecocokan keseluruhan; bila skor sama, tanaman dengan estimasi panen lebih cepat didahulukan.


REVISI FORMULA SKOR KECocokan (100 POIN)
- Media tanam: 25 poin.
- Sinar matahari: 25 poin.
- Waktu perawatan: 15 poin.
- Tujuan menanam: 15 poin.
- Preferensi waktu panen: 20 poin.
- Kategori tanaman adalah filter wajib, bukan bonus skor.
- Tujuan "Bebas" tidak mengurangi skor karena pengguna tidak menetapkan tujuan khusus.
- Skor akhir adalah jumlah poin dari kriteria yang cocok; tidak ada lagi pengali 60% atau bonus panen tambahan.
- Urutan: skor tertinggi dahulu; jika skor sama, estimasi panen lebih cepat dahulu; jika masih sama, urut nama.
- Skor adalah indeks kecocokan berbasis aturan aplikasi, bukan probabilitas keberhasilan panen.

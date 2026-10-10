# Pengaturan judul dan periode dari Google Sheets

1. Nama tab tetap Rate.
2. Isi sel A1 dengan judul dashboard yang diinginkan (opsional). Baris header FASKES diletakkan di baris 2 atau sesudahnya. Jika A1 kosong, judul dibuat otomatis berdasarkan bulan berjalan.
3. Untuk periode Oktober: header bulan sebelumnya “Capaian Jlh Rujukan September”; header berjalan “Capaian Jlh Rujukan sd 5 Oktober”.
4. Untuk November, ganti kedua header menjadi “Capaian Jlh Rujukan Oktober” dan “Capaian Jlh Rujukan sd 7 November”, lalu isi data sesuai periodenya. Tahun boleh ditambahkan setelah bulan. Bulan mengikuti header, bukan tanggal komputer.
5. Sesuaikan pula header dan nilai Sisa Rujukan November serta target bulanan. Dashboard tidak memindahkan data antarbulan sendiri.
6. Kolom peserta tidak tampil pada tabel dashboard. Kolom sumber peserta boleh tetap ada atau dihapus; koneksi Google Sheets mencari kolom berdasarkan nama.
7. Urutan akhir tabel: rujukan berjalan, sisa target, capaian vs target, status. Persentase capaian dibulatkan tanpa desimal; status tetap dihitung dari angka asli.
8. Warna angka bulan sebelumnya: merah di atas target, hijau sama dengan/di bawah target, abu-abu jika capaian/target kosong. Status utama memakai bulan berjalan dengan target bulanan penuh, tanpa prorata.

## Pemasangan
Ekstrak ZIP, unggah index.html ke folder utama repositori GitHub menggantikan file lama, lalu Commit changes. Setelah publikasi selesai, muat ulang dashboard dan klik Muat data Google Sheets.

Google Sheets harus dapat dibaca tanpa login, dengan hak edit hanya untuk pengelola. Koneksi memuat data saat halaman dibuka atau tombol muat ditekan; pembaruan Google dapat mengalami jeda. Sinkronisasi judul dan bulan berlaku pada koneksi Google Sheets. Unggah Excel/CSV lokal adalah pratinjau sementara dengan format lama, bukan publikasi.

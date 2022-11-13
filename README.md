# SIG-Teori-Modul14-SearchingandDownloadingOpenStreetMapData

## Prosedure

1. Cari dan pasang plugin QuickOSM dari QGIS Official Plugin Repository. Lihat Menggunakan Plugin untuk instruksi mengunduh plugin. Pastikan Anda telah memilih kotak centang. Klik Tutup.

2. Setelah diinstal, luncurkan plugin dari Vector ‣ QuickOSM ‣ QuickOSM… .

3. Di tab Kueri cepat , Anda dapat menyetel filter untuk memilih subkumpulan. Atribut fitur peta dalam database OSM disimpan sebagai Tag . Tag diwakili dengan kunci dan nilai. Kuncinya adalah topik dan nilai adalah bentuk spesifik. Lihat halaman wiki Fitur Peta OSM untuk daftar lengkap tag untuk berbagai jenis fitur. Bilah diwakili menggunakan tag amenity:bardan pub dengan tag amenity:pub. Kami pertama-tama akan mengekstrak bilah. Pilih amenitysebagai Kunci dari menu drop-down.

4. Pilih bardari menu tarik-turun Nilai .

5.Kami dapat menghubungkan beberapa kueri dalam versi terbaru (v2.0.0 +) dari plugin QuickOSM. Klik tombol plus, bilah pemilihan kueri berikutnya akan muncul. Klik pada kotak pilihan pertama di mana kita bisa mendapatkan opsi Anddan Or. Dan hanya akan memilih fitur yang benar untuk semua kueri. Atau akan memilih semua fitur yang benar untuk salah satu kueri. Klik Oruntuk memilih fitur bar dan pub.

6. Pilih amenitysebagai Kunci dari menu drop-down. Kemudian pilih pubdari menu tarik-turun Nilai .

7. Masukkan Londonsebagai Masuk untuk membatasi pencarian di dalam batas kota.

8. Luaskan bagian Lanjutan . Dalam model data OSM, fitur direpresentasikan menggunakan node, cara, dan relasi . Karena kami tertarik dengan fitur poin, Anda hanya dapat memilih Nodedan Points. Klik Jalankan kueri .

9. Setelah kueri selesai, alihkan ke jendela utama QGIS. Anda akan melihat layer baru bernama amenity_bar_amenity_pub_Londonditambahkan ke panel Layers . Kanvas akan menunjukkan lokasi bar dan pub yang diekstraksi.

10. Buka tabel Atribut pada layer. Ada 2091fitur. Kemudahan kolom berisi kategori apakah fitur tersebut pubatau bar. Dengan menggunakan kolom kategoris ini, mari menata layer kita.

11. Klik icon panel Open the Layer StylingCategorized , pilih lalu di Value pilih amenitylalu klik Classify . Sekarang layer akan ditata dengan 2 warna yang menampilkan keduanya barsdan pubs.

12. Sekarang klik kanan pada layer, Export ‣ Save Feature As… untuk mengekspor layer sebagai GeoPackage.

13. Di kotak dialog Save Vector Layer as… , di Format pilih GeoPackage, di File name klik ...dan telusuri ke direktori tempat Anda ingin menyimpan data dan beri nama outputnya london.gpkg. Dalam nama Lapisan masukkan bar_and_pubs. Klik Oke .

14. Sekarang lapisan GeoPackage london_bar_and_pubsakan ditambahkan ke kanvas.

15. Selesai.


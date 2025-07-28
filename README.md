# 🛒 Global Superstore Sales Analysis

## 🌍 Background 
Dataset ini berisi mengenai data sales retail dari global superstore selama 4 tahun. Dataset ini diambil dari platform Kaggle

Source
https://www.kaggle.com/datasets/rohitsahoo/sales-forecasting?resource=download

## 📝 Dataset Information
Dataset ini berisi satu file yaitu `sales.csv` dengan `5000 entry data` dan jumlah kolom sebanyak `18 kolom` yang terdiri sebagai berikut:
```
- Row ID = nilai unik berupa angka numerik berurutan
- Order ID = identitas unik setiap pesanan
- Order Date = tanggal setiap pesanan dibuat
- Ship Date = tanggal setiap pesanan dikirim
- Ship Mode = metode atau jenis pengiriman
- Customer ID = identitas unik setiap pelanggan
- Customer Name = nama pelanggan yang melakukan pembelian
- Segment = segmentasi pelanggan yang melakukan pembelian
- Country = negara asal pelanggan
- City = kota asal pelanggan
- State = state asal pelanggan
- Postal Code = kode pos asal pelanggan
- Region = pembagian wilayah asal pelanggan
- Product ID = identitas unik setiap produk
- Category = kategori umum dari setiap produk
- Sub-Category = kategori khusus dari setiap produk
- Product Name = nama setiap produk
- Sales = pendapatan dari setiap pembelian
```

## 🔍 Analysis & Insight
### Mendefinisikan Pertanyaan
1. Bagaimana tren penjualan pada periode 4 tahun tersebut?
2. Bagaimana revenue penjualan pada periode 4 tahun tersebut?
3. Berapa lama total waktu pengemasan barang semenjak barang dipesan?
4. Metode atau jenis pengiriman apa yang paling sering digunakan oleh pelanggan?
5. Jenis segmen pelanggan apa yang paling banyak dan sedikit melakukan pembelian?
6. Persebaran City, State, Region mana yang paling tinggi dan rendah dalam melakukan pembelian?
7. Produk dengan kategori dan sub-category apa yang paling sering dan jarang dibeli oleh pelanggan?
8. Produk apa yang menyumbang revenue tertinggi dan menghasilkan revenue terendah?

### Insight yang Didapat
1. Penjualan menunjukkan tren peningkatan dari tahun 2015 hingga akhir tahun 2018. `Lonjakan tertinggi` penjualan terjadi pada `kuartal keempat di bulan November - Desember` di setiap tahunnya. Walaupun terjadi lonjakan tinggi di kuartal keempat, pada `kuartal pertama di bulan Januari - Februari` mengalami `penurunan` yang signifikan di setiap tahunnya. Namun, jika dilihat secara keseluruhan, tren penjualan ini menunjukkan pertumbuhan yang positif.
2. Secara umum revenue yang dihasilkan mengalami menunjukan tren peningkatan dari tahun 2015 sampai dengan tahun 2018. Tren ini memiliki pola yang hampir sama dengan tren penjualan pada grafik sebelumnya. `Lonjakan revenue` juga terjadi di `kuartal keempat di bulan November-Desember` dan `penurunan tajam` di `kuartal pertama di bulan Januari - Februari` di setiap tahunnya. Walaupun terlihat adanya kenaikan dan penurunan pada musim-musim tertentu, secara keseluruhan tren revenue ini memiliki pertumbuhan yang positif.
3. Waktu pengemasan barang bervariasi dari rentang `0 hari (same day) hingga 7 hari`. Grafik ini juga memperlihatkan total waktu paling tinggi dan rendah pengemasan barang. Terlihat waktu pengemasan barang `paling tinggi` dilakukan dalam waktu `4 hari` dan waktu pengemasan barang `paling rendah` dilakukan dalam waktu `1 hari`.
4. Global Superstore memberikan `4 pilihan metode atau jenis pengiriman`, yaitu Standard Class, Second Class, First Class, dan Same Day. Metode atau jenis pengiriman yang `paling sering digunakan pelanggan` adalah `Standard Class`. Sedangkan yang `paling jarang digunakan pelanggan` adalah `Same Day`.
5. Global Superstore memiliki `tiga segmentasi pelanggan`, yaitu Consumer, Corporate, dan Home Office. Di mana `segment Consumer` menempati `jumlah pelanggan terbanyak`, diikuti dengan `segment Corporate`, dan `paling sedikit` adalah `segmen Home Office`.
6. Global Superstore memiliki persebaran City, State, dan Region sebagai berikut:
   - Persebaran kota dengan `pelanggan tertinggi`, yaitu berasal dari kota `New York City`. Sedangkan untuk kota dengan `pelanggan terendah`, yaitu ada `beberapa kota` seperti `Aberdeen`, `Arlington Heights`, `Arvada`, `Atlantic City`, dan `Yucaipa`
   - Persebaran state dengan `pelanggan tertinggi` adalah `California`, kemudian untuk state dengan `pelanggan terendah` adalah `Wyoming`
   - Persebaran region dibagi kedalam `4 region`, yaitu West, East, Central, dan South. Jika kita ingin membandingkan antara persebaran tertinggi dan terendah, persebaran `pelanggan tertinggi` ada di region `West` dan persebaran `pelanggan terendah` ada di region `South`
7. Global Superstore memiliki beberapa produk, kategori, dan sub-kategori yang paling sering dan jarang dibeli sebagai berikut:
   - Kategori produk yang `paling sering dibeli` oleh pelanggan adalah `Office Suppliers` dan `paling jarang dibeli` oleh pelanggan adalah `Technology`
   - Sub Kategori produk yang `paling sering dibeli` oleh pelanggan adalah `Binders` dan `paling jarang dibeli` oleh pelanggan adalah `Copiers`
   - Kemudian untuk produk yang `paling sering dibeli` oleh pelanggan yaitu `Staple Envelope` dan yang `paling jarang dibeli` oleh pelanggan ada `beberapa produk` diantaranya `Pyle PRT45 Retro Home Telephone`, `Xerox 215`, `Global Enterprise Series Seating Low Back`
8. Produk yang memiliki `revenue produk tertinggi` dihasilkan oleh produk `Canon imageCLASS 2200 Advanced Copier`. Sedangkan untuk `revenue produk terendah` dihasilkan oleh produk `Eureka Disposable Bags`.

📌 Detail proses analisis data terdokumentasi dalam notebook python berikut
[notebook.ipynb](https://github.com/mhmmdridlo/global-superstore/blob/f39e84190b8ca51932563878854bf3c3f19de2c9/notebook.ipynb)

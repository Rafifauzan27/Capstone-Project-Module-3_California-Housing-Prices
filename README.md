# Capstone-Project-Module-3_California-Housing-Prices

## **1. Business Problem Understanding**
---

### **Background**
California adalah negara bagian terpadat di Amerika Serikat dengan populasi lebih dari 39 juta orang. Pertumbuhan populasi yang cepat, terutama di kota-kota besar seperti Los Angeles, San Francisco, dan San Diego, telah mendorong permintaan akan perumahan.  Selain itu, California merupakan salah satu ekonomi terbesar dan paling beragam di dunia. Wilayah ini merupakan pusat teknologi, hiburan, keuangan, dan industri lainnya. Kondisi ekonomi yang kuat, bersama dengan tingkat penghasilan yang tinggi di beberapa daerah, telah menyebabkan harga properti yang tinggi di California.

Dengan keterbatasan lahan yang tersedia dan peraturan pembangunan yang ketat telah membatasi pasokan perumahan di California. Ini telah menyebabkan kenaikan harga properti karena permintaan yang terus meningkat, sementara pasokan perumahan terbatas. Meskipun California memiliki ekonomi yang kuat, ketidaksetaraan sosial dan ekonomi juga menjadi masalah. Harga properti yang tinggi telah menyebabkan kesenjangan antara mereka yang mampu membeli rumah dan mereka yang tidak. Banyak keluarga mengalami kesulitan dalam mencari perumahan yang terjangkau.

Selain California dikenal karena keragaman budaya, etnis, dan demografisnya. Tren demografis, seperti pertumbuhan populasi minoritas yang pesat, juga memengaruhi permintaan dan penawaran perumahan, serta harga properti di berbagai daerah.

### **Problem Statement**
Keterbatasan lahan dan peraturan pembangunan yang ketat di California telah membatasi pasokan perumahan, sementara permintaan terus meningkat karena pertumbuhan populasi yang cepat dan ekonomi yang kuat. Hal ini menyebabkan harga properti yang tinggi, meningkatkan kesenjangan antara mereka yang mampu membeli rumah dan mereka yang tidak. Kondisi ini memperparah ketidaksetaraan sosial dan ekonomi serta menyulitkan banyak keluarga untuk menemukan perumahan yang terjangkau di negara bagian ini. 

Sebagai perusahaan yang bergerak dibidang penjualan properti/rumah, perusahaan ingin mengetahui bagaimana caranya agar dapat menjual propertinya dengan nilai yang optimal untuk penjualan dan membantu keluarga yang ingin membeli rumah dengan harga yang terjangkau.

### **Goals**
Memprediksi harga properti dengan nilai yang optimal untuk penjualan, memungkinkan perusahaan untuk menetapkan harga yang kompetitif dan menguntungkan. Serta, dengan menyediakan informasi yang akurat tentang harga properti, perusahaan dapat membantu mengurangi kesenjangan sosial-ekonomi agar terjangkau bagi semua lapisan masyarakat.

### **Metrics Evaluation**
Metrik evaluasi yang akan digunakan antara lain RMSE (Root Mean Square Error), MAE (Mean Absolute Error), dan MAPE (Mean Absolute Percentage Error), dimana RMSE adalah akar kuadrat dari mean kesalahan kuadrat, MAE adalah mean dari kesalahan absolut, dan MAPE adalah rata-rata persentase kesalahan yang dihasilkan oleh model regresi. Nilai RMSE, MAE, dan MAPE yang lebih kecil menunjukkan bahwa model tersebut lebih akurat dalam memprediksi harga rumah dalam batasan fitur yang digunakan.

Sedangkan Metrics Evaluation yang akan kami gunakan adalah **`MAPE (Mean Absolute Percetage Error)`**, karena :

1. **Interpretasi yang Mudah Dipahami**: MAPE mengukur kesalahan relatif dalam prediksi dengan presentase, sehingga lebih mudah dipahami daripada metrik lainnya seperti MSE (Mean Squared Error) atau RMSE (Root Mean Squared Error).
2. **Respon Terhadap Kesalahan Besar**: MAPE memberikan gambaran yang jelas tentang seberapa besar kesalahan prediksi relatif terhadap nilai sebenarnya. Ini bermanfaat untuk mengetahui seberapa akurat model prediksi, terutama dalam konteks perumahan di mana kesalahan besar dapat memiliki dampak signifikan pada keputusan investasi.
3. **Relevan untuk Tujuan Bisnis**: Dalam industri properti, penting untuk memiliki prediksi yang akurat tentang harga properti untuk mengambil keputusan investasi yang tepat. MAPE membantu dalam mengevaluasi kinerja model prediksi dan meningkatkan keakuratan perkiraan harga properti.


## **2. Data Understanding**
Data ini berisi informasi yang berkaitan dengan detail harga dan kondisi rumah-rumah yang terdapat di beberapa distrik di California dan mencakup beberapa statistik ringkasan tentang kondisi demografis berdasarkan data sensus tahun 1990 di California, USA.

**Attributes Information**

| **Nama Kolom** | **Data Type** | **Deskripsi Singkat** |
| --- | --- | --- |
| longitude | float64 | Koordinat garis bujur daerah perumahan |
| latitude | float64 | Koordinat garis lintang daerah perumahan |
| housing_median_age | float64 | Median Usia Bangunan |
| total_rooms | float64 | Total Ruangan dari keseluruhan Rumah di daerah tersebut|
| total_bedrooms | float64 | Total Kamar Tidur dari keseluruhan Rumah di daerah tersebut|
| population | float64 | Populasi di daerah tersebut |
| households | float64 | Jumlah Rumah Tangga di daerah tersebut|
| median_income | float64 | Median pendapatan penduduk di daerah tersebut dengan satuan sepuluh ribu US Dollar |
| ocean_proximity | object  | Jarak Perumahan dari Laut |
| median_house_value | float64 | Median Harga Rumah dengan satuan US dollar |


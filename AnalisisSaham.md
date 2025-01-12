# ***Analisis Saham Teknologi -AAPL, MSFT, dan GOOGL***

Sektor teknologi merupakan salah satu sektor dengan pertumbuhan tercepat dan berkontribusi besar terhadap ekonomi global. Saham perusahaan seperti  Alphabet Inc. (GOOGL), Microsoft Corp. (MSFT), dan Apple Inc. (AAPL). menjadi fokus utama investor karena inovasi berkelanjutan dan peran strategis mereka dalam transformasi digital. Proyek ini dilatarbelakangi oleh kebutuhan untuk memahami pola pergerakan saham ketiga perusahaan ini, mengevaluasi risiko, serta menentukan potensi keuntungan sebagai dasar pengambilan keputusan investasi.


## Tujuan Analisis
Analisis ini dilakukan dengan tujuan utama sebagai berikut:
1. Menganalisis pola pergerakan harga saham dalam jangka waktu 1 tahun.
2. Mengukur volatilitas masing-masing saham untuk memahami tingkat risiko yang melekat pada setiap saham.
3. Menentukan potensi keuntungan melalui analisis return.
4. Menggunakan model simulasi dan prediksi untuk memproyeksikan pergerakan harga saham di masa depan dan membantu dalam pengambilan keputusan investasi berdasarkan hasil prediksi tersebut.


## Metode Analisis

### a. Pengumpulan Data
Data yang digunakan dalam proyek analisis ini diperoleh dari situs ***Yahoo Finance*** (https://finance.yahoo.com/), yang menyediakan informasi keuangan dan pasar saham secara komprehensif. Data historis yang diambil mencakup harga saham dari perusahaan-perusahaan teknologi terkemuka, seperti Apple Inc. (AAPL), Microsoft Corp. (MSFT), dan Alphabet Inc. (GOOGL). Rentang waktu yang digunakan untuk analisis adalah 1 tahun mulai dari 1 Januari 2024 hingga 1 Januari 2025. 

### b. Pengujian Statistik
Selanjutnya, dilakukan uji statistik yaitu Kolmogorov-Smirnov (KS) dilakukan untuk menguji apakah distribusi return saham mengikuti distribusi normal, dengan menggunakan nilai rata-rata dan standar deviasi yang dihitung sebelumnya. Hasil uji menunjukkan nilai statistik KS sebesar ks_stat dan p-value sebesar ks_p_value. Jika p-value lebih besar dari tingkat signifikansi yang ditetapkan (alpha = 0.05), maka dapat disimpulkan bahwa data return mengikuti distribusi normal (menerima H0). Sebaliknya, jika p-value lebih kecil dari alpha, maka dapat disimpulkan bahwa data return tidak mengikuti distribusi normal (menerima H1).

### c. Simulasi dan Prediksi
Kemudian, Prediksi dilakukan dengan menggunakan metode simulasi Monte Carlo untuk melakukan prediksi harga saham di masa depan. Proses ini melibatkan penambahan noise acak berbasis distribusi normal ke harga saham historis sebagai prediksi.

## Hasil
### Alphabet Inc. (GOOGL)

![grafik saham awal GOOGL](https://github.com/HeraNurKhofifah/Analisis-Saham-Teknologi-AAPL-MSFT-dan-GOOGL/blob/7af3e6517b6891c39425e827f90876971678920a/saham%20awal%20GOOGL.png)

Secara umum, grafik menunjukkan tren naik dalam jangka panjang, yang mengindikasikan bahwa harga saham GOOGL cenderung meningkat seiring berjalannya waktu. Namun, terdapat fluktuasi harga yang cukup signifikan dalam jangka pendek, yang menunjukkan bahwa harga saham GOOGL cukup sensitif terhadap berbagai faktor, seperti berita perusahaan, kondisi pasar secara keseluruhan, dan sentimen investor. Selain itu, grafik juga menunjukkan beberapa puncak (harga tertinggi) dan lembah (harga terendah), yang sering menjadi titik minat bagi para investor karena dapat mengindikasikan potensi perubahan arah tren.


![return GOOGLE](https://github.com/HeraNurKhofifah/Analisis-Saham-Teknologi-AAPL-MSFT-dan-GOOGL/blob/bf4ff40604df31d3d36e62f99aad6f6de912b26d/Return%20GOOGL.png)

Grafik return tersebut menunjukkan fluktuasi yang signifikan, dengan perubahan return yang tajam antara periode satu dengan lainnya. Tidak ada tren yang konsisten, sehingga pergerakan harga cenderung acak, membuat prediksi return di masa depan sulit dilakukan. Fluktuasi tinggi ini mencerminkan volatilitas yang besar, yang berarti saham GOOGL sangat sensitif terhadap faktor eksternal dan dapat mengalami perubahan drastis dalam waktu singkat, membawa potensi keuntungan besar, namun juga risiko yang tinggi.


Kemudian, langkah selanjutnya dilakukan uji statistik berikut:

| Statistik                        | Nilai                               |
|-----------------------------------|-------------------------------------|
| **Mean Return**                   | 0.0013939669442816173              |
| **Standard Deviation of Return**  | 0.012531744671467528              |
| **Variansi Return**               | 0.00015625940138830048            |
| **Kolmogorov-Smirnov Statistic**   | 0.09265470352536748               |
| **P-value**                       | 0.060477680157686065              |


Berdasarkan hasil analisis, dapat dilihat bahwa mean return sebesar 0.0013939669442816173 dan standard deviation of return sebesar 0.012531744671467528. Ini menunjukkan bahwa rata-rata return harian saham cenderung positif dan volatilitasnya relatif rendah. Sementara itu, variansi return tercatat sebesar 0.00015625940138830048, yang menandakan bahwa variasi antara return harian tidak terlalu besar.

Pada tahap berikutnya, dilakukan uji Kolmogorov-Smirnov (KS) untuk menguji apakah distribusi data return sesuai dengan distribusi normal. Hasil uji Kolmogorov-Smirnov menghasilkan statistik KS sebesar 0.09265470352536748, yang menunjukkan seberapa besar perbedaan antara distribusi empiris data dan distribusi normal teoritis. P-value yang diperoleh adalah 0.060477680157686065. Dengan tingkat signifikansi 0.05, karena p-value lebih besar dari 0.05, maka Data return mengikuti distribusi normal (terima H0).

| Harga Saham (Awal) | Return   | Volatilitas | Harga Saham Prediksi | APE (%)  |
|--------------------|----------|-------------|----------------------|----------|
| 137.670929         | 0.000000 | 0.012478    | 137.677127           | 0.004502 |
| 138.418228         | 0.005413 | 0.012478    | 138.416503           | 0.001246 |
| 135.897354         | -0.018380| 0.012478    | 135.905436           | 0.005947 |
| 135.239746         | -0.004851| 0.012478    | 135.258750           | 0.014052 |
| 138.338516         | 0.022655 | 0.012478    | 138.335595           | 0.002112 |
| ...                | ...      | ...         | ...                  | ...      |
| 196.110001         | 0.007575 | 0.012478    | 196.115906           | 0.003011 |
| 195.600006         | -0.002604| 0.012478    | 195.599097           | 0.000465 |
| 192.759995         | -0.014626| 0.012478    | 192.749428           | 0.005481 |
| 191.240005         | -0.007917| 0.012478    | 191.221104           | 0.009884 |
| 189.300003         | -0.010196| 0.012478    | 189.294432           | 0.002943 |

Dari nilai APE yang diperoleh, dilakukan perhitungan MAPE (Mean Absolute Percentage Error) untuk simulasi harga saham, yang menghasilkan nilai sebesar 0.0058. Hal ini menunjukkan bahwa prediksi harga saham memiliki tingkat akurasi yang sangat baik. Dalam periode yang ditampilkan, harga saham GOOGL bervariasi antara harga terendah 130.93 dan harga tertinggi 196.11. Berdasarkan simulasi, diperkirakan harga saham GOOGL akan berada dalam rentang harga minimum 130.91 hingga harga maksimum 196.12. Berikut merupakan grafik dari perbandingan harga saham awal dan harga saham prediksi menggunakan metode simulasi monte carlo.

![grafik perbandingan GOOGL](https://github.com/HeraNurKhofifah/Analisis-Saham-Teknologi-AAPL-MSFT-dan-GOOGL/blob/bf4ff40604df31d3d36e62f99aad6f6de912b26d/Grafik%20Perbandingan%20GOOGL.png)

### Microsoft Corp. (MSFT)

![harga saham MSFT](https://github.com/HeraNurKhofifah/Analisis-Saham-Teknologi-AAPL-MSFT-dan-GOOGL/blob/bf4ff40604df31d3d36e62f99aad6f6de912b26d/saham%20awal%20MSFT.png)

Secara umum, grafik menunjukkan tren naik dalam jangka panjang, yang berarti harga saham MSFT cenderung meningkat seiring berjalannya waktu. Namun, terdapat fluktuasi harga yang cukup signifikan dalam jangka pendek, menunjukkan bahwa harga saham MSFT sensitif terhadap berbagai faktor eksternal, seperti berita perusahaan, kondisi pasar secara keseluruhan, dan sentimen investor. Selain itu, grafik juga memperlihatkan beberapa puncak (harga tertinggi) dan lembah (harga terendah), yang sering menjadi titik perhatian bagi para investor. Puncak dan lembah ini dapat mengindikasikan potensi perubahan arah tren harga saham, yang bisa memberikan peluang bagi investor untuk mengambil keputusan investasi.

![harga saham MSFT](https://github.com/HeraNurKhofifah/Analisis-Saham-Teknologi-AAPL-MSFT-dan-GOOGL/blob/bf4ff40604df31d3d36e62f99aad6f6de912b26d/Return%20MSFT.png)

grafik menunjukkan pergerakan harga saham MSFT yang fluktuatif, dengan perubahan yang signifikan antara periode satu dengan lainnya. Hal ini mencerminkan tingginya fluktuasi harga, di mana harga saham tidak mengikuti tren yang jelas, baik itu tren naik maupun turun. Dengan kata lain, harga saham cenderung bergerak secara acak dari waktu ke waktu. Fluktuasi yang tajam ini juga mengindikasikan volatilitas yang tinggi, yang berarti nilai saham dapat berubah secara drastis dalam waktu yang singkat, baik naik maupun turun, memberikan gambaran tentang ketidakstabilan harga saham MSFT dalam periode yang diamati.

Kemudian, langkah selanjutnya dilakukan uji statistik berikut:

| Statistik                        | Nilai                         |
|------------------------------------|-------------------------------|
| Mean return                        | 0.0021208030199628513         |
| Standard deviation of return       | 0.010013316838437177          |
| Variansi Return                    | 9.984698894330217e-05         |
| Kolmogorov-Smirnov Statistic       | 0.03419031234869374           |
| P-value                            | 0.9335708788936508            |


berdasarkan tabel tersebut, menunjukkan mean return untuk data return saham adalah 0.00212, menunjukkan bahwa rata-rata perubahan harga saham cenderung positif dalam periode yang dianalisis. Standard deviation (deviasi standar) return sebesar 0.010013 menggambarkan seberapa besar fluktuasi harga saham dari rata-rata perubahannya. Variansi return tercatat sebesar 9.98469, yang mengindikasikan seberapa besar penyebaran return di sekitar nilai rata-rata.

Hasil dari uji Kolmogorov-Smirnov menunjukkan statistik sebesar 0.03419, dengan p-value sebesar 0.9335. Karena p-value lebih besar dari tingkat signifikansi ( 0.05), maka tidak ada cukup bukti untuk menolak hipotesis nol (H0), yang berarti data return mengikuti distribusi normal. Dengan demikian, distribusi data return saham dapat dianggap normal berdasarkan uji ini.

| Harga Saham (Awal) | Return   | Volatilitas | Harga Saham Prediksi | APE (%) |
|--------------------|----------|-------------|----------------------|---------|
| 368.117249         | 0.000000 | 0.010013    | 368.122222           | 0.001351 |
| 367.849274         | -0.000728| 0.010013    | 367.847889           | 0.000376 |
| 365.208984         | -0.007204| 0.010013    | 365.215470           | 0.001776 |
| 365.020416         | -0.000516| 0.010013    | 365.035667           | 0.004178 |
| 371.908905         | 0.018696 | 0.010013    | 371.906560           | 0.000630 |
| ...                | ...      | ...         | ...                  | ...     |
| 439.329987         | 0.009330 | 0.010013    | 439.351455           | 0.004887 |
| 438.109985         | -0.002781| 0.010013    | 438.116333           | 0.001449 |
| 430.529999         | -0.017453| 0.010013    | 430.509720           | 0.004710 |
| 424.829987         | -0.013328| 0.010013    | 424.831854           | 0.000439 |
| 421.500000         | -0.007869| 0.010013    | 421.493373           | 0.001572 |


Dari tabel, MAPE (Mean Absolute Percentage Error) yang dihitung adalah 0.0018, menunjukkan bahwa prediksi harga saham memiliki akurasi yang sangat tinggi. Dalam periode yang dianalisis, harga saham bergerak antara harga terendah 365.02 dan harga tertinggi 465.79. Berdasarkan simulasi, harga saham diperkirakan akan berada di kisaran harga minimum 365.04 hingga harga maksimum 465.78.

![grafik perbandingan MSFT](https://github.com/HeraNurKhofifah/Analisis-Saham-Teknologi-AAPL-MSFT-dan-GOOGL/blob/bf4ff40604df31d3d36e62f99aad6f6de912b26d/Grafik%20Perbandingan%20MSFT.png)

### Apple Inc. (AAPL)

![harga saham AAPL](https://github.com/HeraNurKhofifah/Analisis-Saham-Teknologi-AAPL-MSFT-dan-GOOGL/blob/bf4ff40604df31d3d36e62f99aad6f6de912b26d/saham%20awal%20AAPL.png)

Secara umum, grafik harga saham AAPL menunjukkan tren naik dalam jangka panjang, yang mengindikasikan bahwa harga saham cenderung meningkat seiring waktu. Namun, dalam jangka pendek, terlihat adanya fluktuasi harga yang cukup signifikan, yang menunjukkan bahwa saham AAPL sangat sensitif terhadap berbagai faktor eksternal, seperti berita perusahaan, kondisi pasar, dan sentimen investor. Grafik juga memperlihatkan beberapa puncak (harga tertinggi) dan lembah (harga terendah), yang sering kali menjadi titik perhatian bagi investor, karena puncak dan lembah ini dapat menjadi indikasi adanya potensi perubahan arah tren, baik menuju kenaikan maupun penurunan harga saham.

![return AAPL](https://github.com/HeraNurKhofifah/Analisis-Saham-Teknologi-AAPL-MSFT-dan-GOOGL/blob/c732fafc3579861ec7de9311d41ca5ca4b7bea10/return%20AAPL.png)

Grafik menunjukkan fluktuasi harga saham Apple Inc. (AAPL) yang tinggi, dengan garis merah yang menggambarkan pengembalian saham dari waktu ke waktu. Tidak ada tren jelas dalam jangka panjang, yang menunjukkan pergerakan harga yang cenderung acak. Tingginya volatilitas menandakan risiko besar bagi investor, karena harga bisa berubah drastis dalam waktu singkat. Namun, volatilitas ini juga membuka peluang untuk keuntungan besar jika harga saham meningkat tajam.

Kemudian, langkah selanjutnya dilakukan uji statistik berikut:

| Statistik                  | Nilai                         |
|---------------------------------|-------------------------------|
| Mean Return                    | 0.0012484082578907661         |
| Standard Deviation of Return   | 0.010959184968229485          |
| Variansi Return                | 0.000119603302938001          |
| Kolmogorov-Smirnov Statistic   | 0.03381951795173305           |
| P-value                        | 0.9378038670503854            |

berdasarkan tabel tersebut, menunjukkan mean return untuk data return saham adalah 0.00125, menunjukkan bahwa rata-rata perubahan harga saham cenderung positif dalam periode yang dianalisis. Standard deviation (deviasi standar) return sebesar 0.01096 menggambarkan seberapa besar fluktuasi harga saham dari rata-rata perubahannya. Variansi return tercatat sebesar 0.00012, yang mengindikasikan seberapa besar penyebaran return di sekitar nilai rata-rata.

Hasil dari uji Kolmogorov-Smirnov menunjukkan statistik sebesar 0.03382, dengan p-value sebesar 0.9378. Karena p-value lebih besar dari tingkat signifikansi ( 0.05), maka tidak ada cukup bukti untuk menolak hipotesis nol (H0), yang berarti data return mengikuti distribusi normal. Dengan demikian, distribusi data return saham dapat dianggap normal berdasarkan uji ini.

| Harga Saham (Awal) | Return   | Volatilitas | Harga Saham Prediksi | APE (%)  |
|--------------------|----------|-------------|----------------------|----------|
| 184.734985         | 0.000000 | 0.010959    | 184.740429           | 0.002947 |
| 183.351761         | -0.007516| 0.010959    | 183.350246           | 0.000826 |
| 181.023178         | -0.012781| 0.010959    | 181.030276           | 0.003921 |
| 180.296707         | -0.004021| 0.010959    | 180.313398           | 0.009258 |
| 184.655365         | 0.023887 | 0.010959    | 184.652799           | 0.001390 |
| ...                | ...      | ...         | ...                  | ...      |
| 258.200012         | 0.011413 | 0.010959    | 258.206959           | 0.002691 |
| 259.019989         | 0.003171 | 0.010959    | 258.997795           | 0.008568 |
| 255.589996         | -0.013331| 0.010959    | 255.592040           | 0.000799 |
| 252.199997         | -0.013352| 0.010959    | 252.192744           | 0.002876 |
| 250.419998         | -0.007083| 0.010959    | 250.429340           | 0.003731 |

Dari tabel, MAPE (Mean Absolute Percentage Error) yang dihitung untuk simulasi harga saham adalah 0.0041, yang menunjukkan bahwa prediksi harga saham memiliki tingkat akurasi yang sangat baik. Dalam periode yang dianalisis, harga saham bervariasi antara harga terendah 164.41 dan harga tertinggi 259.02. Berdasarkan hasil simulasi, harga saham diperkirakan akan berada dalam rentang harga minimum 164.42 hingga harga maksimum 259.00.Berikut merupakan grafik dari perbandingan harga saham awal dan harga saham prediksi menggunakan metode simulasi monte carlo.
![Grafik perbandingan AAPL](https://github.com/HeraNurKhofifah/Analisis-Saham-Teknologi-AAPL-MSFT-dan-GOOGL/blob/bf4ff40604df31d3d36e62f99aad6f6de912b26d/Grafik%20perbandingan%20AAPL.png)


## Kesimpulan
Berdasarkan hasil analisis terhadap tiga perusahaan teknologi besar, yaitu Alphabet Inc. (GOOGL), Microsoft Corp. (MSFT), dan Apple Inc. (AAPL), terdapat beberapa kesimpulan yang dapat diambil. Ketiga saham secara umum menunjukkan tren kenaikan harga dalam jangka panjang, yang mencerminkan kinerja positif dari masing-masing perusahaan selama periode analisis. Namun, fluktuasi jangka pendek pada semua saham cukup signifikan, menunjukkan sensitivitas terhadap faktor eksternal seperti berita perusahaan, kondisi pasar global, dan sentimen investor.

Return saham untuk ketiga perusahaan ini bervariasi. GOOGL memiliki mean return sebesar 0.00139, sementara MSFT dan AAPL masing-masing mencatatkan mean return sebesar 0.00212 dan 0.00125. Rata-rata perubahan harga saham cenderung positif, meskipun tingkat pengembaliannya berbeda-beda. Dari segi volatilitas, saham GOOGL memiliki volatilitas tertinggi dengan deviasi standar 0.01253, dibandingkan dengan MSFT (0.01001) dan AAPL (0.01096), yang menunjukkan bahwa GOOGL memiliki risiko lebih besar.

Hasil uji Kolmogorov-Smirnov menunjukkan bahwa data return untuk ketiga saham mengikuti distribusi normal, dengan p-value lebih besar dari 0.05 pada masing-masing saham. Hal ini terkonfirmasi dari p-value GOOGL sebesar 0.060, MSFT sebesar 0.933, dan AAPL sebesar 0.938. Normalitas data ini mendukung penggunaan metode statistik berbasis distribusi normal untuk analisis lanjutan. 

Prediksi harga saham menggunakan simulasi Monte Carlo menunjukkan tingkat akurasi yang sangat tinggi, seperti yang tercermin dari nilai Mean Absolute Percentage Error (MAPE). GOOGL memiliki MAPE sebesar 0.0058 (0.58%), MSFT sebesar 0.0018 (0.18%), dan AAPL sebesar 0.0041 (0.41%). Akurasi prediksi ini membuktikan bahwa metode simulasi Monte Carlo dapat memodelkan pergerakan harga saham dengan sangat baik. Rentang harga saham yang diperkirakan melalui simulasi menunjukkan bahwa harga GOOGL berada pada kisaran $130.91 hingga $196.12, MSFT pada kisaran $365.04 hingga $465.78, dan AAPL pada kisaran $164.42 hingga $259.00.

Dari segi risiko dan potensi keuntungan, GOOGL dengan volatilitas tertinggi menawarkan risiko sekaligus potensi keuntungan terbesar dalam jangka pendek, cocok bagi investor dengan profil risiko tinggi. MSFT, yang memiliki volatilitas terendah, lebih stabil dan cocok untuk investor konservatif yang mengutamakan kestabilan. Sementara itu, AAPL menunjukkan karakteristik yang moderat, menjadikannya pilihan yang seimbang bagi investor dengan toleransi risiko menengah. Secara keseluruhan, ketiga saham menunjukkan kinerja positif dengan prediksi harga yang mendekati akurasi sempurna, memungkinkan investor untuk memilih saham sesuai dengan profil risiko masing-masing.

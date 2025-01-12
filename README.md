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



Secara umum, grafik menunjukkan tren naik dalam jangka panjang. Artinya, harga saham GOOGL cenderung meningkat dari waktu ke waktu.
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

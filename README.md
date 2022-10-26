# Home Credit Scorecard Model
Project by Muhammad Farras Rizki

# A. Latar Belakang
Dataframe yang digunakan milik Home Credit Indonesia. Manajemen Home Credit Indonesia ingin membuat membuat prediksi skor kredit. Dengan tujuan, dapat memastikan pelanggan yang mampu melakukan pelunasan tidak ditolak ketika melakukan pengajuan pinjaman, dan pinjaman datap diberikan dengan principal, maturity, dan repayment calendar yang akan memotivsi pelanggan untuk sukses.

# B. Tentang Dataframe
Dataframe application_train berisikan 307511 baris yang merupakan ID transaksi peminjaman pelanggan yang telah terlaksana, baik yang berhasil maupun yang gagal. Data tersebut meliputi informasi demografis pelanggan (umur, pendapatan, dll), hubungan nasabah dengan bank (hipotek, rekening, surat berharga, dll), dan status akhir hasil pengajuan pinjaman nasabah (TARGET). Di antara 307511 nasabah ini, terdapat 24000 pelanggan (8%) yang mengalami gagal bayar.

# C. Tujuan Proyek
Membuat Model Machine Learning yang dapat memberikan sebuah score kelayakan pada client dalam memperoleh pinjaman.

# D. Sumber Dataset
Sumber: https://rakamin-lms.s3.ap-southeast-1.amazonaws.com/vix-assets/home-credit-indonesia/home-credit-default-risk.zip

# E. Deskripsi Singkat Pemodelan
Tujuan dari pemodelan adalah ingin membuat model yang mampu memprediksi skor kredit seorang pelanggan, agar dapat memastikan pelanggan yang mampu melakukan pelunasan tidak ditolak ketika melakukan pengajuan pinjaman. Target Variabel yang akan digunakan adalah TARGET (status akhir hasil pengajuan pinjaman nasabah sebelumnya). Variabel yang paling diinginkan untuk optimal adalah F1-score karena ingin meminimalisir false positive maupun false negative.

Prediksi / Hipotesis yang dibuat berdasarkan target variabel :

0: Pelanggan mampu melakukan pelunasan (Positive)
1: Pelanggan tidak mampu melakukan pelunasan (Negative)
False Positive: Diprediksi pelanggan mampu mampu melakukan pelunasan, Namun aktualnya pelanggan tidak mampu melakukan pelunasan
False Negative: Diprediksi pelanggan tidak mampu melakukan pelunasan, Namun aktualnya pelanggan mampu melakukan pelunasan

Model Machine Learning yang akan diuji antara lain:
1. Logical Regression
2. K-NN
3. Naive Bayes
4. Decision Tree Classification

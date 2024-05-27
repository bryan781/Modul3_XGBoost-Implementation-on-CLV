# Modul3_XGBoost-Implementation-on-CLV


# 1. Business Understanding

Customer Lifetime Value adalah salah satu metrik yang mengukur total pendapatan dari seorang pelanggan selama rentang waktu tertentu. CLV membandingkan pendapatan dari setiap pelanggan dengan customer lifespan, atau sudah berapa lama orang tersebut menjadi pelanggan di suatu bisnis. metrik CLV banyak digunakan oleh perusahaan yang melakukan repeat sales kepada customer maupun perusahaan yang menggunakan sistem berlangganan dalam bisnisnya.

## 1.1 Problem 

Dalam data ini, suatu perusahaan asuransi mobil di Amerika Serikat mengalami masalah dalam meningkatkan revenue perusahaan. Salah satu penyebabnya adalah karena pendekatan strategi marketing yang tidak tepat dimana perusahaan mengeluarkan budget yang sama untuk seluruh tipe customer, sehingga perusahaan akhirnya membayar lebih untuk low-value customer dan kehilangan high-value customer. Maka dari itu, perusahaan menggunakan metrik CLV agar dapat menentukan seberapa valuable customer yang dimiliki dan strategi marketing yang akan digunakan berdasarkan CLV tersebut. Namun perusahaan asuransi mobil ini belum memiliki sistem untuk memprediksi CLV dengan cepat dan akurat sehingga penentuan strategi marketing saat ini memakan waktu lebih lama karena pengolahan data yang masih secara manual. Oleh karena itu, prediksi CLV yang lebih cepat dan akurat sangatlah penting untuk dapat mengambil strategi marketing yang lebih tepat.

## 1.2 Analysis Goal

Berdasarkan permasalahan diatas, tujuan utama dari analisa ini adalah mempermudah perusahaan asuransi mobil (khususnya divisi marketing) apabila terdapat 'tools' untuk memprediksi CLV dengan melihat dari data demografis dan data asuransi mobil customer (tipe asuransi, jumlah polis, biaya premi, total klaim, dan lainnya) sehingga pengolahan data CLV tidak lagi secara manual dan dapat mempercepat proses pengambilan keputusan strategi marketing.

## 1.3 Metric Used

Metrik yang akan digunakan adalah RMSE, MAE, dan MAPE, di mana RMSE adalah nilai rataan akar kuadrat dari error, MAE adalah rataan nilai absolut dari error, sedangkan MAPE adalah rataan persentase error yang dihasilkan oleh model regresi. Semakin kecil nilai RMSE, MAE, dan MAPE yang dihasilkan, berarti model semakin akurat dalam memprediksi CLV sesuai dengan limitasi feature yang digunakan. Akan tetapi pada hasil analisa model, akan berfokus pada RMSE

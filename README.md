
# Problems

Home Credit Indonesia bertujuan membangun model machine learning yang dapat membantu tim dalam memprediksi apakah pengajuan pinjaman dari pelanggan akan menghadapi kesulitan dalam pembayaran kredit atau tidak. Dengan menganalisis data yang tersedia, Home Credit Indonesia berupaya untuk mengidentifikasi karakteristik pelanggan yang cenderung lancar dalam proses pembayaran kredit, sehingga dapat memberikan kontribusi positif terhadap peningkatan pendapatan perusahaan.

## Business Insight
![image](https://github.com/nellyyuliaa/model-hci/assets/122393200/229032b8-f16e-4e1b-b68a-448861e1ed12)
Contract Type (Jenis Kontrak)-(1)
Dalam Revolving Loans contract, terdapat 4 jenis pendapatan utama yang tidak mengalami kesulitan dalam membayar pinjaman, yaitu Businessman, Maternity Leave, Student, dan Unemployed. Namun, jumlah pelanggan yang berasal dari ke-4 jenis pendapatan ini relatif sedikit. Oleh karena itu, diperlukan upaya untuk meningkatkan jumlah pelanggan yang memiliki sumber pendapatan dari salah satu dari empat jenis pendapatan utama tersebut.

Contract Type (Jenis Kontrak)-(2)
![image](https://github.com/nellyyuliaa/model-hci/assets/122393200/71523769-ca1f-4032-98bd-d89677912211)
Dalam Cash Loans contract, Maternity Leave adalah satu-satunya yang memiliki tingkat yang mencapai 100%. Oleh karena itu, kami menyarankan agar klien yang sedang Maternity Leave mempertimbangkan untuk mengajukan pinjaman jenis bergulir, karena pada jenis pinjaman tersebut, klien yang sedang Maternity Leave memiliki tingkat pelanggan yang mencapai 100% dan tidak mengalami kesulitan dalam melunasi pinjaman.

Occupation Type of Customer
![image](https://github.com/nellyyuliaa/model-hci/assets/122393200/f4b04140-2528-4c75-9cf3-5d9f78d3b168)
Pekerjaan yang paling umum di antara pelanggan adalah profesi Accountant, oleh karena itu, kami harus merencanakan sebuah kampanye sebagai tanda terima kasih kepada mereka. Namun, kami juga perlu mempertimbangkan untuk mempromosikan pekerjaan lain dalam grafik, karena persentase pelanggan yang tidak mengalami masalah dalam membayar pinjaman cukup tinggi. Meskipun begitu, jumlah pelanggan dari 3 pekerjaan tersebut masih relatif kecil.

## Machine Learning Model 
Data Preparation:
1. Make a new column (age)
2. Feature selection
3. Remove Outlier
4. Feature Encoding (One hot encoding and label encoding)
5. Feature Transformation

Handling imbalance Data:
1. Oversampling
2. Undersampling

Train Machine Learning Model:
1. Logistic Regression
2. XGBoost
3. Random Forest
4. Desicion Tree

## Result
![Screenshot 2024-04-01 032459](https://github.com/nellyyuliaa/model-hci/assets/122393200/06832aff-f231-46f4-98aa-0190f192cb48)
Dari beberapa model tersebut, Random Forest menonjol sebagai yang terbaik dengan tingkat akurasi, presisi, dan recall yang lebih tinggi dibandingkan dengan model lainnya. Random Forest menjadi pilihan terbaik dari segi akurasi dan prediksi. Meskipun XGBoost memiliki akurasi yang tinggi (95%), Random Forest memiliki akurasi yang sama (96%) namun memiliki prediksi yang lebih baik (100%), menunjukkan kemampuan superior dalam mengklasifikasikan data.

## Summary
1. Dalam Revolving Loans Contract, perlu ditemukan pelanggan dengan berbagai jenis pendapatan seperti Businessmen, Maternity Leave, Students dan Unemployed.
2. Disarankan untuk menginisiasi kampanye khusus bagi pelanggan yang bekerja sebagai Akuntan karena profesi tersebut memiliki jumlah pelanggan terbanyak dan tingkat keberhasilan pembayaran yang tinggi.
3. Pengembangan iklan atau promosi yang ditargetkan kepada staf HR, staf IT, dan agen properti untuk meningkatkan aplikasi kredit.
4. Model Machine Learning yang dipilih adalah Random Forest. Meskipun XGBoost memiliki akurasi yang tinggi (95%), Random Forest memiliki akurasi yang sama (96%) tetapi memiliki prediksi yang lebih baik (100%), menunjukkan kemampuan superior dalam mengklasifikasikan data. Decision Tree memiliki akurasi 91% dan prediksi sempurna (100%), tetapi lebih rendah daripada XGBoost dan Random Forest yang memiliki akurasi lebih tinggi. Meskipun prediksi sempurna, akurasi yang rendah menunjukkan bahwa model tersebut mungkin tidak dapat memahami pola yang kompleks dengan baik seperti XGBoost dan Random Forest. Dengan akurasi yang lebih rendah, Decision Tree tidak seunggul XGBoost dan Random Forest. 

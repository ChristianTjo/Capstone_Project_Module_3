# Capstone_Project_Module_3
## **Mengoptimalkan Harga Apartemen di Area Daegu - Korea Selatan, menggunakan Analisis Machine Learning**

# **1. Business Problem Understanding**

**Context**

Daegu adalah kota terbesar keempat di Korea Selatan dan wilayah metropolitan terbesar ketiga. Kota ini terletak di bagian tenggara negara tersebut, di wilayah Yeongnam.
Daegu adalah aglomerasi perkotaan terbesar ketiga di Korea Selatan setelah Seoul dan Busan; kota metropolitan terbesar keempat di negara ini dengan lebih dari 2,3 juta penduduk.
Daegu dan Provinsi Gyeongsang Utara di sekitarnya sering disebut sebagai Daegu-Gyeongbuk, dengan total populasi lebih dari 5 juta.

Tingkat hunian apartemen di Daegu cukup bervariasi, tetapi secara umum, apartemen di Daegu memiliki beberapa tingkat, seperti 10-15 lantai, dan beberapa apartemen bahkan bisa mencapai 30-50 lantai. Selain itu, apartemen di Daegu juga menawarkan berbagai tipe unit, mulai dari unit kecil hingga unit yang lebih besar atau mewah seperti penthouse. 

Dengan keterbatasan lahan untuk perumahan dan tingginya harga rumah di Daegu,maka apartement adalah salah satu alternatif hunian yang sangat menarik untuk dimiliki,hal ini karena dekat dengan pusat kota juga merupakan tempat tinggal yang nyaman.

**Problem Statement**

Problem utama terkait apartemen Daegu ini adalah terkait menentukan harga jual dari apartemen itu sendiri.penetapan harga jual yang tepat menjadi hal yang
sangat penting,karena harga yang terlalu tinggi dapat menghambat proses penjualan. Sementara harga yang terlalu rendah dapat mengurangi potensi keuntungan.
Ketepatan dalam menetapkan harga sangat penting untuk menjaga keseimbangan antara keuntungan dan daya tarik pasar.
Akan tetapi untuk menetapkan harga ini terdapat banyak faktor yang mempengaruhi seperti lokasi pembangunan apartemen,nilai tanah,dekat dengan fasilitas publik,
dengan dengan area yang populer seperti pusat perbelanjaan dan hiburan serta faktor - faktor lainnya.

**Goals**

Berdasarkan hal tersebut,maka sangat diperlukan pengembangan model prediktif yang dapat memperkirakan harga jual unit apartemen yang ada di Daegu sesuai dengan
karakteristiknya(luas tanah,jarak ke stasiin,dsb.).
Model ini diharapkan dapat membantu para pemangku kepentingan dalam membuat keputusan yang tepat terkait harga, investasi, dan pengembangan properti.

**Analytic Approach**

Oleh sebab itu,hal yang perlu dilakukan adalah menganalis data untuk menemukan pola dari data yang tersedia.Karena target penelitian ini adalah **harga apartemen yang kontinu secara numerik,maka pendekatan analisis yang akan digunakan adalah Model Regresi.
Model ini akan menggunakan data-data apartemen sebagai prediktor untuk memperkirakan harga jual.
Sehingga pada akhirnya akan membantu pemilik apartemen dalam memnbuat keputusan yang terbaik.

**Metric Evaluation**

Evaluasi metrik yang akan digunakan adalah RMSE, MAE, dan MAPE, di mana RMSE adalah nilai rataan akar kuadrat dari error, MAE adalah rataan nilai absolut dari error, sedangkan MAPE adalah rataan persentase error yang dihasilkan oleh model regresi. Semakin kecil nilai RMSE, MAE, dan MAPE yang dihasilkan, berarti model semakin akurat dalam memprediksi harga apartemen yang sesuai dengan limitasi fitur yang digunakan.

Selain itu, kita juga bisa menggunakan nilai R-squared atau adj. R-squared jika model yang nanti terpilih sebagai final model adalah model linear. Nilai R-squared digunakan untuk mengetahui seberapa baik model dapat merepresentasikan varians keseluruhan data. Semakin mendekati 1, maka semakin fit pula modelnya terhadap data observasi. Namun, metrik ini tidak valid untuk model non-linear.

**Limitation**

- Model ini hanya dapat memprediksi harga apartemen di kota Daegu, dan tidak dapat digunakan sebagai tolok ukur harga di area lain.
- Model ini hanya menggunakan data pada satu waktu tertentu, tidak dapat meramalkan harga di masa mendatang, karena dapat terjadi perubahan tren di masa
  mendatang.
- Model ini hanya mempertimbangkan fitur-fitur dalam kumpulan data dan tidak dapat menangkap fenomena di luar fitur yang ada,terutama faktor sosial,budaya,dan
  pemerintahan.


# **2. Data Understanding**

- Dataset ini berisi data apartemen di kota Daegu yang di bangun dalam rentang waktu tahun 1978 s/d 2015
- Dataset ini merupakan data list Apartemen di kota Daegu (Korea Selatan) dan setiap barisnya terdiri dari karakteristik(harga jual, fasilitas, tahun dibuat,
  dsb.

**Attributes Information**

| No. | Column | Description | Data Type |
|----|-------------------------|-----------------------------------------------------------------------------------------------------|-------------|
| 1 | HallwayType | The type of hallway in the property, indicating the interior design or layout. | Categorical |
| 2 | TimeToSubway | Time required to reach the nearest railway station. | Categorical |
| 3 | SubwayStation | Name of the nearest train station. | Categorical |
| 4 | N_FacilitiesNearBy(ETC) | Number of additional facilities near the property (e.g. parks, shopping centers). | Numerical |
| 5 | N_FacilitiesNearBy(PublicOffice) | Number of public office facilities around the property. | Numerical |
| 6 | N_SchoolNearBy(University) | Number of universities near the property. | Numerical |
| 7 | N_Parkinglot(Basement) | Number of parking spaces in the basement of the property. | Numerical |
| 8 | YearBuilt | Year of property construction. | Numerical |
| 9 | N_FacilitiesInApt | Number of facilities available in the apartment. | Numerical |
| 10 | Size(sqf) | Property size in square feet. | Numerical |
| 11 | SalePrice | Property sale price. | Numerical |


# **3. EDA (Exploratory Data Analysis)**
Dalam Exploratpry Data Analysis akan di uraikan lebih lanjut terkait :
- **Data Distribution**
- **Data Correlation**


# **4. Data Preparation**

Untuk dapat membuat keputusan yang lebih baik dan lebih tepat,maka perlu dilakukan oembersihan data seperti jika ada **Missing Value,Duplicate,
Outliers**,sehingga nantinya dapat dipakai untuk analisa lebih lanjut.


# **5. Modeling & Evaluation**

Pada tahap ini akan dilakukan MOdeling & Evaluation, untuk kemudian dipilih model terbaik ( paling cocok ) untuk meprediksi nilai target


# *6. Conclusion and Recommendations**

Berisi Conclusion ( kesimpulan ) dan Recomendations ( rekomendasi )




















# BigData
Tugas Minggu 4 
# Chapter 3 
Deep Dive Into Apache Spark
<h1>Scala</h1>
<h2>1.System Commands Output </h2>
<h3>code</h3>
https://github.com/AryoBags/BigData/blob/1fdbc2e07dd6b2134a00f69e49a0245e4e2d45a1/SystemCommandsOutput.scala#L1-L3
<h3>hasil</h3>
<img src="https://github.com/AryoBags/BigData/blob/81270d7f39d36e2846e87ea414c5c8aaf3cd4fdf/image.png">
<h2> 2. System Commands Return Code </h2>
<h3>code</h3>
https://github.com/AryoBags/BigData/blob/81270d7f39d36e2846e87ea414c5c8aaf3cd4fdf/SystemCommandsReturnCode.scala#L1-L3
<h3>Hasil</h3>
<image src="https://github.com/AryoBags/BigData/blob/076ca4eb6b3d49b2feaac798d23e712d94726436/image.png">

<h1>Python</h1>
<h2> 1. Accumulator </h2>
<h3>code</h3>
https://github.com/AryoBags/BigData/blob/076ca4eb6b3d49b2feaac798d23e712d94726436/Accumulator.py#L1-L4
<h3>hasil</h3>
<image src = "https://github.com/AryoBags/BigData/blob/e04c4bbd1337bf0fcacafeb1a5a7f9d4574f6738/image.png">
<h3>Penjelasan</h3>
1. sc : berguna untuk membuat suatu object dari spark context.

2. accumulator : suatu variabel yang hanya bisa ditambahkan dengan operasi matematika yang memiliki sifat asosiatif dan komutatif (penjumlahan, pengurangan, perkalian, dan pembagian)

3. parallelize : metode pada spark context yang digunakan untuk membuat sebuah kumpulan data yang terdistribusi.

4. lambda : digunakan untuk melakukan pemetaan data atau transformasi data pada RDD (Resilient Distributed Dataset).

5. value : sebuah variabel yang menyimpan suatu nilai atau objek yang digunakan dalam proses pemrosesan data.

<h2> 2.BroadCast </h2>
<h3>code</h3>
https://github.com/AryoBags/BigData/blob/e04c4bbd1337bf0fcacafeb1a5a7f9d4574f6738/BroadCast.py#L1-L2
<h3>Hasil</h3>
<image src="https://github.com/AryoBags/BigData/blob/21fde8d45f961738452a0728b72eadc60ba298af/image.png">
<h3>Penjelasan</h3>
1. broadcast : suatu fitur yang digunakan untuk mendistribusikan variabel secara efisien ke seluruh node dalam cluster.

2. list : salah satu jenis struktur data yang digunakan untuk menyimpan kumpulan elemen atau nilai.

3. range : salah satu struktur data yang digunakan untuk menyimpan kumpulan nilai atau elemen yang terdiri dari serangkaian nilai berturut-turut

<h2> 3.Log Analytics </h2>
<h3>code</h3>
https://github.com/AryoBags/BigData/blob/dc901f0e3c2eb4426c6548d5c2b2f9050f597297/LogAnalytics.py#L1-L27
<h3>Hasil</h3>
<image src="https://github.com/AryoBags/BigData/blob/dc901f0e3c2eb4426c6548d5c2b2f9050f597297/image.png">
<h3>Penjelasan</h3>

1. textFile : alah satu metode untuk membaca data dari file teks pada sistem file distribusi Hadoop. Metode ini digunakan untuk membaca file teks dalam format yang umum digunakan seperti CSV, TSV, JSON, XML, dan lainnya.

2. filter : operasi transformasi yang digunakan untuk memfilter RDD (Resilient Distributed Dataset) berdasarkan kriteria tertentu.
3. cache : operasi yang digunakan untuk menyimpan RDD (Resilient Distributed Dataset) di memori pada setiap node dalam cluster.
4. count : operasi yang digunakan untuk menghitung jumlah elemen pada RDD (Resilient Distributed Dataset) yang diberikan.

<h2> 4. Pair RDD</h2>
<h3>code</h3>
https://github.com/AryoBags/BigData/blob/dc901f0e3c2eb4426c6548d5c2b2f9050f597297/PairRDD.py#L1-L11
<h3>Hasil</h3>
<image src="https://github.com/AryoBags/BigData/blob/061f63f4465c8ab5fa1ebc02dd86d426b76c160c/Pair%20RDD.png">
<h3>Penjelasan</h3>

1. map : operasi yang digunakan untuk mengubah setiap elemen dalam RDD (Resilient Distributed Dataset) menjadi nilai baru dengan menggunakan sebuah fungsi tertentu.
2. collect : operasi yang digunakan untuk mengumpulkan seluruh elemen dari RDD (Resilient Distributed Dataset) dan mengembalikannya sebagai sebuah array pada driver program.
3. len : digunakan untuk menghitung jumlah elemen dalam sebuah list atau array.
4. keys : metode pada tipe data Map yang digunakan untuk mengembalikan semua kunci (key) yang ada dalam Map tersebut.
5. values : digunakan untuk mengembalikan semua nilai (value) yang ada dalam Map tersebut.

<h2> 5.Understanding RDDs </h2>
<h3>code</h3>
https://github.com/AryoBags/BigData/blob/061f63f4465c8ab5fa1ebc02dd86d426b76c160c/UnderstandingRDDs.py#L1-L40
<h3>Hasil</h3>
<image src="https://github.com/AryoBags/BigData/blob/061f63f4465c8ab5fa1ebc02dd86d426b76c160c/Undersatnding%20RDDs.png">
<h3>Penjelasan</h3>

1. defaultParallelism :suatu konfigurasi yang ditentukan oleh SparkContext saat pertama kali diinisialisasi.
2. getNumPartitions : digunakan untuk mengembalikan jumlah partisi (partition) pada sebuah RDD.
3. mapPartitionsWithIndex : digunakan untuk melakukan transformasi data pada setiap partisi RDD dengan mempertahankan indeks partisi. Metode ini mirip dengan mapPartitions tapi dengan adanya argumen indeks partisi pada setiap pemanggilan fungsi transformasi.
4. repartition : digunakan untuk mengubah jumlah partisi RDD menjadi jumlah yang baru tanpa mengubah nilai-nilai pada RDD.
5. coalesce :digunakan untuk mengurangi jumlah partisi RDD menjadi jumlah yang baru tanpa melakukan shuffle data secara besar-besaran.
6. toDebugString : digunakan untuk mencetak informasi debug terkait partisi RDD, seperti lokasi partisi, ukuran partisi.
<h2> 6.WOrd Count </h2>
<h3>code</h3>
https://github.com/AryoBags/BigData/blob/061f63f4465c8ab5fa1ebc02dd86d426b76c160c/WordCount.py#L1-L8
<h3>Hasil</h3>
<image src="https://github.com/AryoBags/BigData/blob/061f63f4465c8ab5fa1ebc02dd86d426b76c160c/Word%20Count.png">
<h3>Penjelasam </h3>

1. flatMap : digunakan untuk mentransformasi sebuah RDD dengan mengaplikasikan sebuah fungsi ke setiap elemen RDD, kemudian mengembalikan nol atau banyak output untuk setiap elemen input.
2. reduceByKey : digunakan untuk melakukan agregasi pada pasangan key-value.
3. split : digunakan untuk memisahkan sebuah string menjadi sebuah array of string dengan memanfaatkan sebuah pemisah yang ditentukan.



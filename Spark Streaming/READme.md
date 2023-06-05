# BigData
Tugas Minggu 12
# Spark Streaming
<h2>1. network__wordcount </h2>
<h3>code</h3>
https://github.com/AryoBags/BigData/blob/b9a55adf34dc8304aa7a81d2307293d32b521aa8/Spark%20Streaming/network_wordcount.py#L29-L50 
<h3>hasil</h3>

![image](https://github.com/AryoBags/BigData/assets/95728907/f6e12840-caaa-49f5-a88f-ed9b29d41d13)

![image](https://github.com/AryoBags/BigData/assets/95728907/4f4ffe61-8a37-47b0-aad9-6ffe5df5af03)

<h2>2. Stateful_network_wordcount.pyt </h2>
<h3>code</h3>
https://github.com/AryoBags/BigData/blob/b9a55adf34dc8304aa7a81d2307293d32b521aa8/Spark%20Streaming/stateful_network_wordcount.py#L33-L62
<h3>hasil</h3>

![image](https://github.com/AryoBags/BigData/assets/95728907/e429ba17-af47-4a85-9541-f772609be197)

![image](https://github.com/AryoBags/BigData/assets/95728907/f9f2561b-65a8-49a9-940b-d5e78a3ba516)

<h2>3. transformasi_word_sentiment </h2>
<h3>code</h3>
https://github.com/AryoBags/BigData/blob/b9a55adf34dc8304aa7a81d2307293d32b521aa8/Spark%20Streaming/tws.py#L1-L46



<h2>Tugas </h2>

Silakan selesaikan praktikum tersebut sesuai langkah-langkah sebelumnya, lalu laporkan hasilnya berupa link repository GitHub dengan nama spark-streaming disertai dengan screenshot hasilnya.
Jelaskan perbedaan spark streaming dengan metode stateless dan stateful stream processing ?
Jelaskan masing-masing maksud kode berikut sesuai nomor kodenya pada laporan praktikum Anda!
Nomor Kode

Sintaks

1 sys.argv, sys.stderr, StreamingContext, sc, socketTextStream, reduceByKey, lambda line, awaitTermination

2 nc, lk

3 spark-submit, master, local[*]

4 ssc.checkpoint, parallelize, updateStateByKey, flatMap

5 rdd.take(5), transform, rdd.sortByKey(False)

<h2>Jawab </h2>

1.    - sys.argv: Variabel yang berisi argumen baris perintah saat menjalankan skrip Python.
      - sys.stderr: Saluran standar untuk output kesalahan.
      - StreamingContext: Konteks inti dalam Spark Streaming untuk pemrosesan streaming.
      - sc: SparkContext untuk berinteraksi dengan kluster Spark.
      - socketTextStream: Membuat DStream dari data yang diterima melalui socket.
      - reduceByKey: Menggabungkan nilai-nilai dengan kunci yang sama dalam RDD menggunakan fungsi pengurangan.
      - lambda line: Fungsi anonim dengan satu parameter line.
      - awaitTermination: Meminta StreamingContext agar tetap berjalan hingga pemrosesan streaming selesai.
   
2. - nc, lk: Utilitas netcat untuk membuka koneksi dan mengirim/menerima data melalui jaringan.
3. - spark-submit: Perintah untuk mengirimkan aplikasi Spark ke kluster Spark untuk dieksekusi.
   - master: Argumen untuk menentukan alamat URL atau mode eksekusi kluster Spark.
   - local[*]: Mode eksekusi Spark lokal dengan menggunakan semua core yang tersedia pada mesin.

4. - ssc.checkpoint: Mengatur tempat penyimpanan sementara (checkpoint) untuk operasi pemrosesan streaming stateful.
   - parallelize: Membuat RDD dari koleksi data yang ada di memori dalam bentuk array.
   - updateStateByKey: Memperbarui state (keadaan) pada DStream dengan menggabungkan nilai-nilai yang memiliki kunci yang sama.
   - flatMap: Membagi setiap elemen dalam RDD menjadi beberapa elemen dalam bentuk yang berbeda.

5. - rdd.take(5): Mengambil n elemen pertama dari RDD dan mengembalikannya dalam bentuk list.
   - transform: Menerapkan transformasi pada DStream.
   - rdd.sortByKey(False): Mengurutkan pasangan kunci-nilai dalam RDD berdasarkan kunci secara menurun (descending order).

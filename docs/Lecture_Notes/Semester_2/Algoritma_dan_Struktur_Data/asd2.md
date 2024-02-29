# **Lecture 2: Algoritma dan Struktur Data**
## **Algoritma**
Algoritma merupakan konsep dan ide di balik pembuatan program komputer yang digunakan untuku memberitahu komputer tentang **urutan kerja** apa yang harus dilakukan:

1. Untuk **memecahkan masalah** khusus yang terdefinisi secara baik.
2. Bersifat **independen** terhadap:
    - Jenis **hardware** yang akan digunakan oleh program.
    - **Bahasa pemrograman** yang akan digunakan untuk menulis program.

Algoritma merupakan **langkah logis tertentu** yang tepat dan pasti untuk memecahkan masalah yang dituangkan secara tertulis.

- Sangat diperlukan dalam **pemrograman** --> komputasi numeris.
- Program merupakan **implementasi dari algoritma**.

## **Struktur Data**
Struktur data adalah **penyimpanan** yang digunakan untuk **mengorganisasi** suatu data.

Merupakan suatu cara untuk **menata data** dalam komputer agar dapat **diakses** dan **diperbarui** secara efisien.

## **Algoritma sebagai Problem Solving**
Diperlukan strategi untuk problem solving ini:

1. Bekerja secara mundur, dimulai dengan **tujuan** -> langkah-langkah yang diperlukan untuk mencapai hasil.
2. Mencari masalah yang **mirip** yang telah berhasil diselesaikan sebelumnya sehingga bisa dibandingkan.
3. Mengurai atau **membagi** masalah menjadi beberapa sub-masalah.

Kesederhanaan harus menjadi tujuan utama dalam desain dan kompleksitas harus dihindari.

## **Sifat Algoritma**
Algoritma bersifat **umum** artinya:

- Tidak menggunakan simbol atau **sintaks** dari suatu bahasa pemrograman.
- Tidak tergantung pada **suatu bahasa pemrograman**.
- **Notasi-notasinya** dapat digunakan untuk **seluruh bahasa** manapun.

## **Kriteria Algoritma (Donald E. Knuth)**
- Input: algoritma dapat memiliki nol atau lebih input dari luar.
- Output: algoritma harus memiliki minimal satu buah output(keluaran).
- *Definiteness* (pasti): algoritma memiliki instruksi-instruksi yang jelas dan tidak ambigu.
- *Finiteness* (ada batas): algoritma harus memiliki titik berhenti(stopping role).
- *Efectiveness* (tepat dan efisien): algoritma sebisa mungkin harus dapat dilaksanakan dan efektif.

## **Jenis Proses Algoritma**
- *Sequence Process*: instruksi dikerjakan secara sekuensial, berurutan.
- *Selection Process*: instruksi dikerjakan jika memenuhi kriteria tertentu.
- *Iteration Process*: instruksi dikerjakan berulang selama memenuhi suatu kondisi tertentu.
- *Concurrent Process*: beberapa instruksi dikerjakan secara bersama.

## **Flowchart**
- Flowchart adalah bentuk gambar/diagram yang mempunyai aliran satu atau dua arah secara sekuensial yang digunakan untuk menentukan alur logika program.
- Flowchart digunakan untuk merepresentasikan maupun mendesain program. Oleh karena itu flowchart harus bisa merepresentasikan komponen-komponen dalam bahasa pemrograman.
- Flowchart adalah penggambaran secara grafik dari langkah-langkah dan urut-urutan instruksi dari suatu program. 

## **Pseudocode**
- Pseudocode merupakan notasi singkat untuk pemrograman yang menggunakan kombinasi struktur pemrograman informal dan deskripsi secara verbal.

## **Ketentuan Penulisan Pseudocode**
- Pernyataan ditulis dalam bahasa Inggris sederhana
- Setiap instruksi ditulis dalam baris terpisah
- Digunakan keyword dan indentasi untuk membedakan struktur kendali tertentu
- Setiap set instruksi ditulis dari atas ke bawah
- Kelompok pernyataan dapat dibentuk menjadi modul dan diberi nama

## **Notasi Algoritma Scholl 88**
Teks Algoritma terdiri dari 3 bagian yaitu:

1. Judul (Header)
    - berisi tentang judul program/modul/subrutin.
    - ada deskripsi singkat tentang intisari tujuan/kegunaan program tersebut.
2. Kamus
    - merupakan tempat mendefinisikan input, output, tipe data, variabel, konstanta, spesifikasi subrutin/modul.
3. Langkah urutan proses algoritma
    - berisi urutan instruksi-instruksi atau pemanggilan aksi.

## **Operasi Algoritma**
1. Operasi penerimaan informasi
    * `Read` - digunakan ketika algoritma menerima input dari record atau file
    * `Get` - digunakan ketika algoritma menerima input dari keyboard

Contoh:
```
Read namaMhs
Prompt
Get tanggal
```

2. Operasi pengeluaran informasi
    * `Print` - digunakan ketika output dikirim ke printer
    * `Write` - digunakan ketika output dikirim ke file
    * `Put, Output, Display` - digunakan ketika output dikirim ke screen
    * `Prompt` - diperlukan sebelum instruksi `Get`
  
Contoh:
```
Print `program completed`
Write customer record to master file
Put out name, address and postcode
Output total-tax
Display `End of data`
```

3. Operasi Aritmetika
    * Verb used: `Compute`,`Calculate`
    * Symbol used: `+`,`-`,`*`,`/`,`()`

Contoh:
```
Add number to total
Total = total + number
Divide total_marks by student_count
Sales_tax = cost_price * 0.10
Compute C = (F-32) * 5/9
```

4. Operasi pemberian nilai pada variabel
    * `Initialise` atau `Set` - pemberian nilai awal variabel
    * `=` atau `<-` - pemberian nilai sebagai hasil suatu proses aritmatik
    * `Save` atau `Store` - penyimpan variabel untuk digunakan kemudian

Contoh:
```
Initialize total_price to zero
Set student_count to 0
Total_price = cost_price + sales_tax
Total_price <- cost_price + sales_tax
Store customer_num in last_customer_num
```

5. Membandingkan 2 variabel dan memilih satu dari dua alternatif langkah operasi
    * `if`,`then`,`else`

Contoh:
```
IF student_attendance_status is part_time
  THEN
    add 1 to part_time_count
  ELSE
    add 1 to full_time_count
ENDIF
```

6. Pengulangan dari beberapa operasi
    * `dowhile`,`enddo`

Contoh:
```
DOWHILE student_total < 50
    Read student record
    Print student name, address to report
    Add 1 to student_total
ENDDO
```

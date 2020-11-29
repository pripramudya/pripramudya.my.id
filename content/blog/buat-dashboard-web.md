---
title: 'Panduan Pamungkas: Bagaimana Cara Membuat Dashboard Berbasis Web'
date: '2018-09-13'
slug: buat-dashboard-web
tags:
  - dashboard
  - R
---

Di tempat kerja, apakah Kamu pernah bingung harus mengerjakan apa hari ini?

Zaman now, kerjaan begitu numpuk, banyak, belum lagi di pressure dengan target yang tidak masuk akal, memang kadang-kadang bikin stress, bikin bingung apa yang harus dikerjakan lebih dulu.

Bagi Kamu yang berprofesi sebagai pegawai mungkin pernah mengalami hal tersebut. Masih lebih baik jika Kamu tahu apa yang harus Kamu capai untuk hari ini, minggu ini, atau bahkan untuk bulan ini.

Jika masih belum tahu, inilah mungkin permasalahannya.

Kamu sudah merasa banyak tugas yang sudah Kamu kerjakan hari ini, tapi tidak tahu sejauh mana kontribusi yang didapat perusahaan ataupun di tempat kerja Kamu atas hasil jerih payah Kamu.

Apakah tugas yang Kamu kerjakan sudah satu jalan dengan apa yang ingin dicapai oleh organisasi atau perusahaan Kamu?

Jika Kamu masih belum tahu apa yang ingin dicapai perusahaan Kamu, mungkin di tempat kerja Kamu dibutuhkan sebuah dashboard.

***

### Daftar Isi

* [Apa itu Dashboard](#dashboard)
* [8 Alasan Harus ada Dashboard](#alasan)
    + [Alasan#1: Fokus Mencapai Tujuan serta Visi dan Misi](#alasan1)
    + [Alasan#2: Berikan Gambaran Besar Tentang Kondisi Perusahaan](#alasan2)
    + [Alasan#3: Berikan Identifikasi dan Peringatan Dini Permasalahan](#alasan3)
    + [Alasan#4: Tingkatkan Kolaborasi dan Komunikasi Antar Lini](#alasan4)
    + [Alasan#5: Awali Langkah Perubahan Menuju Perbaikan](#alasan5)
    + [Alasan#6: Tingkatkan Efisiensi dan Produktivitas Kerja](#alasan6)
    + [Alasan#7: Permudah Mengambil Keputusan](#alasan7)
    + [Alasan#8: Sederhanakan Data Rumit](#alasan8)
* [Tipe Dashboard](#tipe)
* [Aplikasi Pembuat Dashboard](#aplikasi)
* [Sekilas Bahasa R](#r)
* [6 Langkah Membuat Dashboard Berbasis Web](#langkah)
    + [Langkah#1: Instal R dan RStudio](#langkah1)
    + [Langkah#2: Instal R Packages](#langkah2)
    + [Langkah#3: Unduh Contoh Dataset](#langkah3)
    + [Langkah#4: Buat Proyek Baru di RStudio](#langkah4)
    + [Langkah#5: Tulis Script](#langkah5)
    + [Langkah#6: Publikasikan di shinyapps.io](#langkah6)
    
***

### Apa itu Dashboard? {#dashboard}

Dashboard.

Begitu mendengar kata ini, mungkin Kamu teringat langsung pada sebuah tampilan yang ada di mobil atau motor Kamu. Fungsinya adalah untuk mengetahui kondisi terkini dari kendaraan Kamu.

Berapa kecepatannya saat ini, berapa jarak total yang sudah ditempuh, sampai dengan berapa banyak bensin yang masih tersedia.

Ada banyak sekali definisi dari dashboard dan menurut saya yang paling baik menjelaskan “dashboard” adalah dari [Stephen Few](http://www.stephen-few.com/) di bukunya yang berjudul Information Dashboard Design:

> a visual **display** of the **most important information** needed to **achieve one or more objectives**; consolidated and arranged on a single screen so the information can be monitored **at a glance.**

Jadi, dashboard adalah sebuah **tampilan** yang dibutuhkan **untuk mencapai tujuan, diatur** sedemikian rupa sehingga informasi bisa dilihat **pada satu layar dan satu kali lihat saja.**

Jika sampai dengan sini Kamu masih ragu dan merasa tidak memerlukan dashboard di tempat kerja Kamu, mungkin alasan-alasan berikut bisa merubah pemikiran Kamu.

### 8 Alasan Kenapa Harus Ada Dashboard di Tempat Kerja Kamu {#alasan}

#### Alasan#1: Dashboard Membuat Kamu Fokus Mencapai Tujuan serta Visi dan Misi Perusahaan Kamu {#alasan1}
Orang gila.

Waktu kecil dulu, saya sering kali melihat orang gila, tanpa pakaian sehelai pun, berjalan santai di trotoar.

Ke mana mereka pergi? Yaa mereka berjalan saja, tanpa ada tujuan.

Masih lebih baik zombie yang sering muncul di film. Mereka masih punya tujuan: makan orang hidup.

Dengan dashboard, memastikan Kamu tidak menjadi orang gila, yang bingung mau ngapain di kantor. Bekerja, menyelesaikan tugas sesuai dengan tujuan, visi, dan misi perusahaan Kamu.

> Set realistic goals, keep re-evaluating, and be consistent.

Tujuan atau target bisa ditampilkan di dashboard. Target menantang pada dashboard yang menempel di ruang kerja Kamu membuat Kamu berpacu memberikan yang terbaik untuk mencapainya.

Terkadang manajemen memberikan target pada saat rapat dilakukan. Setelah rapat selesai, target tersebut biasanya di broadcast melalui media aplikasi grup di whatsapp oleh notulis. Satu atau dua hari kemudian, Kamu masih bisa melihatnya. Satu atau dua minggu kemudian? Dimana detail target berupa pesan di whatsapp itu, pasti Kamu agak susah mencarinya.

Dashboard bisa menampilkan ringkasan target beserta pencapaiannya tanpa harus bergantung kepada aplikasi whatsapp.

#### Alasan#2: Dashboard Memberikan Gambaran Besar Tentang Kondisi Perusahaan Kamu Saat Ini {#alasan2}

Perusahaan didirikan untuk menghasilkan laba. Jika tidak bisa menghasilkan laba maka perusahaan dapat dikatakan dalam kondisi yang tidak bagus. Selain dari laba, kondisi perusahaan dapat dilihat dari pendapatannya.

Dua kunci indikator ini, laba dan pendapatan dapat ditampilkan pada dashboard secara langsung. Dengan hanya melihat dashboard ini, Kamu dapat langsung mengetahui kondisi perusahaan Kamu saat ini. Apakah dalam kondisi yang baik atau tidak.

Kesimpulan terkait kondisi perusahaan dapat Kamu ambil tentunya juga dengan bantuan data-data pendukung indikator lainnya, seperti biaya/pengeluaran, ataupun jumlah pelanggan.

Dari berbagai macam data serta indikator tersebut di dashboard dapat ditampilkan seluruh ringkasannya (*executive summary*).

#### Alasan#3: Dashboard Memberikan Identifikasi dan Peringatan Dini Permasalahan di Perusahaan Kamu {#alasan3}

Sistem peringatan dini juga bisa ditampilkan di sebuah dashboard. Dengan adanya peringatan dini, maka Kamu dapat mengambil langkah untuk mencegah ataupun meminimalisir terjadinya risiko yang dapat merugikan perusahaan.

Contohnya, bagaimana menjaga pelanggan untuk tetap memakai produk perusahaan Kamu. Dashboard bisa dibuat untuk  mengidentifikasi dan memprediksi kira-kira pelanggan yang akan beralih memakai produk kompetitor perusahaan Kamu.

Informasi ini tentu akan berguna sekali, sehingga Kamu bisa melakukan program-program yang dapat membuat pelanggan Kamu tetap setia untuk menggunakan produk perusahaan Kamu dan tidak jadi beralih ke kompetitor.

#### Alasan#4: Dashboard Meningkatkan Kolaborasi dan Komunikasi Antar Lini {#alasan4}

Salah satu fungsi dasar dashboard adalah sebagai alat bantu untuk berkomunikasi.

Berkomunikasi dengan siapa?

*Stakeholders.*

Semua pihak yang berkaitan dalam usaha untuk mencapai tujuan perusahaan Kamu. Pihak ini diantaranya direksi, pimpinan unit/departemen, manajer, pegawai/staff, vendor, dan lainnya.

Dashboard menyatukan stakeholders untuk satu irama dalam pencapaian tujuan perusahaan Kamu.

Dengan adanya dashboard memungkinkan koordinasi dan kolaborasi antar stakeholders menjadi lebih efektif sehingga tujuan perusahaan Kamu dapat tercapai sesuai ekspektasi.

#### Alasan#5: Dashboard Mengawali Langkah Perubahan Menuju Perbaikan {#alasan5}

Adanya inisiatif untuk membuat dashboard merupakan langkah awal perubahan dalam rangka menjadikan perusahaan Kamu menjadi lebih baik lagi.

Dashboard menjadikan kinerja dan performansi masing-masing lini atau departemen menjadi lebih transparan serta bisa dilihat oleh semua pihak yang berkepentingan terkait pencapaian tujuan perusahaan Kamu.

Keterbukaan akses terhadap informasi dan performansi ini membuat masing-masing lini atau departemen semakin berpacu untuk menorehkan prestasi terbaiknya demi kejayaan perusahaan Kamu.

Selain itu, dashboard juga dapat memberikan feedback ataupun evaluasi terhadap hasil kinerja dan performansi. Dari evaluasi ini, tentunya manajemen Kamu akan mengambil tindakan ataupun program untuk memperbaiki kinerja menjadi lebih baik lagi.

#### Alasan#6: Dashboard Meningkatkan Efisiensi dan Produktivitas Kerja {#alasan6}

Berkat penggunaan dashboard di tahun pertamanya, [IBM merealisasikan efisiensi biaya sekitar USD 2 juta](https://www-01.ibm.com/common/ssi/cgi-bin/ssialias?htmlfid=CIE03086USEN).

Efisiensi biaya tersebut didapat dari hasil penggunaan dashboard yang meminimalisir pengolahan data dan laporan secara manual sehingga memberikan efesiensi dan produktivitas kerja di segala lini perusahaan IBM.

Mengumpulkan dan mengolah data secara manual menggunakan aplikasi *spreadsheet* memiliki risiko kesalahan ketik/input (*human error*) yang cukup tinggi serta menghabiskan banyak waktu dan tenaga.

Pengolahan data tersebut bisa di-otomatisasi dengan menggunakan kode pemrograman sehingga di dashboard dapat ditampilkan informasi atau laporan sesuai keinginan pengguna.

Pekerjaan pengolahan data yang jenuh dan berulang dapat diminimalisir bahkan dapat dihilangkan sehingga Kamu bisa mengemat waktu, tenaga, maupun biaya serta dapat mengalokasikan sumber daya tersebut ke bagian yang menurut Kamu jauh lebih penting.

#### Alasan#7: Dashboard Mempermudah Kamu dalam Mengambil Keputusan {#alasan7}

Sekarang, Kamu tidak perlu mengambil sebuah keputusan hanya berdasarkan *feeling* saja, karena sudah ada dashboard.

Fakta dan analisis data, bahkan sebuah rekomendasi program yang harus diambil dapat ditampilkan di dashboard. Ringkasan informasi dari masing-masing lini atau departemen atau di unit kecil bisa diatur sedemikian rupa sehingga dapat disajikan dalam satu tampilan saja sehingga membuat keputusan Kamu menjadi lebih efektif.

Kamu juga tidak perlu waktu lama dalam mengambil keputusan, menunggu data, fakta, laporan dan analisis dari masing-masing departemen. Cukup lihat informasi di dashboard, Kamu dapat lebih cepat dalam mengambil keputusan terbaik bagi perusahaan Kamu.

#### Alasan#8: Dashboard Menyederhanakan Data Rumit Menjadi Informasi yang Strategis {#alasan8}

Jika data perusahaan Kamu diambil dari berbagai sumber dan struktur yang berbeda, maka bisa dikatakan data perusahaan Kamu adalah data rumit.

Data rumit ini dapat disederhanakan dengan pemrograman terlebih dahulu. Dashboard membuat data rumit ini seolah “dipaksa” untuk disederhanakan sehingga Kamu bisa dengan mudah mendapatkan insight dari kerumitan data tersebut.

Visualisasi berupa grafik di dashboard akan membuat data rumit tersebut menjadi lebih sederhana.

Dengan beberapa tampilan berupa grafik dan ringkasannya, Kamu akan lebih mudah memperoleh informasi dan *insight* yang strategis untuk membuat sebuah inovasi baru bagi kemajuan perusahaan Kamu.

Alasan-alasan di atas tentunya sudah meyakinkan Kamu untuk mengupayakan adanya sebuah dasboard di tempat Kamu.

Yang menjadi pertanyaan selanjutnya adalah bagaimana cara membuat dashboard?

Pada artikel ini pun, saya akan memandu Kamu bagaimana cara membuat dashboard sederhana berbasis web.

Dashboard dibuat dengan menggunakan bahasa R dan Shiny (dijelaskan lebih lanjut di bawah).

### Tipe Dashboard {#tipe}

Dashboard dibagi menjadi 3 jenis: strategis, analitis, dan operasional.

#### #1: Dashboard Strategis

Menampilkan ringkasan dan informasi strategis perusahaan yang biasanya digunakan oleh level manajemen atau direksi. Data total penjualan, total laba, dan marjin keuntungan merupakan beberapa contoh yang ditampilkan pada dashboard strategis.

#### #2: Dashboard Analitis

Menampilkan analisis data sehingga didapatkan pola, trend, serta insight dari suatu studi kasus atau permasalahan. Misalnya, pengguna ingin mengetahui informasi 5 produk dengan penjualan tertinggi atau persentase pelanggan churn pada bulan berjalan.

#### #3: Dashboard Operasional

Menampilkan data terkini (bahkan diperbaharui secara real time) dari suatu kegiatan operasional bisnis. Jumlah pengunjung website dan beban kerja server merupakan beberapa contoh informasi yang terdapat pada dashboard operasional.

### Aplikasi Pembuat Dashboard {#aplikasi}

Cukup banyak aplikasi yang bisa digunakan untuk membuat dashboard. Saya akan menjelaskan sedikit saja 3 aplikasi yang pernah saya gunakan, yakni: Microsoft Excel, Tableau, dan R Shiny.

Perbandingan Excel, Tableau, dan R Shiny:

![](/post/2018-09-13-buat-dashboard-web_files/perbandingan.jpg)

#### #1: Microsoft Excel

Kalau yang satu ini bisa dikatakan aplikasi sejuta umat eh semiliar umat. Semua profesional pasti pernah menggunakannya. Dengan memanipulasi data, format, linking ke sheet utama, Kamu bisa membuat dashboard menggunakan Excel. Kekurangannya, untuk membuat dashboard Excel berbasis web, Kamu harus tahu tentang pemrograman VBA (macros).

#### #2: Tableau

Software data visualisasi ini merupakan software yang paling populer diantara yang lain karena sangat mudah dalam penggunaannya. Bagi Kamu yang tidak menguasai satu bahasa pemrograman pun, tidak perlu khawatir, tinggal poin, click, drag, dan drop, Kamu sudah bisa menampilkan grafik yang indah. Gabungkan grafik-grafik yang Kamu buat tadi dalam satu tampilan, jadilah dashboard.

Benar-benar mudah sekali.

Jika Kamu memiliki dana yang cukup untuk membeli lisensinya, maka Tableau pasti jadi nomor 1 pilihan Kamu.

#### #3: R Shiny

Shiny adalah salah satu paket dari bahasa R yang memudahkan Kamu untuk membuat aplikasi berbasis web tanpa harus menguasai pemrograman HTML, CSS, ataupun JavaScript.

Ya, Kamu hanya perlu menguasai bahasa pemrograman R untuk bisa membuat dashboard berbasis web.

Jangan khawatir, di artikel ini saya akan memandu Kamu langkah demi langkah **bagaimana cara membuat dashboard berbasis web dengan menggunakan R Shiny.**

### Sekilas Tentang Bahasa R {#r}

R adalah perangkat lunak gratis untuk komputasi dan analisis data statistik serta menampilkan visualisasi grafik. R didukung oleh ribuan *packages* yang dibuat oleh banyak kontributor aktif sehingga memudahkan pengguna dalam pengembangan aplikasi.

Shiny adalah salah satu paket R.

R banyak digunakan oleh berbagai kalangan dan bermacam bidang, mulai dari akademis sampai skala bisnis.

Bahasa pemrograman ini bisa diinstal di seluruh sistem operasi: Windows, Linux, ataupun Mac. Untuk memudahkan pengembangan aplikasi berbasis R, saya anjurkan menginstal IDE (*integrated development environment*)  untuk R, yakni RStudio.

Jadi, untuk memulai membuat dashboard, R dan RStudio harus diinstal terlebih dulu di komputer.

### 6 Langkah Bagaimana Cara Membuat Dashboard Berbasis Web {#langkah}

#### Langkah#1: Instal R dan RStudio {#langkah1}

Pilihlah paket instalasi sesuai sistem operasi yang Kamu pakai. Untuk RStudio, pilih yang versi desktop.

* R dapat diunduh di [sini](https://repo.bppt.go.id/cran/).
* RStudio dapat diunduh di [sini](https://www.rstudio.com/products/rstudio/download/).

Buka software RStudio.

Layout RStudio terdiri dari bagian Script, Console, Variable, dan Output.

![](/post/2018-09-13-buat-dashboard-web_files/Rstudio_Layout.jpg)

#### Langkah#2: Instal R *Packages* {#langkah2}

Packages adalah komponen penting yang memungkinkan pengguna untuk menggunakan program siap pakai tanpa harus membuatnya dari awal.

Pengguna cukup menginstalnya saja dengan menggunakan perintah 
`install.packages()`

Lalu, packages apa saja yang perlu diinstal?

Berikut daftarnya:

* `tidyverse` (untuk memanipulasi data)
* `shinydashboard` (untuk menampilkan dashboard)

Pada bagian CONSOLE ketik perintah:

```
install.packages("tidyverse")
install.packages("shiny")
install.packages("shinydashboard")
```

#### Langkah#3: Unduh Contoh Dataset {#langkah3}

Unduh [Telco Customer Churn](/data/WA_Fn-UseC_-Telco-Customer-Churn.csv).

Nama filenya: `WA_Fn-UseC_-Telco-Customer-Churn.csv`

Dataset ini merupakan file yang bisa dipakai untuk demo perangkat lunak IBM Watson Analytics.

Ceritanya, Kamu adalah seorang analis di salah satu perusahaan telco yang sedang ingin mengetahui kenapa beberapa pelanggan beralih ke kompetitor yang lain.

Dataset ini terdiri beberapa informasi tentang:

* Pelanggan yang pindah mulai bulan lalu – kolom ini dinamakan Churn.
* Berlangganan layanan apa –  phone, multiple lines, internet, online security, online backup, device protection, tech support, streaming TV, movies.
* Informasi pelanggan – berapa lama mereka berlangganan, jenis kontrak, cara pembayaran, apakah menggunakan tagihan tanpa kertas, tagihan bulanan, dan total tagihan.
* Info demografi pelanggan – jenis kelamin, gender, jarak usia, dan apakah mereka memiliki pasangan dan mandiri.
* Untuk panduan membuat dashboard ini mencakup informasi total pelanggan, total pendapatan, jumlah pelanggan churn, dan persentase churn.

Selain itu juga ada grafik interaktif jumlah pelanggan yang dibagi berdasarkan kategori layanan internet dan kontrak langganan serta bisa diketahui berapa jumlah pelanggan yang churn dan yang tidak churn.

Terakhir ditampilkan grafik yang menunjukkan faktor apa yang memiliki persentase churn yang paling tinggi sehingga dari informasi ini dapat dibuat usulan program untuk mengurangi pelanggan churn berdasarkan faktor tersebut.

#### Langkah#4: Buat Proyek Baru di RStudio {#langkah4}

Pada 3 langkah sebelumnya sudah dilakukan tahap persiapan, sekarang langkah utamanya, yakni pembuatan aplikasi dan menulis program.

Berikut rincian tahapannya, dimulai dengan membuat dan menamai proyek baru di RStudio:

* Pilih menu File > New Project > New Directory > New Project
* Isi Nama Directory, misalnya “dashboard” dan klik Create Project.
* Pindahkan dataset yang baru saja di unduh tadi ke folder “dashboard”.
* Pilih menu File > New File > R Script
* Klik icon kecil bergambar floppy disk untuk menyimpan.
* Beri nama `app.R`.


Struktur aplikasi Shiny bisa juga terdiri dari dua file script: `ui.R` dan `server.R` yang harus disimpan di dalam directory project.

* `ui.R` mengatur layout dan tampilan aplikasi.
* `server.R` mengatur instruksi yang dibutuhkan untuk membuat aplikasi.

Selain stuktur dua file, shiny juga mengenali struktur satu file, yakni dengan menulis script di file `app.R`.

Untuk panduan ini, digunakan file `app.R` agar memudahkan Kamu untuk menyalin dan menempelkan keseluruhan script sehingga bisa langsung dijalankan di komputer Kamu.

Setelah menulis script di file `app.R`, maka aplikasi bisa dijalankan dengan mengklik tombol “Run App” pada atau dengan mengetik `runApp(“nama_proyek”)` di CONSOLE.


#### Langkah#5: Tulis Script {#langkah5}

Berikut script untuk membuat Dashboard Churn Pelanggan disertai penjelasannya:

```{r eval = FALSE}
#~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
# DASHBOARD PELANGGAN CHURN
#~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
# Aplikasi ini mencakup bagaimana cara membuat: 
# - ringkasan dari sumber data (manipulasi data)
#   menggunakan dplyr
# - modifikasi tema ggplot2
# - grafik interaktif
# - grafik biasa
# - dashboard berbasis web yang dapat diakses di
#   shinyapps.io
#~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

#~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
# INISIASI PAKET YANG DIBUTUHKAN
# - tidyverse untuk manipulasi data
# - shinydashboard untuk membuat dashboard
#~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

library(tidyverse)
library(shinydashboard)

#~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
# BUKA DATA
# Baca file csv dan simpan di variabel "data".
#~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

data <- read.csv("WA_Fn-UseC_-Telco-Customer-Churn.csv")

#~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
# MANIPULASI DATA
# Membuat data tabel baru untuk menganalisis
# faktor yang paling tinggi mempengaruhi Churn
# pelanggan menggunakan paket dari dplyr.
# Variabel masing-masing field dihitung jumlah 
# pelanggannya.
#~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

ringkasan <- data %>% 
  group_by(Churn) %>% 
  summarise(
    Pria = length(customerID[gender == "Male"]),
    Wanita = length(customerID[gender == "Female"]),
    Senior = length(customerID[SeniorCitizen == 1]),
    Non.Senior = length(customerID[SeniorCitizen == 0]),
    Pasangan = length(customerID[Partner == "Yes"]),
    Non.Pasangan = length(customerID[Partner == "No"]),
    Mandiri = length(customerID[Dependents == "Yes"]),
    Non.Mandiri = length(customerID[Dependents == "No"]),
    Telepon = length(customerID[PhoneService == "Yes"]),
    Non.Telepon = length(customerID[PhoneService == "No"]),
    Multi.Line = length(customerID[MultipleLines == "Yes"]),
    Non.Multi.Line = length(customerID[MultipleLines == "No"]),
    Layanan.DSL = length(customerID[InternetService == "DSL"]),
    Layanan.FO = length(customerID[InternetService == "Fiber optic"]),
    Non.Layanan = length(customerID[InternetService == "No"]),
    OL.Security = length(customerID[OnlineSecurity =="Yes"]),
    Non.OL.Security = length(customerID[OnlineSecurity =="No"]),
    OL.Backup = length(customerID[OnlineBackup =="Yes"]),
    Non.OL.Backup = length(customerID[OnlineBackup =="No"]),
    Proteksi = length(customerID[DeviceProtection =="Yes"]),
    Non.Proteksi= length(customerID[DeviceProtection =="No"]),
    Support = length(customerID[TechSupport =="Yes"]),
    Non.Support = length(customerID[TechSupport =="No"]),
    StreamTV = length(customerID[StreamingTV =="Yes"]),
    Non.StreamTV = length(customerID[StreamingTV =="No"]),
    StreamMov = length(customerID[StreamingMovies =="Yes"]),
    Non.StreamMov = length(customerID[StreamingMovies =="No"]),
    Kontrak.Bulanan = length(customerID[Contract == "Month-to-month"]),
    Kontrak.Setahun = length(customerID[Contract == "One year"]),
    Kontrak.Duatahun = length(customerID[Contract == "Two year"]),
    Tagihan.Kertas = length(customerID[PaperlessBilling == "No"]),
    Non.Tagihan.Kertas = length(customerID[PaperlessBilling == "Yes"]),
    Bayar.Bank = length(customerID[PaymentMethod == "Bank transfer (automatic)"]),
    Bayar.Kredit = length(customerID[PaymentMethod == "Credit card (automatic)"]),
    Bayar.Cek = length(customerID[PaymentMethod == "Electronic check"]),
    Bayar.Cek.Email = length(customerID[PaymentMethod == "Mailed check"])
  )

#~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
# MENGUBAH DATA WIDE FORMAT KE LONG FORMAT
# Diubah ke long format untuk mempermudah
# perhitungan dan meringkas data.
#~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
ringkasan2 <- gather(ringkasan, "Faktor", "Jml.Pelanggan", 2:37)


#~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
# MERINGKAS DATA
# Menghitung persentase churn masing-masing 
# faktor 
#~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

ringkasan.churn <- ringkasan2 %>% 
  group_by(Faktor) %>% 
  summarise(pelanggan = sum(Jml.Pelanggan), 
            churn = sum(Jml.Pelanggan[Churn == "Yes"]) / sum(Jml.Pelanggan) * 100) %>% 
  arrange(desc(churn))

#~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
# MODIFIKASI TEMA
#~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

tema <-
  theme(text = element_text(family = "Verdana", color = "#444444")) +
  theme(plot.title = element_text(size = 24)) +
  theme(plot.subtitle = element_text(size = 18)) +
  theme(axis.title = element_text(size = 14)) +
  theme(axis.title.y = element_text(angle = 0, vjust = .5, margin = margin(r = 15))) +
  theme(axis.text = element_text(size = 10)) +
  theme(axis.title.x = element_text(margin = margin(t = 20))) +
  theme(legend.title = element_blank())

#~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
# JUDUL DASHBOARD
#~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

header <- dashboardHeader(
    title = HTML(paste(icon("cubes"), "Dashboard"))
  )

#~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
# MENU DASHBOARD
#~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

sidebar <- dashboardSidebar(
  sidebarMenu(id = "tabs", 
              menuItem("Pelanggan",
                       tabName = "pelanggan", 
                       icon = icon("address-book")
              )
  )
)

#~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
# KOTAK INFORMASI TOTAL PELANGGAN
#~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
info.1 <- valueBox(
  value = length(data$customerID),
  subtitle = "total pelanggan", 
  icon = icon("users"), width = 3
)

#~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
# KOTAK INFORMASI TOTAL PENDAPATAN
#~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

info.2 <- valueBox(
  value = formatC(sum(data$TotalCharges, na.rm = "yes")/1000000, 
                  big.mark = ".", decimal.mark = ",", 
                  format = "f", digits = 2),
  subtitle = "total pendapatan ($juta)", 
  icon = icon("money"), width = 3
)

#~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
# KOTAK INFORMASI TOTAL PELANGGAN CHURN
#~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

info.3 <- valueBox(
  value = length(data$customerID[data$Churn == "Yes"]),
  subtitle = "pelanggan churn",
  icon = icon("user-times"), width = 3
)

#~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
# KOTAK INFORMASI PERSENTASE CHURN PELANGGAN
#~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

info.4 <- valueBox(
  value = formatC(length(data$customerID[data$Churn == "Yes"]) /
                    length(data$customerID) * 100, big.mark = ".", 
                  decimal.mark = ",", format = "f", digits = 2),
  subtitle = "persen churn (%)",
  icon = icon("line-chart"), width = 3
)

#~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
# GRAFIK FAKTOR LAYANAN INTERNET
#~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

box.grafik.1 <- box(
  title = "Faktor Layanan Internet",
  solidHeader = TRUE,
  radioButtons(
    inputId = "keterangan1",
    label = "Churn?",
    choices = c("Ya" = "Yes", "Tidak" = "No"),
    inline = TRUE
  ),
  plotOutput("grafik1", height = "150px"),
  width = 6,
  status = "primary"
)

#~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
# GRAFIK FAKTOR KONTRAK LANGGANAN
#~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

box.grafik.2 <- box(
  title = "Faktor Kontrak Langganan",
  solidHeader = TRUE,
  radioButtons(
    inputId = "keterangan2",
    label = "Churn?",
    choices = c("Ya" = "Yes", "Tidak" = "No"),
    inline = TRUE
  ),
  plotOutput("grafik2", height = "150px"),
  width = 6,
  status = "primary"
)

#~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
# KOTAK INFROMASI ANALISIS CHURN
#~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

box.analisis <- box(
  title = "Analisis Churn",
  solidHeader = TRUE,
  plotOutput("grafik.analisis", height = "750px"),
  width = 12,
  status = "primary"
)

#~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
# MENGGABUNGKAN SEMUA GRAFIK DI BODY DASHBOARD
#~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

body <- dashboardBody(
  tabItems(
    tabItem(tabName = "pelanggan",
            fluidRow(info.1, info.2, info.3, info.4, 
                     box.grafik.1, box.grafik.2, box.analisis))
  )
)

#~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
# MENGGABUNGKAN SEMUA ELEMEN VISUAL DASHBOARD
#~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

ui <- dashboardPage(header, sidebar, body)
  
#~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
# MEMETAKAN FUNGSI INPUT DAN OUTPUT ELEMEN
#~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

server <- function(input, output) {

#~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
# GRAFIK INTERAKTIF LAYANAN INTERNET
#~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

output$grafik1 <- renderPlot({
    data %>%
      group_by(InternetService) %>%
      filter(Churn == input$keterangan1) %>%
      summarise(Jumlah.Pelanggan = n()) %>%
      ggplot(aes(y = Jumlah.Pelanggan, x = InternetService)) +
      geom_bar(stat = "identity", fill = "#0072B2") +
      geom_text(aes(label = Jumlah.Pelanggan), hjust = 1.1, color = "white") +
      coord_flip() + 
      labs(y = "Jumlah Pelanggan", x = NULL) +
      tema
  })

#~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
# GRAFIK INTERAKTIF FAKTOR KONTRAK LANGGANAN
#~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

output$grafik2 <- renderPlot({
  data %>%
    group_by(Contract) %>%
    filter(Churn == input$keterangan2) %>%
    summarise(Jumlah.Pelanggan = n()) %>%
    ggplot(aes(y = Jumlah.Pelanggan, x = Contract)) +
    geom_bar(stat = "identity", fill = "#0072B2") +
    geom_text(aes(label = Jumlah.Pelanggan), hjust = 1.1, color = "white") +
    coord_flip() + 
    labs(y = "Jumlah Pelanggan", x = NULL) +
    tema
})

#~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
# GRAFIK ANALISIS FAKTOR CHURN
#~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

output$grafik.analisis <- renderPlot({
  ringkasan.churn %>% 
    ggplot(aes(y = churn, x = reorder(Faktor, churn))) + 
    geom_bar(stat = "identity", fill = "#0072B2") + 
    geom_text(aes(label = round(churn, 1)), hjust = 1.1, color = "white") + 
    coord_flip() + ggtitle("Faktor Churn Pelanggan") + 
    labs(y = "Persen Churn", x = NULL) + 
    tema
  
})

}

#~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ 
# MENGGABUNGKAN ELEMEN UI DAN SERVER
#~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

shinyApp(ui = ui, server = server)
```

#### Langkah#6: Publikasikan di shinyapps.io {#langkah6}

Jika script di langkah #5 sudah dibuat dan dicoba untuk dijalankan di komputer serta berhasil dengan sukses, Kamu bisa mempublikasikan aplikasi Kamu di [shinyapps.io](http://shinyapps.io/).

Shinyapps adalah hosting tempat menyimpan dan mempublikasikan aplikasi Shiny agar bisa diakses oleh siapapun di internet.

Berikut tahapan bagaimana mempublikasikan aplikasi di shinyapps.io:

* Instal rsconnect package dengan mengetikkan `install.packages(“rsconnect”)` di CONSOLE RStudio.
* Buat akun di shinyapps.io.
* Navigasi ke menu Account > Tokens, lalu klik show. 
* Salin dan tempel kode di CONSOLE RStudio Kamu.
* Ketik perintah `rsconnect::deployApp()` di CONSOLE RStudio untuk mempublikasikan aplikasi di shinyapps.io.


![](/post/2018-09-13-buat-dashboard-web_files/dashboard.churn_.png)

Aplikasi yang dibuat melalui panduan ini hasilnya dapat dilihat di link berikut: [dashboard churn](http://pripramudya.shinyapps.io/dashboard/).


Akhir kata, dashboard merupakan salah satu tool yang memiliki fungsi utama untuk mengkomunikasikan insight yang didapat dari hasil eksplorasi data analisis yang Kamu lakukan.

Shiny memudahkan pengguna untuk membuat dashboard dengan menggunakan bahasa R tanpa harus memiliki pengetahuan tentang aplikasi web.

Selain dapat dipublikasikan melalui shinyapps.io, Shiny juga bisa diakses melalui server internal dengan menggunakan Shiny Server.

Jika Kamu masih bingung tentang artikel ini, maka saya sarankan Kamu untuk membaca buku [3 Langkah Kilat Mahir Analisis Data](/mahir-analisis-data).

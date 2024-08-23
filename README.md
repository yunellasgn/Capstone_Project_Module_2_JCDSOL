# Capstone_Project_Module_2_JCDSOL
Capstone Project Data Analysis from Airbnb Listings Bangkok Dataset

# **Latar Belakang**

## Business Context

Sebuah perusahaan Airbnb yang bergerak di bidang penyediaan tempat penginapan meminta kita sebagai seorang *data analyst* untuk menganalisa data mengenai tempat penginapan yang ada di Bangkok, Thailand. Perusahaan ini memiliki daftar dataset tempat-tempat penginapan (_listings_) yang tersebar di beberapa lingkungan di Bangkok dengan tipe-tipe kamar yang berbeda.

Perusahaan ingin mengetahui tempat penginapan dengan tipe kamar bagaimana yang banyak tersedia di dataset daftar tempat penginapan yang dimiliki perusahaan. Informasi ini akan membantu perusahaan untuk mengetahui apakah daftar tempat penginapan yang ada dalam list Airbnb sudah sesuai/menjawab kebutuhan customer.

Tipe kamar yang tersedia dalam list yang dimiliki perusahaan ada 4 kategori yaitu : Entire home/apt, private room, hotel, dan shared room. Minimal masa inap/sewa untuk setiap tipe kamar tersebut adalah kurang-lebih untuk tipe Entire home/apt (21 malam), private room (9 malam), shared room (3 malam), dan hotel (1 malam). Minimal masa sewa yang durasinya paling lama, jumlah reviews nya justru banyak. Sebagai data analis, kita dapat menganalisa hal ini.

## Problem Statements

Sebagai seorang *data analyst*, kita akan mencoba menjawab pertanyaan berikut :

**Bagaimana tempat penginapan yang dicari para customer sehingga jumlah reviews tertinggi (197.943) justru diperoleh tempat penginapan dengan tipe kamar yang minimal sewanya justru paling lama (21 hari) ?**

## Goal/Tujuan

* Menginformasikan kepada perusahaan bagaimana **karakteristik tempat penginapan** yang menjadi kebutuhan customer
* **Merekomendasi suatu _sugestion_** sebagai tambahan/pendukung kepada perusahaan agar membooster para customer lebih antusias memberikan review sehingga jumlah review dari penginapan selain Entire room dapat meningkat, serta menghitung estimasi % keuntungan yang diperoleh perusahaan dari saran yang berikan

* # **Kesimpulan** 

Dari analisis yang telah dilakukan, kita memperoleh **kesimpulan** sebagai berikut :

* Dari hasil statistika inferensial, kita ketahui bahwa dari 4 tipe kamar dalam dataset, **ada salah satu tipe kamar yang berpengaruh signifikan**.
* Dari 15854 data penginapan di Bangkok yang kita miliki, tipe kamar Entire room/apt memang tersedia paling tinggi (**56,21%**).
* Kebanyakan lingkungan yang ada di Bangkok memang menyediakan penginapan dengan tipe kamar **'Entire room/apt'**.
* Data set ini terdiri dari 50 lingkungan dimana lingkungan yang paling favorit (jumlah reviewnya tinggi) dan paling banyak menyediakan tempat penginapan adalah lingkungan **Khlong Tei** dan **Vadhana**.
Lingkungan Khlong Tei memang menyediakan banyak tempat menarik untuk travelling seperti Grand Palace, Wat Arun, Sea Life Bangkok Ocean World, dan lainnya https://www.trip.com/travel-guide/attraction/khlong-toei-2016435/tourist-attractions/?locale=en-XX&curr=USD. Untuk lingkungan Vadhana atau dikenal juga Watthana adalah ternyata salah satu kawasan komersial di Bangkok dengan banyak kondominium.
* Penginapan yang dibutuhkan/dicari customer cenderung yang **memberikan ruang privasi** untuk penyewa, yaitu tipe kamar 'Entire room/apt' dan 'private room'. Hal ini ditunjukkan bahwa penginapan yang sudah banyak di booking ke depan (terlihat dari data availability_365 berada di batas bawah Q1) merupakan tipe kamar Entire room/apt (87%) dan private room(13%). Berdasarkan artikel https://bnbduck.com/airbnb-private-room-vs-entire-place/ juga menyatakan customer memilih tipe entire agar lebih privasi dan bebas, dan jika ingin versi lebih murah dapat memilih yang tipe private room. Ini semakin menguatkan mengapa data juga menunjukkan hal demikian.

* Tipe **customer** yang biasanya memesan tempat penginapan di Airbnb Bangkok ini sebagian besar adalah :
1. **Turis Internasional**. Menurut _Elite Plus Magazine_, Bangkok adalah salah satu pasar Airbnb tersebar di dunia. Daya tarik Bangkok/Thailand ini sangat kuat di kancah internasional, banyak wisatawan dunia tertarik berkunjung untuk merasakan _hospitality_, budaya, makanan, dan tradisi negara Thailand. Dengan durasi wisata yang lama (mungkin 4 hari, 1 minggu, atau lebih), penginapan tipe Entire room menjadi pilihan paling banyak yang dipilih pada turis asing.
2. **Ekspatriat**. Bangkok memiliki banyak distrik komersial sehingga banyak warga negara asing yang tinggal di Bangkok untuk keperluan bisnis. Ini juga dapat membuat pemesanan penginapan tipe Entire room menjadi lebih dominan.

* Kita menganalisa data dari kurun waktu 2012-2022. Hasil analisa menunjukkan adanya peningkatan dari tahun 2012 sampai 2020, lalu 2021 terjadi penurunan sekitar 7 kali lipat yang disebabkan pandemi covid-19 yang menyerang sektor pariwisata. Selanjutnya, ditahun 2022 pariwisata sudah kembali bangkit meningkat 50 kali lipat. Hal ini menunjukkan sektor pariwisata Bangkok optimis akan semakin berkembang ke depannya.

* Rekomendasi / **Saran** :

* Sebagai tambahan, saran bersifat pendukung dari segi bisnis, untuk tipe kamar selain 'Entire home/apt' kita dapat melakukan sesuatu yang mampu meningkatkan jumlah review. Kita ketahui bahwa jumlah review pastinya berbanding lurus dengan jumlah transaksi yang berhasil. Transaksi meningkat berarti revenue perusahaan juga meningkat. 

Berdasarkan artikel https://www.hostaway.com/blog/how-to-get-more-reviews-on-airbnb/ dari beberapa cara meningkatkan jumlah review, faktor nomor 1 adalah _competitive price_. Ini berarti cara-cara yang berkaitan dengan harga memang yang paling menarik perhatian customer. Oleh karena itu, kami menyarankan membuatkan promo yaitu memberikan e-voucher berupa potongan harga kepada customer yang memberikan review dalam 48 jam sejak check-out yang berlaku untuk 1 tahun depan. Review yang bertambah harapannya dapat menarik calon customer baru dan menjaga ex-customer kita juga agar melakukan booking kembali.

* Dengan asumsi gerakan ini berhasil berarti jumlah review se-minimalnya dapat bertambah satu(1) di setiap tempat penginapan kecuali yang availability_365 = 0 (karena berarti tidak dapat dibooking 1 tahun ke depan) dan akan mengalami **peningkatan revenue se-minimalnya 8,94%**.


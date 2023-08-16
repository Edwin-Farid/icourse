---
title: "Hal yang perlu di pelajari sebelum menjadi programming"
date: 2023-08-16T12:10:11+08:00
draft: false
---

## Pengantar

Dahulu untuk memindahkan suatu barang berat ke tempat lain diperlukan usaha
fisik yang berat pula. Problem ini menjadi lebih ringan dengan ditemukannya alat
yang bernama roda, di mana pengaplikasiannya memudahkan proses transportasi
pengangkutan barang. Dari dahulu sampai sekarang, memang manusia selalu mencari
cara untuk mempermudah pekerjaan mereka di segala bidang, baik di bidang
transportasi, pertanian, pendidikan, atau perekonomian. Perilaku inilah yang
mendorong manusia mampu berkembang seiring zaman.

Saat ini di abad ke 21, semuanya sudah serba mudah dengan bantuan alat yang
dinamakan komputer. Hanya dengan satu komputer, banyak sekali
kebutuhan-kebutuhan manusia yang bisa diselesaikan olehnya. Dulu untuk mengirim
pesan, kita harus memanfaatkan surat yang tentunya akan memakan waktu tergantung
dari jarak tujuan suratnya. Bandingkan dengan menggunakan komputer, untuk
mengirim pesan kita cukup meluangkan waktu untuk menulis dan kemudian kirim ke
alamat tujuan, tak hanya sampai 5 menit, pesan kita sudah bisa ke manapun tanpa
terhalang tembok yang bernama jarak.

Sama halnya dengan penemuan roda, ditemukannya roda adalah karena ada kebutuhan
pada aktivitas manusia, yang mendorong seseorang untuk berpikir kemudian mencari
solusi untuk kebutuhan tersebut. Begitu pula dengan kebutuhan di era yang serba
mudah saat ini, kebutuhan manusia bahkan bertambah berkali-kali lipat dari zaman
dahulu, alhasil banyak solusi-solusi mutakhir yang bahkan merevolusi perilaku
manusia secara utuh. Ambil saja misal internet dengan website-nya. Website
adalah bentuk solusi dari kebutuhan manusia, mulai dari kebutuhan transaksi
barang hingga interaksi manusia melewati media sosial.

Tak hanya website, sejak adanya smartphone muncul ribuan bahkan ratusan ribu
aplikasi yang bisa diakses melalui marketnya. Ada aplikasi kalkulator yang
mempermudah akses ke alat penghitung pada setiap saat, atau bahkan aplikasi dari
bank yang mampu melakukan transfer uang kapan pun dan di mana pun. Tapi apakah
aplikasi-aplikasi ini bisa muncul secara tiba-tiba di suatu market? Kalau tidak
tiba-tiba, bagaimanakah prosesnya? Atau mungkin, siapa sih yang membuat
aplikasi-aplikasi tersebut?

Tergantung dari aplikasi yang akan dibuat, pembuatan software bisa memakan waktu
dari beberapa minggu hingga tahunan. Aplikasi sederhana seperti kalkulator
mungkin cukup dibutuhkan 1-2 orang dengan waktu cukup singkat juga untuk
menyelesaikannya. Akan tetapi aplikasi kompleks seperti ojek online dengan
segala fiturnya, bisa membutuhkan ratusan orang dengan waktu berbulan-bulan.

Pembuatan aplikasi menjadi satu hal, akan tapi mengelolanya dengan melakukan
berbagai macam update sesuai kebutuhan pengguna, juga merupakan hal yang tak
kalah penting demi menjaga aplikasi tetap relevan dengan penggunanya.

Dalam dunia software development (pengembangan aplikasi), ada beberapa proses
yang bisa diikuti untuk membuat suatu aplikasi. Dimulai dari perencanaan hingga
ke pengelolaan, biasanya runtutan ini disebut dengan Software Development Life
Cycle (SDLC).

Berikut ilustrasinya prosesnya:

![SDLC](image/image.png)

- Planning: Perencanaan

- Analysis: Analisis

- Design: Desain

- Development: Pengembangan

- Testing: Pengujian

- Deployment : Penggelaran

- Maintenance: Pemeliharaan

Tiap-tiap proses dalam SDLC adalah penting, di mana setiap proses akan
memberikan dampak terhadap proses setelahnya. Misalnya jika kita melakukan
proses planning, analysis, dan design secara matang, maka proses implementasi
dan testing akan bisa dieksekusi secara lebih baik dan juga lancar.
Kebalikannya, jika proses implementasi dan testing tidak bisa dilakukan secara
baik, maka proses maintenance (pemeliharaan) akan mengalami banyak masalah.Dalam
pengembangan aplikasi, untuk mengetahui kebutuhan pengguna secara utuh, biasanya
dilakukan proses pembuatan dokumen User Requirements Specification (URS) atau
User Requirement Document (URD). Dokumen ini bukan bersifat teknis, melainkan
dibikin dengan format agar semua orang dapat membaca dan paham dengan gambaran
besarnya.

Tapi yang perlu diingat adalah kebutuhan pengguna sangatlah beragam yang
tentunya akan menjadi tantangan tersendiri dalam proses pengembangan aplikasi.
Dengan fakta beragamnya kebutuhan pengguna, maka akan menjadi mustahil untuk
membuat solusi aplikasi yang bisa memenuhi kebutuhan semua pengguna secara
sempurna. Pasti akan bertemu dengan titik di mana kita harus mengambil keputusan
dan akan muncul pertanyaan, “Apakah keputusan ini menguntungkan? Bukankah ini
akan merugikan kelompok tertentu?”. Hal ini sudah menjadi lazim dalam
pengembangan aplikasi, makanya banyak sekali opsi-opsi atau alternatif dalam
dunia aplikasi, misalnya ada dua aplikasi yang memiliki tujuan sama akan tetapi
fiturnya sangat berbeda.

Seperti yang kita tahu, User Requirement Specification diperlukan sebelum
mengembangkan aplikasi. Lalu pertanyaannya,

1. Apa saja yang harus diperhatikan ketika membuat User Requirement
   Specification (URS)?
2. Poin-poin penting apa saja yang tidak boleh terlewatkan ketika membuatnya?

Mari kita bahas.

URS dibuat supaya stakeholder (pemegang kepentingan) dapat memahami suatu
aplikasi yang ingin dibuat. Sehingga, ketika ada yang membaca dokumen ini,
mereka akan mendapat pemahaman yang sama dan mengurangi kesalahpahaman yang
terkadang membuat proses pengembangan menjadi terhambat.

Dalam pembuatan URS tidak boleh menggunakan jargon teknis yang hanya dipahami
oleh sekelompok orang saja. Misalnya, kita tidak boleh menggunakan istilah
encryption (enkripsi) karena mungkin hanya pengembang aplikasi di bidang
security (keamanan) saja yang mengetahui artinya.

Kemudian dalam pembuatan dokumen URS, penggunaan media seperti tabel atau
diagram sangat disarankan karena dapat mempermudah penyampaian pesan asli
terkait kebutuhan pengguna.

Lalu, bagaimana cara mendapatkan kebutuhan pengguna? Untuk menjawab pertanyaan
tersebut, kita perlu melakukan requirement gathering.

Requirement gathering adalah proses mendapatkan informasi dari para stakeholder
(pemegang kepentingan), seperti manajer, developer, customer, dan user. Teknik
yang dapat digunakan untuk requirement gathering, antara lain interview, user
stories, straw man documents, dan prototyping.

Oke, mari kita bahas satu per satu.

### Interview

Pertama adalah interview. Proses interview pada dasarnya merupakan proses tanya
jawab, di mana kita menanyakan suatu pertanyaan, kemudian dijawab oleh peserta
wawancara. Selain memberikan pertanyaan, kita juga perlu mencatat apa saja yang
disampaikan oleh peserta wawancara.

Bahkan tidak hanya dengan itu, interview juga bisa dilakukan dengan beberapa
cara.

- Cara pertama adalah Master-apprentice relationship.Cara ini merupakan proses
  transfer knowledge (transfer pengetahuan) dengan maksud mengajari suatu hal.
  Di sini seorang master (pengajar) dapat menanyakan beberapa hal sambil
  memberikan arahan kepada apprentice-nya (yang diajar).
- Kedua, kita dapat meminta seseorang untuk mengajarkan kepada kita apa yang
  mereka lakukan.
- Ketiga, kita dapat mengamati seseorang ketika melakukan suatu tugas. Sehingga,
  kita dapat mengetahui penyebab terhambatnya suatu proses atau bahkan faktor
  yang dapat membantu proses mereka menjadi lebih baik.

### User Stories

Selain menggunakan teknik interview, kita juga bisa menggunakan teknik User
Stories.

User stories digunakan sebagai kriteria dalam menentukan product acceptance atau
produk yang diinginkan. Selain itu, teknik ini juga dapat meningkatkan pemahaman
tentang produk yang kita buat. Sebab, melalui user stories, Anda dapat menemukan
berbagai kelebihan dan kekurangan dari suatu produk. Sehingga, Anda dapat
mengetahui bagian manakah yang harus diperbaiki.

User Stories dilakukan dengan menuliskan kebutuhan user sesuai dengan role dan
keinginannya. Contoh format penulisan user stories adalah sebagai berikut:

Sebagai seorang [deskripsi dari pengguna], Saya menginginkan [suatu
fungsionalitas], sehingga mendapatkan [suatu kemampuan atau fitur tertentu].

### Straw Man Documents

Teknik selanjutnya adalah Straw Man Documents. Teknik ini berguna untuk
menyampaikan ide dari aplikasi tanpa menuliskan kode program apa pun. Teknik
Straw Man Documents dapat dilakukan dengan berbagai macam media, misalnya
storyboards, flowcharts, dan mock-up html.

### Prototyping

Selanjutnya kita beralih ke teknik terakhir yaitu Prototyping. Teknik ini
merupakan proses pembuatan prototipe program yang terbatas pada fungsionalitas
utama saja. Dengan prototyping, kita bisa mendapatkan feedback yang lebih
lengkap karena stakeholder sudah bisa mencoba langsung dan mendapatkan gambaran
cara kerja aplikasi ketika sudah selesai nantinya. Namun, prototyping
membutuhkan biaya ekstra karena mau tidak mau kita harus membuat programnya
terlebih dahulu meskipun fungsionalitasnya terbatas. Selain itu, jika ada
feedback dari stakeholder yang bertolak belakang, akan menyebabkan keluarnya
biaya tambahan lagi untuk mengubahnya.

Nah, dengan adanya pembahasan materi tadi, diharapkan Anda dapat menerapkannya
untuk menentukan kebutuhan aplikasi dari sisi pengguna sebelum membuat sebuah
aplikasi. Tetap Semangat, ya!

## User Requirement Specification

Hai!

Supaya Anda lebih memahami tentang kebutuhan aplikasi dari sisi pengguna, mari
kita coba menerapkannya berdasarkan studi kasus tertentu. Contoh studi kasus
yang akan kita buat kali ini adalah User Requirement Specification terkait
proses login dan logout.

Pasti Anda sudah sering mendengar proses login dan logout, bukan? Proses login
dan logout sudah biasa digunakan dalam suatu aplikasi, sehingga banyak pengguna
akan familier dengan proses tersebut. Walaupun sudah umum digunakan dalam suatu
aplikasi, terkadang dalam proses implementasi login dan logout akan berbeda
antara aplikasi satu dengan aplikasi lainnya. Oleh karena itu, kita perlu
menentukan kebutuhan dari sisi pengguna terlebih dahulu.

Kali ini kita akan menggunakan teknik interview untuk mengumpulkan informasi
terkait kebutuhan aplikasi yang ditujukan untuk end-user atau calon pengguna
nantinya. Salah satu contoh pertanyaan yang dapat diajukan adalah sebagai
berikut:

"Apa yang sebenarnya diharapkan pengguna ketika melakukan proses login atau
logout?"

Setelah Anda menanyakan hal tersebut, bersiaplah untuk mencatat jawaban dari
pengguna. Anggap saja Anda memperoleh beberapa jawaban seperti berikut:

Di halaman login seharusnya pengguna bisa melakukan proses login dengan
memasukkan email dan password. Ketika pengguna melakukan proses logout, ia akan
secara otomatis pindah ke halaman login. Oke, kita telah berhasil mendapat 2
user requirements. Sehingga dari dua jawaban tersebut, kita bisa mengetahui
kebutuhan pengguna terkait proses login logout. Nah, setelah mengetahui user
requirement-nya, langkah apa yang selanjutnya dapat dilakukan?

Untuk mengetahui jawabannya, mari kita ke materi selanjutnya untuk mulai
membahas Spesifikasi Teknis Aplikasi.

Selamat belajar.

---
title: "Lotim Dev MeetUp 4"
date: 2023-04-08T11:37:32+08:00
draft: false

showTableOfContents : true
---

## Technical Feasibility : Sudaryatno as CTO at GITS Indonesia

Gits sebuah perusahaan yang berfokus dalam bidang perkembangan software.

Technical Feasibility adalah bagimana cara membuat produk secepat mungkin.

Hal yang perlu di lakukan sebelum membuat sebuah produk :

1. Memahami produknya terlebih dahulu 

Engineering Manager : Harus tau tujuan dari bisnis dan perusahaan.

Design Thinking : Mempermudah untuk membuat fitur apa yang dibutuhkan

1. Tentukan fitur prioritas (MVP - Minimum Valuable Product)
    
    Bisa berkomunikasi dengan tim untuk menentukan Minimum Valuable Product
    
2. List of Technology
    
    Memilih teknologi. Cara memilih dengan cara listing.
    
    Kemudian kategorikan : 
    
    Infrastructure
    
    Backend
    
    Database
    
    Frontend
    
    Mobile Apps
    
    Community Technology
    
- Maturity Community
- Great Documentation

1. Strong Team
    
    Kekuatan tim yang bisa :
    
    - Saling menginspirasi dan memandu
    - Melakukan perubahan yang cepat
    - Melakukan micromanaging

Setelah itu …

1. Choose Infrastructure
    
    Analisis sesuai dengan kemampuan
    
    - Server Side : Node JS
    - Platform : Microsoft, Firebase, ASW
        
        Lakukan perbandingan.
        

1. Choose Mobile Technology
    
    Memilih Flutter
    
    Tim jhony memutuskan :
    
    - Node JS
    - Firebase
    - Flutter
    

Timing Better than Perfect : Jangan terlalu sempurna, yang paling cepat itu paling baik.

1. Metrics
    
    EM harus mempunyai tolak ukur keberhasilan
    
    - Metrics Success Product
        - Quality : Load Testing, Performance Test, Test Coverage, Customer Feedback, Production Incidents. Customer feedback untuk melihat segimana kulitas produk kita.
        - Value : Berapa banyak customer yang make, segimana efisien biaya, jumlah transaksi
        - Productivity : Batch size, cycle time, number of commit. Standar yang benar adalah 1 hari 1 commit.
    
2. Analytic
    
    Harus tetap menganalisis 
    
3. Crash Tracker
    
    menganalisisi menggunakan
    
    - Firebase Crashlytics
    
4. User angagement
    
    Push notifications
    
    Email
    
5. Repeat

Engineering Manager : Role model dalam perusahaan yang memanfaatkan teknologi, soft skill dan hard skill. Goals untuk mencapai tujuan produk / perusahaan bersama dengan team.

ASK?

Bagaimana jika sudah produksi namun ketika sudah jalan, teknologi yang digunakan itu tidak efisien dan ingin merubah teknologi. Namun developernya hanya bisa menggunakan teknologi yang sebelumnya tidak dengan teknologi yang akan di update. Jadi apakah tetap menggunakan teknologi yang lama atau bagaimana?

Jawabannya :

Lakukan metrics yang detail untuk fitur atau app tersebut. Kemudian ketika ingin upgrade. Developer juga perlu belajar technology apa yang ingin di upgrade.

Technology itu adalah tools bukan job desk.

## Increase App Performance with Flutter Isolate : Nasrul Alawy as Lead Mobile Dev

Biasa perusahaan menggunakan flutter untuk mempres cost application.

Flutter : asynchrony = Membaca codingan dari atas sampai bwah.

Bekerja dengan event loop. Meskipun tidak ada aktifitas, flutter akan terus melakukan looping.

Ketika melakukan perhitungan kompleks akan terjadi mengalag. Jadi itu fungsinya isolate.

Kalau ingin memblock error mengguakan “await”.

Sistem :

- Open
- Idle
- Click Button
- Req API
- etc

- Flutter Isolate : Membuat isolasi terpisah. Ketika ada sebuah event yang berat kita akan mengisolasinya, dengan proses sendiri. Memiliki ruang khusus yang di kirim melalui port.

Fungsi : 

- Memperbaiki performa aplikasi dengan menjalankan kode secara paralel.
- Membagi beban kerja di antara core CPU
- Menjalan kode yang memerlukan lingkungan yang aman
- Meningkatkan stabilitas apps

Kekurangan :

- Codingan makin lebih kompleks : Cost pertambah
- Tidak semua function di jadikan isolate

ASK:
Karena tadi tidak semua function bisa kita lakukan isolate. Bagaimana cara menentukan function yang akan di isolate?

## Fuzzing The Rest : Rahmat Wahyu Hadi

Critical bugs biasa menemukan 3 dari 10 bug critical.

1. Apa itu debugging
    
    Mendefinisikan untuk mencari problem pada code.
    
2. Apa itu fuzzing
    
    menginput secara automate software dengan inputan yang tidak di sangka.
    
    pyload : apa yang dikirim dari user ke backend.
    
3. Traditional Fuzzing
    
    Breaking things with randoms input. Melakukan testing menggunakan inputan random.
    
4. Modern Fuzing
    
    Payloadnya sudah terstruktur. Tingkat efisiensi mencari bug sangat tinggi. Semakin kompleks payload makan semakin tinggi tingkat keberhasilan mencari bug. 
    

Sebelum melakukan payload harus mendefinisikan payloadnya. 

Apa yang bisa di fuzzing?

Semua yang ada inputan dan output.

Logger sangat penting dalam fuzzing  : apa yang kita input dan output kita simpan dari hasil fuzzing. Agar bisa menganalisis masalah

Tools : bugsmith

Langkah-langkah :

1. Menganalisis inputan atau parameter
2. Membuat payload
3. Paste pada bugsmith
4. Kita lihat requestnya. (anomali)
5. Lakukan eksploitas
6. Decrypt requestnya

Automade Testing :

1. Login pake email random dan password random
2. Mengenerate untuk melakukan fuzzing
3. melakukan fuzzing mengunakan nucklei
4. elastic search untuk logging
5. data elastic di simpan 
6. melakukan eksploitasi

Step :

1. Fuzzing
2. Debugging
3. Eksploitasi

- direction
- rest condition

## Agile Product Management : Ray Rizaldy as CEO Gits

Kebanyakan konsep bisa membuat nggk perfek”.

Proses pengembangan produk

- Build
- Measure
- Learn

Agile : Kita bisa mendevelop sesuatu secepat mungkin.

Pada customer

VUCA : Harus bisa di jawab dengan prediksi, jadi kita berbicara tentang estimasi.

- Volatillity : ukuran harga
- Uncertanity : ukuran ketidak pastian
- Ambiguity : ukuran ambigu dari suatu produk
- Complexity : ukuran dari kerumitan dari sebuah produk

Dimensi dalam bidang developer : Hal yang mempengaruhi development

1. Product : Banyak product yang nggk jalan
2. People : Banyak pemikiran
3. Technology : Bingung memilih teknologi
4. Process : Bentrok memilih proses

User Story :

As a <role>

I want <goals>

so that <benefit>

 Step :

- Card : Requitmen on strory card
- Conversation : Discuss all details in the team
- Confirmation : Define acceptance criteria for when a story is done

Tips : 

- Pindahkan card bukan ketika sudah selesai, namun ketika ingin dikerjakan.
- Informasikan kepada tim apa yang sedang di kerjakan

Project Manager tree : 

- To do
- In Progres
- Complete
- Backlog

Tools : Gunakan 1 tools 

- Taiga
- Trelo
- Hasana

Estimasi : Bandingkan relatif ambil yang paling lambat. Harus dicatat.

## Run Your Back End App Using Cloud Run  : Ibnu Sina Wardy as Google Developer Expert Cloud

Speed is important

1. Serverless vs Traditional Architecture
    
    

Servless :

- Google Cloud Run : Deploy server apapun yang di manage oleh google.

Keuntungan :

- No server to manage
- Focus on writing code
- Scale up fast
- Scale down to zero
- pay for exact usage
- just deploy
- any staless container : Kirim code ke server lain. Jangan di tempat publish. Aman untuk menghapus aplikasi dan memindahkan data. Memisahkan data.
- any language any library
- url in second

Cloud Run Servis : Bisa gratis

Kalkulator : Google Cloud Pricing Calculator

Cloud Run Jobs :

Step :

- Build pake docker
- Upload ke google
- Deploy faster, so we can test it on production

Cara Deploy :

1. Docker.file untuk resepnya : Harus paham dockerizing or docker.file
    1. copy file json
    2. tentukan home atau tempat installnya
    3. jalankan npm install
    4. copy semua source code
2. gcloud run deploy : 
    1. otomatis switch jika ada update version application

VCC

## Build CI/CD with GitLab : Didiet Agus Pambudiono as Lead DevOps Gits

Apa itu Continuous Integration (CI)?

- Developers commit code to a shared repository on a refular basis.
- Version control system is being monitored. When a commit is detected, a build will be triggered automatically.
- If the build is not green (gagal), developers will be notified immediately (maka akan ada pemberitahuan).

Kenapa ktia butuh Continuoues Integration ?

- Mendeteksi bug dan bisa dengan mudah kita deteksi lebih awal.

Development before CI :

- Release manually = semua dirilis secara manual
- Test happens late = rilis tidak secepat secara otomation
- Few releases

Publish :

Development

Staging

Production

Vibernate

Gitlabs CI, DevOps bisa memberitahu WA untuk mengetes server.

- Delivery team
- Version Control
- Build
- Automated
- User Approve
- Release

1. Continuous Integration
2. Continuous Delivery
3. Continuous Deployment

Cara mengimplimintasi CI

- Non hosted solutions
    - jenkins
    - gitlab CE
    - Teamcity
- Hosted Solutions
    - Circle

Kenapa Gitlab CI/CD

- Integrated : Bisa digunakan gratis
- Easy to learn : Mudah untuk memulai
- Beautiful : Familiar, mudah digunakan
- Scalable : Bisa digunakan di mesin manapun
- Faster results : Buildnya bisa di split multiple jobs
- Open source :

Fitur :

- Multi Platform
- Multi language : Java, PHP, Ruby, C, etc
- Parallel build : Split build in pararel
- Docker support
- Pipeline
    - Editor
    - Jobs :
        - Build
        - Deploy
- Build arifacts
- Container Registry
- Environments
- Autoscaling
- Real Time logging
- Versioned test

Monorepo : 2 aplikasi menggunakan 1 component
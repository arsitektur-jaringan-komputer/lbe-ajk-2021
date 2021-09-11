# Web Deploy

## **CONTENTS**
* [**Deploy**](#deploy)
* [**LEMP**](#lemp)
* [**Laravel**](#laravel)
* [**SSL**](#ssl)
* [**DNS**](#dns)
* [**Link Materi Praktik**](#link-materi-praktik)
* [**Referensi**](#referensi)

## Deploy
Deploy adalah sebuah istilah untuk mengembangkan website atau aplikasi. Contoh, untuk aplikasi bisa deploy ke playstore dan website bisa deploy ke hosting server.  
![how-does-a-web-server-work](https://user-images.githubusercontent.com/55046884/132818456-febb87bd-a5bc-4b0f-b361-8df9fb7a65a1.jpg)  

## LEMP
**LEMP** adalah singkatan dari Linux, Nginx (web server), MySQL (database server), dan PHP. **Web server** adalah sebuah software (perangkat lunak) yang memberikan layanan berupa data. Berfungsi untuk menerima permintaan HTTP atau HTTPS dari klien atau kita kenal dengan web browser (Chrome, Firefox). Selanjutnya ia akan mengirimkan respon atas permintaan tersebut kepada client dalam bentuk halaman web. **Database Server** adalah sebuah software (perangkat lunak) untuk menyimpan dan mengelola data dari website kita. Sedangkan **PHP** sendiri berperan sebagai mengenerate website ke dalam bentuk website dinamis artinya bisa berinteraksi dengan user.  

## Laravel
Laravel adalah salah satu framework PHP yang paling populer dan paling banyak digunakan di seluruh dunia dalam membangun aplikasi web mulai dari proyek kecil hingga besar. Dalam 
materi deploy kali ini projek laravel bisa dilihat di https://gitlab.com/kuuhaku86/web-penugasan-individu. Laravel memiliki tools yang menjadi andalannya, tools tersebut adalah **composer** dan **artisan**. Composer merupakan tool yang di dalamnya terdapat dependencies dan kumpulan library. Seluruh dependencies disimpan menggunakan format file composer.json sehingga dapat ditempatkan di dalam folder utama website. Oleh karena itu composer dikenal dengan dependencies management. Sedangkan Artisan merupakan command line interface yang dimiliki oleh Laravel. Artisan mencakup sekumpulan perintah yang membantu Anda untuk membangun sebuah website atau aplikasi web.  

## SSL
![http-vs-https](https://user-images.githubusercontent.com/55046884/132826325-24d51f16-40bc-4a2f-9463-41b240ce47ec.png)  
SSL adalah singkatan dari Secure Socket Layer, salah satu komponen penting yang harus dimiliki website. Dengan SSL, transfer data di dalam website menjadi lebih aman dan terenkripsi. Apabila sistem keamanan ini ditambahkan pada website Anda, maka URL website akan berubah menjadi HTTPS. Tujuan utama pemasangan SSL adalah sebagai pengaman pertukaran data yang terjadi melalui jaringan internet.  
Salah satu layanan gratis untuk mendapatkan sertifikat ssl pada website adalah https://letsencrypt.org/id/ . Layanan tersebut cukup mudah diimplementasikan dan bisa diterapkan di berbagai jenis server, termasuk juga linux server.  

## DNS
DNS adalah sebuah sistem yang mengubah URL website ke dalam bentuk IP Address. Tanpa DNS, Anda harus mengetikkan IP Address secara lengkap ketika ingin mengunjungi sebuah website.  
  
![DNS_schema-768x427](https://user-images.githubusercontent.com/55046884/132827882-240196d3-10b9-46c7-8642-822c583a23b6.png)  
* **Root-Level Domain** merupakan bagian tertinggi dari hirarki DNS. Biasanya ia berwujud tanda titik (.) di bagian paling belakang sebuah URL.  
* **Top-Level Domain** adalah ekstensi yang berada di bagian depan root-level domain. contoh pada gambar adalah org.  
* **Second-Level Domain** ialah nama lain untuk domain itu sendiri. Ia sering digunakan sebagai identitas institusi atau branding. Dalam kasus URL en.wikipedia.org, yang dimaksud SLD adalah wikipedia.  
* **Third-Level Domain atau subdomain** merupakan bagian dari domain utama yang berdiri sendiri. Apabila domain diibaratkan sebagai rumah, subdomain adalah salah satu  ruang khusus di rumah itu sendiri. contoh pada gambar adalah en  
* **Hostname** atau bisa disebut juga dengan scheme. Ini merupakan bagian yang mengawali sebuah URL. Bagian ini menunjukkan sebuah fungsi dari sebuah website atau halamannya. Contoh paling banyak digunakan, yaitu HTTPS atau Hypertext Transfer Protocol Secure.  

## Referensi
https://umbraco.com/knowledge-base/deployment/  
https://www.dicoding.com/blog/apa-itu-web-server-dan-fungsinya/#:~:text=Web%20server%20adalah%20sebuah%20software,client%20dalam%20bentuk%20halaman%20web.  
https://www.dewaweb.com/blog/lamp-atau-lemp-manakah-yang-lebih-baik/  
https://www.niagahoster.co.id/blog/laravel-adalah/  
https://www.jagoanhosting.com/blog/framework-laravel/  
https://www.hostinger.co.id/tutorial/apa-itu-ssl  
https://www.niagahoster.co.id/blog/apa-itu-dns/?amp

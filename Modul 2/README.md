# Materi
1. [OSI Layer](#osi-layer)
2. 

# OSI Layer
## Apa itu OSI Layer?

Biasa disebut sebagai OSI Layer Model. OSI merupakan singkatan dari Open System Interconnection. Standar ini dikembangkan oleh ISO – ‘International Organization of Standardization‘ - pada tahun 1984. OSI model merupakan sebuah konsep yang menggambarkan fungsi jaringan dan sistem telekomunikasi. Model lapisan ini yang nantinya harus dilewati oleh paket data. Proses transmisi melewati OSI layer ini terjadi setiap kali paket data akan ditransmisikan, baik itu transmisi paket data dari server, serta transmisi paket data menuju client.

## Fungsi?

Model ini membantu memberikan deskripsi visual tentang apa yang terjadis dengan sistem jaringan tertentu. Ini dapat membantu manajer jaringan mempersempit masalah (Apakah itu masalah fisik atau sesuatu dengan aplikasi?), serta pemrogram komputer (ketika mengembangkan aplikasi, lapisan lain mana yang perlu dikerjakan?). Vendor teknologi yang menjual produk baru akan sering merujuk ke model OSI untuk membantu pelanggan memahami lapisan mana yang berfungsi dengan produk mereka atau apakah itu berfungsi "di seluruh tumpukan".

Ketika sebuah perangkat dalam jaringan komputer mengirimkan data ke perangkat lain, maka data tersebut akan mengalir mulai dari layer 7 ke layer 1.

![image](https://user-images.githubusercontent.com/75016595/131870451-2482b441-031d-4300-8ca2-d9f0e43c9fac.png)

## Layer 7 - Application

Application Layer merupakan lapisan pertama pada saat sebuah data mulai ditransfer, dan merupakan lapisan terakhir yang dilewati ketika komputer client menerima data tersebut. Pada layer ini terjadi interaksi antarmuka antara pengguna (end user) dengan aplikasi yang bekerja menggunakan fungsionalitas sebuah jaringan. Layer ini menerima informasi langsung dari pengguna (lain) dan menampilkan data yang masuk ke pengguna (kita), melakukan pengaturan bagaimana aplikasi bekerja menggunakan resource jaringan, kemudian dapat memberikan pesaan jika terjadi sebuah kesalahan pada proses pengaturan jaringan.

Ada beberapa protocol yang ditempatkan pada lapisan application layer ini, yaitu :

- HTTP
- SMTP
- NFS

## Layer 6 - Presentation

Presentation Layer mewakili area yang tidak bergantung pada representasi data Application layer. Secara umum merepresentasikan penyusunan atau penerjemahan (mentranslate) format data yang hendak ditransmisikan oleh aplikasi melalui jaringan ke dalam format yang bisa ditransmisikan oleh jaringan, atau dari format jaringan ke format aplikasi. Dalam artian, layer ini menyajikan data untuk aplikasi atau jaringan. Salah satu contohnya adalah enkripsi dan dekripsi data untuk secure transmission.

Beberapa protocol pada Presentation Layer :

- Redirectopr software
- Virtual Network Computing
- Remote Desktop Protocol

## Layer 5 - Session

Ketika dua perangkat komputer atau server perlu berbicara satu sama lain, maka perlu dibuat session. Tanggung jawab dari Session Layer adalah mengendalikan sesi koneksi dialog dan juga mengelola atau memutuskan koneksi dari komputer. Fungsi pada lapisan ini melibatkan pengaturan, koordinasi (misalnya berapa lama sistem harus menunggu respons) dan penghentian antara aplikasi di setiap akhir sesi.

## Layer 4 – Transport

Transport Layer merupakan lapisan yang memiliki tugas sebagai pengantar. Transport Layer berkaitan dengan koordinasi transfer data antara end systems dan host. Berapa banyak data yang akan dikirim, berapa kecepatannya, kemana perginya, dll. Contoh paling terkenal dari Transport Layer adalah Transmission Control Protocol (TCP), yang dibangun di atas Internet Protocol (IP), umumnya dikenal sebagai TCP/IP. Nomor port TCP dan UDP bekerja di Layer 4, sedangkan alamat IP bekerja di Layer 3, Network Layer.

Fungsi utama dari Transport Layer :

- Memotong data menjadi potongan yang lebih kecil
- Mentransmisikan data dari session layer menuju network layer, maupun sebaliknya.
- Membuat penomoran (sequence number) pada potongan data
- Melakukan proses transmisi ulang pada potongan data yang hilang

Potongan data yang leih kecil dan telah diberikan sequence number, potongan tersebut dikenal dengan nama _segments_.

## Layer 3 - Network

Network Layer bertanggung jawab dalam mendefinisikan alamat IP (Internet Protocol). Baik alamat IP pengirim maupun tujuan. Hal ini membuat setiap komputer agar dapat terhubung didalam 1 jaringan. Fungsi dari beberapa hardware jaringan seperti router dan juga hub berjalan pada layer ini, berfungsi untuk melakukan proses routing serta membuat header pada segments yang ada. Ketika segments sudah diberi header. Nama nya berubah menjadi _packets_.

## Layer 2 – Data Link

Data Link Layer menyediakan transfer data node-to-node (antara dua node yang terhubung langsung), menangani koreksi kesalahan dari Physical Layer, flow control, dan menetukan bagaimana perangkat-perangkat jaringan seperti hub, bridge, repeater, dan switch dapat beroperasi.

Layer ini merupakan layer yang paling kompleks diantara layer lainnya. Karna pada layer ini terdapat 2 sublayer yaitu MAC (Media Access Control) dan juga LLC (Logical Link Control). Tugas dari MAC adalah mengendalikan perangkat dari suatu jaringan yang mendapat akses ke medium dan juga izin ketika melakukan transmisi data. Sedangkan LLC sendiri bertugas mengidentifikasi kemudian membungkus protokol network layer dan juga melakukan kontrol terhadap koreksi kesalahan.

Pada layer ini pula, _packets_ akan dilengkapi dengan beberapa informasi tambahan kembali, dan naamnya berubah menjadi _frames_

## Layer 1 - Physical

Physical layer mewakili representasi listrik dan fisik dari sebuah sistem. Ini mencakup semuanya mulai dari jenis kabel, topologi, frekuensi radio (seperti dalam sistem nirkabel 802.11), serta tata letak pin, voltase, dan persyaratan fisik lainnya. Kketika masalah jaringan terjadi, banyak profesional jaringan langsung ke lapisan fisik untuk memeriksa apakah semua kabel terhubung dengan benar dan steker listrik belum ditarik dari router, sakelar, atau komputer.

Pada layer ini, setiap frames akan diubah menjadi bits. Bits inilah yang akan dikirim ke endpoint yang lain dalam jaringan.

![osi_layer_2_LI](https://user-images.githubusercontent.com/75016595/132080044-488a3c1d-2b88-4dc6-b182-66a6b08c5511.jpg)

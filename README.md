# Jarkom-Modul-5-IT32-2024

##### Praktikum Jaringan Komputer Modul 5 Tahun 2024

### Anggota Kelompok
| Nama | NRP |
|---------|---------|
| Muhammad Kenas Galeno Putra | 5027231069   |
| Veri Rahman | 5027231088   |

# Laporan Resmi

# Daftar Isi
- [Misi 1: Memetakan Kota NewEridu](#no-1)
  - [No 1](#no-1)
  - [No 2](#no-2)
  - [No 3](#no-3)
  - [No 4](#no-4)
- [Misi 2: Menemukan Jejak Sang Peretas](#no-20)
  - [no-1](#no21)
  - [no-2](#no22)
  - [no-3](#no23)
  - [no-4](#no24)
  - [no-5](#no25)
  - [no-6](#no26)
  - [no-7](#no27)
  - [no-8](#no28)
  - [Misi 3: Menangkap Burnice](#no-30)

### Prefix IP
Kelompok kami memiliki prefix IP *10.79*

## Misi 1: Memetakan Kota NewEridu
### No 1
<a name="no-1"></a>
Soal:
    **Sebuah topologi sederhana menggambarkan jaringan New Eridu:**
    <img src="img/topo-soal.png">
    Keterangan:
      HDD: Berfungsi sebagai DNS Server.
      Fairy: Berfungsi sebagai DHCP Server.
      Web Servers: HIA, HollowZero.
    Client:
      Burnice: Memiliki 5 host.
      Lycaon: Memiliki 20 host.
      Policeboo: Memiliki 30 host.
      Caesar: Memiliki 50 host
      Ellen: Memiliki 100 host.
      Jane: Memiliki 200 host.

 Berikut topologi jaringan pada GNS3 seperti yang diberikan soal:
 <img src="img/topo-it32.png">

### No 2
<a name="no-2"></a>
Soal:
    **Setelah membagi alamat IP menggunakan VLSM, gambarkan pohon subnet yang menunjukkan hierarki pembagian IP di jaringan New Eridu. Lingkari subnet-subnet yang akan dilewati dalam jaringan.**
Berikut adalah tabel routing, tabel pembagian IP VLSM, dan tree VLSM.

#### Tabel Routing:
<img src="img/routing-vlsm.png">

#### Tabel Pembagian IP VLSM:
<img src="img/ip-vlsm.png">

#### Tree VLSM:
<img src="img/Treemodul5.png">

Untuk topologi jaringan pada GNS3 dengan lingkaran pembagian IP VLSM adalah sebagai berikut.
<img src="img/topo-vlsm.png">

### No 3
<a name="no-3"></a>
Soal:
Setelah pembagian IP selesai, buatlah konfigurasi rute untuk menghubungkan semua subnet dengan benar di jaringan New Eridu. Pastikan perangkat dapat saling terhubung.

### No 4
<a name="no-4"></a>
Soal:


## Misi 2: Menemukan Jejak Sang Peretas
<a name="no-20"></a>
### No 1
<a name="no-21"></a>
Soal: 
Agar jaringan di New Eridu bisa terhubung ke luar (internet), kalian perlu mengkonfigurasi routing menggunakan iptables. Namun, kalian tidak diperbolehkan menggunakan MASQUERADE.

### No 2
<a name="no-22"></a>
Soal:
Karena Fairy adalah AI yang sangat berharga, kalian perlu memastikan bahwa tidak ada perangkat lain yang bisa melakukan ping ke Fairy. Tapi Fairy tetap dapat mengakses seluruh perangkat.

### No 3
<a name="no-23"></a>
Soal:
Selain itu, agar kejadian sebelumnya tidak terulang, hanya Fairy yang dapat mengakses HDD. Gunakan nc (netcat) untuk memastikan akses ini. [hapus aturan iptables setelah pengujian selesai agar internet tetap dapat diakses.]

### No 4
<a name="no-24"></a>
Soal:
Fairy mendeteksi aktivitas mencurigakan di server Hollow. Namun, berdasarkan peraturan polisi New Eridu, Hollow hanya boleh diakses pada hari Senin hingga Jumat dan hanya oleh faksi SoC (Burnice & Caesar) dan PubSec (Jane & Policeboo). Karena hari ini hari Sabtu, mereka harus menunggu hingga hari Senin. Gunakan curl untuk memastikan akses ini.

### No 5
<a name="no-25"></a>
Soal:
Sembari menunggu, Fairy menyarankan Phaethon untuk berlatih di server HIA dan meminta bantuan dari faksi Victoria (Ellen & Lycaon) dan PubSec. Akses HIA hanya diperbolehkan untuk
a. Ellen dan Lycaon pada jam 08.00-21.00.
b. Jane dan Policeboo pada jam 03.00-23.00. (hak kepolisian)
Gunakan Curl untuk memastikan akses ini.

### No 6
<a name="no-26"></a>
Soal:
Sebagai bagian dari pelatihan, PubSec diminta memperketat keamanan jaringan di server HIA. Jane dan Policeboo melakukan simulasi port scan menggunakan nmap pada rentang port 1-100.
a. Web server harus memblokir aktivitas scan port yang melebihi 25 port secara otomatis dalam rentang waktu 10 detik.
b. Penyerang yang terblokir tidak dapat melakukan ping, nc, atau curl ke HIA.
c. Catat log dari iptables untuk keperluan analisis dan dokumentasikan dalam format PDF.

### No 7
<a name="no-27"></a>
Soal:
Hari Senin tiba, dan Fairy menyarankan membatasi akses ke server Hollow. Akses ke Hollow hanya boleh berasal dari 2 koneksi aktif dari 2 IP yang berbeda dalam waktu bersamaan. Burnice, Caesar, Jane, dan Policeboo diminta melakukan uji coba menggunakan curl.

### No 8
<a name="no-28"></a>
Soal:
Selama uji coba, Fairy mendeteksi aktivitas mencurigakan dari Burnice. Setiap paket yang dikirim Fairy ke Burnice ternyata dialihkan ke HollowZero. Gunakan nc untuk memastikan alur pengalihan ini.

## Misi 3: Menangkap Burnice
<a name="no-30"></a>

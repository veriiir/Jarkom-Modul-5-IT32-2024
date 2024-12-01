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
- [Perhitungan VLSM](#perhitungan-vlsm)
- [VLSM Tree](#vlsm-tree)
- [Config dan Routing](#config-vlsm)

### Prefix IP
Kelompok kami memiliki prefix IP *10.79*

## Misi 1: Memetakan Kota NewEridu
### No 1
<a name="no-1"></a>
Soal:
    **Sebuah topologi sederhana menggambarkan jaringan New Eridu:**
    <img src="img/topo-soal.png">
    **Keterangan:
    - HDD: Berfungsi sebagai DNS Server.
    - Fairy: Berfungsi sebagai DHCP Server.
    - Web Servers: HIA, HollowZero.
    - Client:
      - Burnice: Memiliki 5 host.
      - Lycaon: Memiliki 20 host.
      - Policeboo: Memiliki 30 host.
      - Caesar: Memiliki 50 host
      - Ellen: Memiliki 100 host.
      - Jane: Memiliki 200 host.**
 Berikut topologi jaringan pada GNS3 seperti yang diberikan soal:
 <img src="img/topo-it32.png">

### No 2
<a name="no-2"></a>
Soal:
    **Setelah membagi alamat IP menggunakan VLSM, gambarkan pohon subnet yang menunjukkan hierarki pembagian IP di jaringan New Eridu. Lingkari subnet-subnet yang akan dilewati dalam jaringan.**
Berikut adalah tabel routing, tabel pembagian IP VLSM, dan tree VLSM.
Tabel Routing:
<img src="img/topo-it32.png">
Tabel Pembagian IP VLSM:
<img src="img/topo-it32.png">
Tree VLSM:
<img src="img/topo-it32.png">
Untuk topologi jaringan pada GNS3 dengan lingkaran pembagian IP VLSM adalah sebagai berikut.
<img src="img/topo-it32.png">
    
## Misi 2: Menemukan Jejak Sang Peretas
<a name="perhitungan-cidr"></a>
### Pengabungan
Cara :
1. Kelompokkan dari node terjauh dari awan. Hitung router terjauh
2. Gabungkan lagi dari yang sudah dikelompokkan sebelumnya

## Misi 3: Menangkap Burnice

# Portofolio Keamanan Siber oleh Ramdhani – Kelas 6D MAK, 2025

**Nama**: Ramdhani  
**Kelas**: 6D MAK  
**Asal Sekolah**: Darunnajah  
**Tahun**: 2025  
**GitHub**: [https://github.com/acongkuy](https://github.com/acongkuy)  
**HackerOne**: [https://hackerone.com/chunsky](https://hackerone.com/chunsky)

---

## 1. Pendahuluan

Saya adalah siswa kelas 6D MAK di Darunnajah yang memiliki minat dalam bidang keamanan siber. Sejak tahun 2025, saya mulai aktif melakukan eksplorasi, pengujian, dan pelaporan kerentanan keamanan baik di platform internasional seperti HackerOne maupun secara langsung ke instansi sekolah saya. Portofolio ini merangkum pengalaman dan kontribusi saya dalam praktik keamanan siber selama tahun 2025.

---

## 2. Bug Bounty di HackerOne

Saya berpartisipasi dalam program bug bounty di platform **HackerOne** untuk mengasah kemampuan teknis dan pemahaman saya terhadap kerentanan keamanan aplikasi.

**Ringkasan laporan**:
- Total laporan: 5
  - **1 valid**
  - **1 duplicate/late**
  - **3 not applicable**

**Jenis kerentanan yang pernah saya laporkan**:
- Allocation of Resources Without Limits or Throttling (CWE-770)
- UI Redressing / Clickjacking (CAPEC-103)
- Cleartext Transmission of Sensitive Information (CWE-319)

🔗 **Profil HackerOne saya**: [https://hackerone.com/chunsky](https://hackerone.com/chunsky)

---

## 3. Audit dan Pelaporan Keamanan di Lingkungan Sekolah

### 3.1 Audit Website darunnajah.ac.id Berdasarkan Model OSI Layer

Saya melakukan analisis keamanan terhadap website resmi sekolah saya, **darunnajah.ac.id**, dengan pendekatan OSI Layer menggunakan berbagai tools open-source.

**Layer 7 – Application Layer**  
- Tidak terdapat header `X-Frame-Options` dan `X-Content-Type-Options`.  
  → Potensi risiko: clickjacking dan content-type sniffing.  
- HTTP redirect dari http ke https terdeteksi.

**Layer 6 – Presentation Layer**  
- Website mendukung TLS 1.2 dan 1.3 dengan cipher yang kuat.  
- Tidak ditemukan kerentanan renegotiation maupun Heartbleed.

**Layer 4 – Transport Layer**  
- Port 80 dan 443 terbuka.  
- Mendukung HTTP/2 dan HTTP/3.

**Layer 3 – Network Layer**  
- Akses stabil via IPv6, tanpa packet loss.  
- Terhubung melalui rute internasional via Cloudflare.

### 3.2 Laporan Keamanan ke Pihak Sekolah

Saya telah secara langsung mengirimkan laporan kerentanan kepada pihak sekolah Darunnajah, di antaranya:

- **Clickjacking** pada website darunnajah.ac.id
- **Allocation of Resources Without Limits or Throttling (CWE-770)**

📎 Laporan dikirim dalam bentuk PDF dan dapat dilihat melalui repositori GitHub saya.

---

## 4. Tools yang Digunakan

Dalam melakukan pengujian dan audit, saya menggunakan beberapa tools berikut:

- **Nikto** – Pemindaian aplikasi web
- **Nmap** – Port dan network scanning
- **Rapidscan** – Pemindaian kerentanan otomatis
- **Subfinder** – Deteksi subdomain
- **Slowloris** – Simulasi serangan DoS
- **Ping**, **Traceroute**, **Curl**, **Sslyze** – Analisis jaringan dan TLS

---

## 5. Penutup

Portofolio ini menggambarkan kontribusi awal saya dalam dunia keamanan siber. Saya percaya bahwa dengan terus belajar dan berkontribusi, saya dapat berkembang menjadi individu yang mampu memberikan dampak positif dalam bidang ini, baik secara lokal maupun global.

---


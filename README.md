# 🛡️ Portofolio Keamanan Siber: Penelitian dan Pengujian Aplikasi Web

**Nama:** Ramdhani  
**Kelas:** 6D MAK  
**Asal Sekolah:** Darunnajah  
**Tahun:** 2025  
**GitHub:** [@acongkuy](https://github.com/acongkuy)  
**HackerOne:** [@chunsky](https://hackerone.com/chunsky)  
**LinkedIn:** [acong-walnut](https://www.linkedin.com/in/acong-walnut-a88207363)

---

## 1. 📘 Pendahuluan

Saya adalah siswa kelas 6D MAK di Darunnajah dengan minat besar pada **keamanan siber**. Sejak tahun 2025, saya aktif dalam eksplorasi, pengujian, dan pelaporan kerentanan keamanan, baik melalui platform bug bounty internasional seperti **HackerOne**, maupun secara langsung kepada pihak sekolah.  

Portofolio ini merangkum pengalaman, temuan, serta kontribusi saya dalam praktik keamanan siber selama tahun 2025.

---

## 2. 🐞 Bug Bounty di HackerOne

Saya aktif berpartisipasi dalam program **bug bounty di HackerOne** untuk meningkatkan kemampuan teknis dan memahami berbagai jenis kerentanan.

### 📊 Ringkasan Laporan:
- **Total laporan:** 8  
  - ✅ 1 valid-resolved  
  - ♻️ 2 duplicate/late  
  - 🚫 3 not applicable  
  - ⏳ 2 under review

### 📌 Jenis Kerentanan yang Pernah Dilaporkan:
- Allocation of Resources Without Limits or Throttling (CWE-770)  
- UI Redressing / Clickjacking (CAPEC-103)  
- Cleartext Transmission of Sensitive Information (CWE-319)  
- Cross-site Scripting (XSS) – Reflected / Stored / DOM (CWE-79)  
- Improper Authorization in Handler for Custom URL Scheme (CWE-939)

📍 **Profil HackerOne:** [https://hackerone.com/chunsky](https://hackerone.com/chunsky)

---

## 3. 🔍 Audit dan Pelaporan Keamanan di Lingkungan Sekolah

### 3.1 🔬 Audit Website darunnajah.ac.id Berdasarkan Model OSI Layer

#### Layer 7 – Application Layer
- ❌ Tidak terdapat header `X-Frame-Options` dan `X-Content-Type-Options` → **Potensi risiko: clickjacking & content-type sniffing**
- 🔁 HTTP redirect dari `http` ke `https` terdeteksi

#### Layer 6 – Presentation Layer
- ✅ Mendukung TLS 1.2 dan 1.3 dengan cipher kuat
- 🛡️ Tidak ditemukan Heartbleed maupun masalah renegotiation

#### Layer 4 – Transport Layer
- 🔓 Port 80 dan 443 terbuka
- 🚀 Mendukung HTTP/2 dan HTTP/3

#### Layer 3 – Network Layer
- 📶 Stabil via IPv6, tanpa packet loss
- 🌐 Routing melalui Cloudflare internasional

### 3.2 📩 Laporan Keamanan ke Pihak Sekolah

Saya telah mengirimkan laporan kerentanan berikut ke pihak sekolah:

- ⚠️ Clickjacking pada website Darunnajah  
- ⚠️ Allocation of Resources Without Limits or Throttling (CWE-770)

📁 Semua laporan lengkap tersedia di repositori ini:  
🔗 [GitHub Repo: cybersecurity-portfolio](https://github.com/acongkuy/cybersecurity-portfolio)

---

## 4. 🧰 Tools yang Digunakan

Berikut tools yang saya gunakan dalam aktivitas pengujian dan audit keamanan:

- **Burp Suite** – Web vulnerability testing  
- **Nikto** – Web server scanner  
- **Nmap** – Port & network scanning  
- **Rapidscan** – Otomatisasi scanning  
- **Subfinder** – Subdomain enumeration  
- **Slowloris** – DoS simulation  
- **Ping, Traceroute, Curl, Sslyze** – Network & TLS analysis  
- **Amass** – Subdomain enumeration  
- **XSStrike** – XSS payload automation  
- DLL

---

## 5. 🧾 Penutup

Portofolio ini merupakan dokumentasi awal dari perjalanan saya di dunia **cybersecurity**. Saya percaya bahwa dengan terus belajar, bereksperimen, dan berbagi temuan, saya bisa berkontribusi secara positif dalam menjaga keamanan informasi—baik di tingkat lokal maupun global.

---

> 🔐 “Security is not a product, but a process.” – Bruce Schneier

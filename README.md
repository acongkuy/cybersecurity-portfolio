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

Saya adalah siswa lulusan tahun 2025 kelas 6D MAK di Darunnajah dengan minat besar pada **keamanan siber**. Sejak tahun 2025, saya aktif dalam eksplorasi, pengujian, dan pelaporan kerentanan keamanan, baik melalui platform bug bounty internasional seperti **HackerOne**, maupun secara langsung kepada pihak sekolah.  

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

## 3. 🔍 Audit dan Penanganan Kerentanan pada Subdomain simak.darunnajah.ac.id/login

### 3.1 📝 Latar Belakang

Subdomain ini adalah aplikasi berbasis PHP dengan framework CodeIgniter. Saat diuji, input karakter khusus `'` menyebabkan error PHP terkait pengelolaan sesi pengguna. Selain itu, versi jQuery yang dipakai adalah 1.2.1, yang sudah lama dan rawan serangan XSS serta manipulasi DOM.

### 3.2 ⚠️ Temuan Kerentanan

* 🛑 **Masalah Pengelolaan Sesi:** Sesi pengguna tidak diinisialisasi atau diakses dengan benar, berpotensi bocor data atau kegagalan autentikasi.
* 🔍 **Input Tidak Aman:** Input karakter khusus bisa picu error dan membuka celah injeksi atau XSS.
* 📉 **jQuery Versi Lama:** Versi 1.2.1 rentan terhadap XSS dan manipulasi DOM yang berbahaya.
* 💥 **Penanganan Error Buruk:** Pesan error teknis langsung tampil ke pengguna, bisa jadi bahan eksploitasi.

### 3.3 💥 Dampak

* 🔐 Risiko bocornya data pengguna dan celah keamanan aplikasi.
* 😕 Pengalaman pengguna buruk karena munculnya pesan error teknis.
* ⚠️ Potensi eksploitasi dari pustaka jQuery yang sudah usang.

### 3.4 💡 Rekomendasi Perbaikan

* 🔒 Sanitasi & validasi input ketat, gunakan `htmlspecialchars()` atau `addslashes()`.
* 🛠️ Pastikan sesi diinisialisasi dan dicek sebelum dipakai.
* 🚫 Terapkan error handling aman, jangan tampilkan pesan teknis ke pengguna.
* ⬆️ Update jQuery ke versi terbaru (misal 3.x), pakai Content Security Policy (CSP) & Subresource Integrity (SRI).

---
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

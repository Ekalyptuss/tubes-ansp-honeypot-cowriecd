# IMPLEMENTASI HONEYPOT SEBAGAI PENDETEKSI SERANGAN SSH  
## Tugas Besar – Advanced Network Security and Protocols

---

## 📌 Deskripsi Proyek
Repository ini berisi **laporan, dokumentasi, dan hasil implementasi Honeypot SSH menggunakan Cowrie** sebagai bagian dari **Tugas Besar Mata Kuliah Advanced Network Security and Protocols (ANSP)**.

Proyek ini bertujuan untuk:
- Menerapkan honeypot sebagai **alat deteksi serangan**
- Menganalisis **pola serangan SSH**
- Mengamati **aktivitas penyerang secara langsung**
- Mengumpulkan dan menganalisis **log keamanan**

---

## 🧠 Topik
- Network Security
- Honeypot
- SSH Attack Detection
- Cowrie Honeypot
- Log Analysis
- Cyber Attack Simulation

---

## 🛠 Tools & Teknologi
| Komponen | Keterangan |
|--------|------------|
| OS Host | macOS |
| Virtualization | UTM (QEMU ARM64) |
| Guest OS | Ubuntu Server 24.04 LTS (ARM64) |
| Honeypot | Cowrie SSH Honeypot |
| Language | Python 3 |
| Protocol | SSH |
| Logging | JSON Log Cowrie |
| Attack Simulation | SSH brute-force & command execution |

---

## 🧩 Lingkungan Praktikum
- **Host:** MacBook (Apple Silicon)
- **VM:** Ubuntu Server 24.04 LTS
- **IP Server:** `192.168.64.2`
- **Port Honeypot:** `2222`
- **User Honeypot:** `cowrie`
- **Akses Penyerang:** SSH dari macOS host

---

## ⚙️ Alur Implementasi
1. Instalasi Ubuntu Server menggunakan ISO ARM64 di UTM
2. Update dan upgrade sistem
3. Instalasi dependensi Cowrie
4. Pembuatan user khusus Cowrie
5. Instalasi Cowrie menggunakan virtual environment
6. Konfigurasi file `cowrie.cfg`
7. Menjalankan Cowrie SSH Honeypot
8. Simulasi serangan SSH dari host
9. Pengambilan dan analisis log serangan
10. Dokumentasi hasil dan kesimpulan

---

## 🔐 Skenario Serangan
Sesuai dengan instruksi tugas besar, dilakukan simulasi:
- Login SSH ke port honeypot (2222)
- Percobaan autentikasi
- Eksekusi perintah seperti:
  - `whoami`
  - `uname -a`
  - `ls`
  - `cat /etc/passwd`
  - `ps aux`

Semua aktivitas berhasil direkam oleh Cowrie.

---

## 📊 Hasil & Analisis
- Cowrie berhasil menangkap:
  - IP penyerang
  - Username & password
  - Perintah yang dijalankan
  - Versi SSH client
- Log tersimpan dalam format **JSON**
- Data siap digunakan untuk analisis forensik dan pola serangan
📦 tubes-ansp-honeypot-cowrie
┣ 📂 laporan
┃ ┗ 📄 Laporan_Praktikum_Honeypot_Cowrie.docx
┣ 📂 dokumentasi
┃ ┗ 📷 Screenshot instalasi & pengujian
┣ 📂 log
┃ ┗ 📄 cowrie.json
┣ 📄 README.md

---

## 🧪 Bukti Implementasi
- Screenshot instalasi Ubuntu Server
- Screenshot konfigurasi Cowrie
- Screenshot koneksi SSH ke honeypot
- Screenshot log serangan SSH
- Dokumentasi lengkap pada laporan Word

---

## 📌 Kesimpulan
Implementasi honeypot SSH menggunakan Cowrie **berhasil dilakukan dengan baik**.  
Sistem mampu mendeteksi, merekam, dan menyimpan aktivitas penyerang sesuai tujuan tugas besar.

---

## 👤 Identitas Mahasiswa
- **Nama:** Muhal Haikal  
- **Mata Kuliah:** Advanced Network Security and Protocols  
- **Tugas:** Tugas Besar (TUBES)

---

## ⚠️ Catatan
Repository ini dibuat **khusus untuk keperluan akademik** dan pembelajaran keamanan jaringan.
---

## 📁 Struktur Repository

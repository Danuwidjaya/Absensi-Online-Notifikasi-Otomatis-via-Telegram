# 🧾 Absensi Online & Notifikasi Otomatis via Telegram

## 📌 Deskripsi Singkat
Sistem ini dibuat untuk mengotomatiskan proses absensi harian dengan mengirimkan notifikasi ke grup Telegram setiap kali form absensi diisi oleh karyawan.

## 🎯 Tujuan Project
- Mempercepat proses pengecekan kehadiran.
- Mengurangi beban admin untuk monitoring manual.
- Meningkatkan transparansi dan komunikasi tim.

## 🛠️ Tools yang Digunakan

| Tools         | Fungsi                                  |
|---------------|------------------------------------------|
| Google Forms  | Input data absensi                       |
| Google Sheets | Menyimpan data absensi                   |
| Make.com      | Otomasi integrasi dan alur kerja         |
| Telegram      | Media notifikasi ke grup                 |
| Telegram Bot  | Pengirim pesan otomatis dari sistem      |

## 🔄 Alur Kerja (Workflow)

```mermaid
flowchart TD
    A[Form Absensi Diisi] --> B[Google Sheets Bertambah Row]
    B --> C[Make.com Deteksi Trigger]
    C --> D[Ambil Data Absensi]
    D --> E[Format Pesan]
    E --> F[Kirim ke Grup Telegram via Bot]

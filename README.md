# 📎 URL-Based Minimal Text Editor

Sebuah **web text editor super minimalis** yang **menyimpan seluruh isi catatan langsung di dalam URL**.  
Tidak menggunakan akun, database, backend, atau server sama sekali.

Semua berjalan **100% di browser** dan bisa di-host sebagai **static website**.

---

## Fitur Utama

- Editor teks minimalis
- Seluruh catatan tersimpan di URL
- Mudah dibagikan (cukup copy link)
- Tanpa login
- Tanpa database
- Tanpa backend
- Static HTML + JavaScript

---

## Cara Kerja

1. Teks yang diketik:
   - Di-encode ke **Base64**
   - Disimpan di bagian URL (`#fragment`)
2. Saat link dibuka:
   - URL otomatis di-decode
   - Teks muncul kembali di editor

---

## Batasan

- Panjang URL terbatas (sekitar 2–8 ribu karakter tergantung browser)
- Data **tidak terenkripsi**
- Tidak cocok untuk catatan sangat panjang
- Siapa pun yang punya link bisa membaca isi catatan

---

## Ide Pengembangan

- Enkripsi sebelum encode
- Kompresi teks (LZ-String)
- Preview Markdown
- Ganti tema
- Tombol copy link

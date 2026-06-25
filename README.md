# QRIS Decoder and Parser

## Yang diperbaiki:

Load jsQR dari cdn.jsdelivr.net yang proper untuk standalone HTML
Tambah loading spinner saat proses decode
Coba 3 skala gambar (100%, 200%, 50%) supaya deteksi lebih robust
Error message lebih informatif

## Fitur tambahan:

Ctrl+V langsung di halaman juga bisa paste gambar (tidak perlu klik tombol paste dulu)
Tombol "Copy" untuk copy raw string
Value enriched — contoh tag 53 (currency) langsung tampil 360 → IDR – Rupiah Indonesia
Tag 01 langsung tampil apakah Static atau Dynamic QR

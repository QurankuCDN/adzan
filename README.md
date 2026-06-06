# Quranku Adzan CDN

<p align="center">
  <img src="./Icon/40edeba4-756b-4440-9738-f15ffe394768.png" alt="Quranku Adzan CDN" width="120">
</p>

Repository ini berisi aset statis audio adzan dan ikon yang digunakan sebagai CDN pendukung untuk **Quranku API**.

API utama: [https://quranku.apirizz.my.id](https://quranku.apirizz.my.id)

## Base URL CDN

Gunakan base URL berikut untuk mengambil aset dari repository ini:

```text
https://cdn.jsdelivr.net/gh/QurankuCDN/adzan@main/
```

Fallback GitHub raw:

```text
https://raw.githubusercontent.com/QurankuCDN/adzan/main/
```

Contoh akses audio:

```text
https://cdn.jsdelivr.net/gh/QurankuCDN/adzan@main/4%20Waktu/Adzan%20Arab.mp3
```

## Struktur Aset

```text
.
|-- 4 Waktu/
|   |-- ADZAN BAYYATI HUSAINI.mp3
|   |-- AZAN ASJAL RUWHI.mp3
|   |-- Adzan Arab.mp3
|   |-- Adzan Nahawand.mp3
|   |-- Adzan Rast.mp3
|   |-- Azan jiharkah Abdulkarim Almakki.mp3
|   `-- Makkah Maghri.mp3
|-- Subuh/
|   |-- AZAN SUBUH JIHARKAH.mp3
|   |-- Adzan Subuh Nahawand .mp3
|   `-- Azan by Mishary Rashid Al Afasy.mp3
`-- Icon/
    |-- 40edeba4-756b-4440-9738-f15ffe394768.png
    `-- favicon.ico
```

## Penggunaan di Quranku API

Quranku API di [https://quranku.apirizz.my.id](https://quranku.apirizz.my.id) dapat memakai URL CDN dari repository ini untuk mengembalikan file audio adzan dan ikon aplikasi ke client.

Contoh response:

```json
{
  "name": "Adzan Arab",
  "category": "4 Waktu",
  "audio": "https://cdn.jsdelivr.net/gh/QurankuCDN/adzan@main/4%20Waktu/Adzan%20Arab.mp3"
}
```

## Catatan Pemeliharaan

- Jaga nama folder dan file tetap stabil karena URL aset bisa dipakai langsung oleh API dan client.
- Jika ada spasi pada path, encode sebagai `%20` saat digunakan di URL.
- Hindari file tunggal di atas 100 MB untuk penyimpanan GitHub biasa.
- Setelah menambah, menghapus, atau mengganti nama aset, update README dan konfigurasi API yang memakai path tersebut.

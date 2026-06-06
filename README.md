<div align="center">
  <img src="./Icon/40edeba4-756b-4440-9738-f15ffe394768.png" alt="Quranku Adzan CDN" width="128">

  <h1>Quranku Adzan CDN</h1>

  <p>
    CDN aset audio adzan dan ikon resmi untuk integrasi
    <strong>Quranku API</strong>.
  </p>

  <p>
    <a href="https://quranku.apirizz.my.id"><strong>Quranku API</strong></a>
    &middot;
    <a href="https://github.com/QurankuCDN/adzan">Repository</a>
    &middot;
    <a href="#daftar-aset">Daftar Aset</a>
  </p>

  <p>
    <img alt="CDN jsDelivr" src="https://img.shields.io/badge/CDN-jsDelivr-ff5627?style=flat-square">
    <img alt="Asset Type" src="https://img.shields.io/badge/assets-MP3%20%7C%20PNG%20%7C%20ICO-0f766e?style=flat-square">
    <img alt="Repository" src="https://img.shields.io/badge/repository-static%20cdn-2563eb?style=flat-square">
  </p>
</div>

---

## Overview

Repository ini menyimpan aset statis yang dipakai oleh
[Quranku API](https://quranku.apirizz.my.id), khususnya file audio adzan untuk
jadwal shalat dan ikon aplikasi. Aset dibuat mudah diakses melalui CDN agar
client tidak perlu mengambil file langsung dari server API utama.

## Base URL

Gunakan jsDelivr sebagai endpoint utama untuk distribusi aset:

```text
https://cdn.jsdelivr.net/gh/QurankuCDN/adzan@main/
```

Fallback GitHub raw:

```text
https://raw.githubusercontent.com/QurankuCDN/adzan/main/
```

## Quick Start

Contoh URL audio:

```text
https://cdn.jsdelivr.net/gh/QurankuCDN/adzan@main/4%20Waktu/Adzan%20Arab.mp3
```

Contoh URL ikon:

```text
https://cdn.jsdelivr.net/gh/QurankuCDN/adzan@main/Icon/40edeba4-756b-4440-9738-f15ffe394768.png
```

Contoh response dari API:

```json
{
  "name": "Adzan Arab",
  "category": "4 Waktu",
  "audio": "https://cdn.jsdelivr.net/gh/QurankuCDN/adzan@main/4%20Waktu/Adzan%20Arab.mp3"
}
```

## Daftar Aset

### Audio Adzan 4 Waktu

| Nama | Path | CDN |
| --- | --- | --- |
| ADZAN BAYYATI HUSAINI | `4 Waktu/ADZAN BAYYATI HUSAINI.mp3` | [Play](https://cdn.jsdelivr.net/gh/QurankuCDN/adzan@main/4%20Waktu/ADZAN%20BAYYATI%20HUSAINI.mp3) |
| AZAN ASJAL RUWHI | `4 Waktu/AZAN ASJAL RUWHI.mp3` | [Play](https://cdn.jsdelivr.net/gh/QurankuCDN/adzan@main/4%20Waktu/AZAN%20ASJAL%20RUWHI.mp3) |
| Adzan Arab | `4 Waktu/Adzan Arab.mp3` | [Play](https://cdn.jsdelivr.net/gh/QurankuCDN/adzan@main/4%20Waktu/Adzan%20Arab.mp3) |
| Adzan Nahawand | `4 Waktu/Adzan Nahawand.mp3` | [Play](https://cdn.jsdelivr.net/gh/QurankuCDN/adzan@main/4%20Waktu/Adzan%20Nahawand.mp3) |
| Adzan Rast | `4 Waktu/Adzan Rast.mp3` | [Play](https://cdn.jsdelivr.net/gh/QurankuCDN/adzan@main/4%20Waktu/Adzan%20Rast.mp3) |
| Azan Jiharkah Abdulkarim Almakki | `4 Waktu/Azan jiharkah Abdulkarim Almakki.mp3` | [Play](https://cdn.jsdelivr.net/gh/QurankuCDN/adzan@main/4%20Waktu/Azan%20jiharkah%20Abdulkarim%20Almakki.mp3) |
| Makkah Maghri | `4 Waktu/Makkah Maghri.mp3` | [Play](https://cdn.jsdelivr.net/gh/QurankuCDN/adzan@main/4%20Waktu/Makkah%20Maghri.mp3) |

### Audio Adzan Subuh

| Nama | Path | CDN |
| --- | --- | --- |
| AZAN SUBUH JIHARKAH | `Subuh/AZAN SUBUH JIHARKAH.mp3` | [Play](https://cdn.jsdelivr.net/gh/QurankuCDN/adzan@main/Subuh/AZAN%20SUBUH%20JIHARKAH.mp3) |
| Adzan Subuh Nahawand | `Subuh/Adzan Subuh Nahawand .mp3` | [Play](https://cdn.jsdelivr.net/gh/QurankuCDN/adzan@main/Subuh/Adzan%20Subuh%20Nahawand%20.mp3) |
| Azan by Mishary Rashid Al Afasy | `Subuh/Azan by Mishary Rashid Al Afasy.mp3` | [Play](https://cdn.jsdelivr.net/gh/QurankuCDN/adzan@main/Subuh/Azan%20by%20Mishary%20Rashid%20Al%20Afasy.mp3) |

### Ikon

| Nama | Path | CDN |
| --- | --- | --- |
| Quranku Icon PNG | `Icon/40edeba4-756b-4440-9738-f15ffe394768.png` | [View](https://cdn.jsdelivr.net/gh/QurankuCDN/adzan@main/Icon/40edeba4-756b-4440-9738-f15ffe394768.png) |
| Favicon | `Icon/favicon.ico` | [View](https://cdn.jsdelivr.net/gh/QurankuCDN/adzan@main/Icon/favicon.ico) |

## Struktur Repository

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
|-- Icon/
|   |-- 40edeba4-756b-4440-9738-f15ffe394768.png
|   `-- favicon.ico
`-- README.md
```

## Integrasi API

Saat mengirim data adzan dari Quranku API, simpan URL CDN penuh di field audio
agar client dapat memutar file langsung:

```json
{
  "id": "adzan-arab",
  "label": "Adzan Arab",
  "type": "regular",
  "source": "cdn",
  "url": "https://cdn.jsdelivr.net/gh/QurankuCDN/adzan@main/4%20Waktu/Adzan%20Arab.mp3"
}
```

## Maintenance

- Pertahankan nama file dan folder karena path digunakan sebagai URL publik.
- Encode spasi sebagai `%20` saat path dipakai di URL.
- Update README setiap ada aset baru, rename, atau penghapusan file.
- Hindari file tunggal di atas 100 MB untuk kompatibilitas GitHub biasa.
- Untuk cache CDN, gunakan path `@main` untuk aset terbaru atau tag rilis untuk
  versi yang stabil.

---

<div align="center">
  <strong>Quranku Adzan CDN</strong><br>
  Static audio assets for Quranku API
</div>

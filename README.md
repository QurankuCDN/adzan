<div align="center">
  <img src="./Icon/40edeba4-756b-4440-9738-f15ffe394768.png" alt="Quranku Adzan CDN" width="132">

  <h1>Quranku Adzan CDN</h1>

  <p>
    Asset delivery layer for <strong>Quranku API</strong>, built to serve
    adzan audio and application icons through a fast public CDN.
  </p>

  <p>
    <a href="https://quranku.apirizz.my.id"><strong>Live API</strong></a>
    &nbsp;|&nbsp;
    <a href="https://github.com/QurankuCDN/adzan"><strong>GitHub Repository</strong></a>
    &nbsp;|&nbsp;
    <a href="#asset-catalog"><strong>Asset Catalog</strong></a>
  </p>

  <p>
    <img alt="CDN" src="https://img.shields.io/badge/CDN-jsDelivr-f97316?style=for-the-badge">
    <img alt="Audio" src="https://img.shields.io/badge/audio-MP3-0f766e?style=for-the-badge">
    <img alt="Icons" src="https://img.shields.io/badge/icons-PNG%20%7C%20ICO-2563eb?style=for-the-badge">
    <img alt="Repository" src="https://img.shields.io/badge/type-static%20assets-111827?style=for-the-badge">
  </p>
</div>

---

## Purpose

**Quranku Adzan CDN** adalah repository aset statis untuk mendukung
[Quranku API](https://quranku.apirizz.my.id). Repository ini memisahkan file
audio dan ikon dari server API utama agar response API tetap ringan, konsisten,
dan mudah digunakan oleh client web maupun mobile.

## Delivery Endpoints

| Channel | Base URL | Usage |
| --- | --- | --- |
| Primary CDN | `https://cdn.jsdelivr.net/gh/QurankuCDN/adzan@main/` | Recommended untuk aplikasi production |
| GitHub Raw | `https://raw.githubusercontent.com/QurankuCDN/adzan/main/` | Fallback langsung dari repository |
| Repository | `https://github.com/QurankuCDN/adzan` | Source of truth aset CDN |

### Quick Copy

```text
https://cdn.jsdelivr.net/gh/QurankuCDN/adzan@main/
```

Audio example:

```text
https://cdn.jsdelivr.net/gh/QurankuCDN/adzan@main/4%20Waktu/Adzan%20Arab.mp3
```

Icon example:

```text
https://cdn.jsdelivr.net/gh/QurankuCDN/adzan@main/Icon/40edeba4-756b-4440-9738-f15ffe394768.png
```

## Integration Contract

Quranku API dapat mengembalikan URL CDN penuh pada response agar client bisa
langsung memutar audio tanpa membangun path secara manual.

```json
{
  "id": "adzan-arab",
  "name": "Adzan Arab",
  "category": "4-waktu",
  "mime": "audio/mpeg",
  "source": "quranku-cdn",
  "url": "https://cdn.jsdelivr.net/gh/QurankuCDN/adzan@main/4%20Waktu/Adzan%20Arab.mp3"
}
```

### HTML Audio

```html
<audio controls preload="metadata">
  <source
    src="https://cdn.jsdelivr.net/gh/QurankuCDN/adzan@main/4%20Waktu/Adzan%20Arab.mp3"
    type="audio/mpeg"
  >
</audio>
```

### JavaScript

```js
const adzanAudio = new Audio(
  "https://cdn.jsdelivr.net/gh/QurankuCDN/adzan@main/4%20Waktu/Adzan%20Arab.mp3"
);

await adzanAudio.play();
```

## Asset Catalog

### Audio: 4 Waktu

| Asset | Path | CDN |
| --- | --- | --- |
| ADZAN BAYYATI HUSAINI | `4 Waktu/ADZAN BAYYATI HUSAINI.mp3` | [Open](https://cdn.jsdelivr.net/gh/QurankuCDN/adzan@main/4%20Waktu/ADZAN%20BAYYATI%20HUSAINI.mp3) |
| AZAN ASJAL RUWHI | `4 Waktu/AZAN ASJAL RUWHI.mp3` | [Open](https://cdn.jsdelivr.net/gh/QurankuCDN/adzan@main/4%20Waktu/AZAN%20ASJAL%20RUWHI.mp3) |
| Adzan Arab | `4 Waktu/Adzan Arab.mp3` | [Open](https://cdn.jsdelivr.net/gh/QurankuCDN/adzan@main/4%20Waktu/Adzan%20Arab.mp3) |
| Adzan Nahawand | `4 Waktu/Adzan Nahawand.mp3` | [Open](https://cdn.jsdelivr.net/gh/QurankuCDN/adzan@main/4%20Waktu/Adzan%20Nahawand.mp3) |
| Adzan Rast | `4 Waktu/Adzan Rast.mp3` | [Open](https://cdn.jsdelivr.net/gh/QurankuCDN/adzan@main/4%20Waktu/Adzan%20Rast.mp3) |
| Azan Jiharkah Abdulkarim Almakki | `4 Waktu/Azan jiharkah Abdulkarim Almakki.mp3` | [Open](https://cdn.jsdelivr.net/gh/QurankuCDN/adzan@main/4%20Waktu/Azan%20jiharkah%20Abdulkarim%20Almakki.mp3) |
| Makkah Maghri | `4 Waktu/Makkah Maghri.mp3` | [Open](https://cdn.jsdelivr.net/gh/QurankuCDN/adzan@main/4%20Waktu/Makkah%20Maghri.mp3) |

### Audio: Subuh

| Asset | Path | CDN |
| --- | --- | --- |
| AZAN SUBUH JIHARKAH | `Subuh/AZAN SUBUH JIHARKAH.mp3` | [Open](https://cdn.jsdelivr.net/gh/QurankuCDN/adzan@main/Subuh/AZAN%20SUBUH%20JIHARKAH.mp3) |
| Adzan Subuh Nahawand | `Subuh/Adzan Subuh Nahawand .mp3` | [Open](https://cdn.jsdelivr.net/gh/QurankuCDN/adzan@main/Subuh/Adzan%20Subuh%20Nahawand%20.mp3) |
| Azan by Mishary Rashid Al Afasy | `Subuh/Azan by Mishary Rashid Al Afasy.mp3` | [Open](https://cdn.jsdelivr.net/gh/QurankuCDN/adzan@main/Subuh/Azan%20by%20Mishary%20Rashid%20Al%20Afasy.mp3) |

### Brand Assets

| Asset | Path | CDN |
| --- | --- | --- |
| Quranku Icon | `Icon/40edeba4-756b-4440-9738-f15ffe394768.png` | [Open](https://cdn.jsdelivr.net/gh/QurankuCDN/adzan@main/Icon/40edeba4-756b-4440-9738-f15ffe394768.png) |
| Favicon | `Icon/favicon.ico` | [Open](https://cdn.jsdelivr.net/gh/QurankuCDN/adzan@main/Icon/favicon.ico) |

## Repository Map

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

## Operational Notes

| Topic | Standard |
| --- | --- |
| URL stability | Jangan rename folder atau file tanpa update API consumer |
| Encoding | Gunakan `%20` untuk spasi pada URL publik |
| Cache | Gunakan `@main` untuk latest asset atau tag release untuk versi stabil |
| File size | Jaga file tunggal di bawah batas GitHub biasa, maksimal 100 MB |
| Updates | Setiap perubahan aset harus disertai update katalog README |

## Recommended API Shape

```json
{
  "cdn": {
    "provider": "jsdelivr",
    "baseUrl": "https://cdn.jsdelivr.net/gh/QurankuCDN/adzan@main/"
  },
  "assets": {
    "regular": "4 Waktu/Adzan Arab.mp3",
    "subuh": "Subuh/AZAN SUBUH JIHARKAH.mp3",
    "icon": "Icon/40edeba4-756b-4440-9738-f15ffe394768.png"
  }
}
```

---

<div align="center">
  <strong>Quranku Adzan CDN</strong>
  <br>
  Public static assets for Quranku API
  <br>
  <a href="https://quranku.apirizz.my.id">quranku.apirizz.my.id</a>
</div>

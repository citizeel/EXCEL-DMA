# Forum 12.2 – Merapikan Dashboard (lanjutan Forum 12.1)

File: `2902836054_Mellanda_Kumalasari_Dashboard_Forum_12.2_Rapi.xlsx` (sheet **Dashboard**; sheet data/summary tidak diubah)

## 1. Elemen apa yang dikurangi, dihilangkan, atau dirapikan?

| Elemen | Tindakan |
|---|---|
| Banner judul 2 lapis (fill navy + fill abu gelap, teks putih 20pt) | Diganti judul teks biasa + subjudul dengan satu garis tipis |
| Baris "filter" Year / Genre / Artist / Subscription | Dihapus (hanya teks statis, bukan slicer, tidak bisa diklik) |
| Angka 1, 2, 3, 5 yang nyasar di kolom A | Dihapus |
| Chart "Unique Listeners per Hari" | Dihapus (pola hampir sama dengan Total Plays per Hari, data hanya 0–2) |
| Border biru tebal + header bar berwarna pada 4 KPI card | Diganti kartu abu-abu muda tanpa border |
| Donut chart 3 warna + legend | Diganti bar horizontal 1 warna (tanpa legend) |
| 3 kotak insight 3 warna (hijau, kuning, biru) dengan border tebal | Satu gaya: label + teks, dipisah garis tipis |
| Border abu tebal di sekeliling chart, gridline rapat, axis tick | Dihapus / dilemahkan |
| Zoom 51% | Dikembalikan ke 100% |

Jumlah chart turun dari 4 menjadi 3, dan tinggi dashboard turun dari 40 baris ke 33 baris.

## 2. Mengapa dianggap noise?

- **Tidak membawa informasi**: angka nyasar di kolom A, dan filter yang tidak berfungsi justru menyesatkan karena tampak bisa diklik.
- **Duplikat**: dua chart tren harian menjawab pertanyaan yang sama sehingga mata harus membandingkan dua grafik untuk hasil yang sama.
- **Dekorasi bersaing dengan data**: border tebal, fill gelap, dan banyak warna menarik perhatian ke bingkai, bukan ke angka.
- **Warna tanpa makna**: 3 warna insight dan 3 warna donut tidak menandai apa pun yang berbeda secara bisnis.
- **Pesan kontradiktif**: insight lama menyebut rata-rata 6 plays "tergolong sedang", padahal KPI-nya berstatus "Tercapai" (target ≥5).

## 3. Bagaimana dashboard dibuat lebih mudah dibaca?

- **Urutan baca atas → bawah**: judul → 4 KPI → tren → perbandingan (lagu & genre) → insight.
- **KPI jadi fokus**: angka 28pt bold di kartu bersih. Status target tampil kecil di bawah angkanya (hijau saat tercapai, otomatis oranye/merah saat Waspada/Rendah).
- **Warna dibatasi**: navy untuk data utama, abu-biru untuk pembanding, abu untuk teks dan garis. Hijau/oranye/merah hanya dipakai untuk status.
- **Bar chart menonjolkan yang teratas**: batang pertama (lagu/genre teratas) navy, sisanya diredam. Label nilai langsung di ujung batang, sumbu angka dihapus.
- **Judul seksi bermakna**: setiap bagian punya judul satu baris dengan garis bawah tipis.
- **Whitespace**: spasi antar bagian seragam, kolom dan lebar chart sejajar dengan kartu KPI.
- **Insight ringkas dan konsisten**: teks tetap dihitung otomatis dari data (formula), dan kini selaras dengan status KPI.

## 4. Perbedaan sebelum vs sesudah

| | Sebelum | Sesudah |
|---|---|---|
| Elemen dekoratif | Banner gelap, border tebal, header bar, 3 warna kotak | Garis tipis dan kartu abu muda |
| Chart | 4 (garis, kolom, bar, donut + legend) | 3 (garis, bar, bar) |
| Warna dominan | Navy, biru, oranye, abu, hijau, kuning | Navy + abu (hijau/oranye/merah hanya untuk status) |
| Filter palsu | 4 kotak "▾" | Tidak ada |
| Tinggi | 40 baris, zoom 51% | 33 baris, zoom 100% |
| Insight | Kontradiktif dengan KPI | Konsisten dengan target KPI |

> Catatan: semua nilai KPI, chart, dan insight tetap tersambung ke sheet Summary_KPI / Summary_Lagu / Summary_Genre / Data_Tren, jadi ikut berubah bila data berubah.

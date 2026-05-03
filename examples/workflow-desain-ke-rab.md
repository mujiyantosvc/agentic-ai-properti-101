# Workflow: Dari Desain ke RAB

**Kasus:** Renovasi tampak depan rumah tipe 72, 1 lantai, budget terbatas.

---

## Konteks

Pak Arief (45 tahun, karyawan BUMN) punya rumah tipe 72 di kawasan perumahan Tangerang. Rumah sudah 12 tahun, tampak depan terlihat sangat standar — cat putih polos mengelupas, pagar besi lama berkarat, tidak ada teras.

Istrinya ingin renovasi tampak depan sebelum ulang tahun pernikahan ke-20 tahun ini. Budget yang tersedia: 45-65 juta.

Pak Arief tidak punya waktu banyak untuk riset — dia ingin bisa datang ke kontraktor dengan ide yang sudah agak jelas, bukan mulai dari nol.

---

## Yang Dibutuhkan untuk Workflow Ini

- Foto tampak depan rumah (minimal 2-3 angle)
- Foto tampak samping jika ada
- Dimensi dasar: lebar fasad, posisi pintu, jendela, carport
- Akses ke tools AI (ChatGPT, Claude, atau tools serupa)
- Waktu: 2-3 jam untuk run workflow ini dari awal

---

## Langkah 1: Buat Brief Properti (Layer 1 — Context)

Sebelum prompt pertama, isi dulu template brief.

**Brief Pak Arief:**

```
Nama proyek: Renovasi Fasad Rumah
Tipe properti: Rumah tapak 1 lantai
Lokasi: Tangerang, Banten (iklim tropis panas)
Luas tanah: 120 m²
Luas bangunan: 72 m²
Jumlah lantai: 1
Kondisi saat ini: Cat lama mengelupas, pagar besi berkarat, tidak ada teras,
                  tampak depan sangat standar dan tidak ada karakter
Tujuan: Renovasi tampak depan untuk estetika dan sedikit meningkatkan nilai properti
Gaya yang diinginkan: Minimalis modern tropis, tidak terlalu futuristik
Budget: Rp 45-65 juta
Batasan penting:
  - Tidak ubah posisi pintu utama
  - Tidak ubah posisi dan ukuran jendela (3 jendela depan)
  - Carport motor di kanan — bisa sedikit dimodifikasi tapi tidak dipindah
  - Tidak ada perubahan struktur atau atap
Output yang diinginkan: Eksplorasi opsi renovasi + estimasi kasar
```

---

## Langkah 2: Eksplorasi Opsi Renovasi (Layer 3 — Reasoning)

**Prompt ke AI:**

```
Saya punya rumah tipe 72, 1 lantai di Tangerang. Iklim panas, usia bangunan 12 tahun.
Tampak depan: cat putih mengelupas, pagar besi lama berkarat, tidak ada teras.
Lebar fasad kira-kira 8 meter, tinggi 4 meter dari tanah.

Budget renovasi tampak depan: 45-65 juta.

Batasan:
- Tidak ubah posisi pintu, jendela (3 jendela di fasad depan), carport motor kanan
- Tidak ada perubahan struktural atau atap
- Gaya yang diinginkan: minimalis modern tropis

Bantu saya:
1. Eksplorasi 3 opsi renovasi dengan level investasi berbeda
   (ekonomis / menengah / maksimal dalam budget)
2. Untuk tiap opsi: deskripsikan apa saja yang dikerjakan dan tampak seperti apa
3. Pertimbangan khusus untuk iklim Tangerang (panas, hujan)
4. Warning untuk hal yang sering jadi surprise cost di renovasi fasad
```

**Output yang diharapkan:**

Tiga opsi renovasi:

**Opsi A — Ekonomis (estimasi 20-30 juta):**
- Cat ulang seluruh fasad dengan cat eksterior premium (2 lapis)
- Pagar hollow besi baru model minimalis, cat powder coating hitam
- Tambah kanopi ringan baja ringan+polycarbonate di atas pintu
- Tanaman pot di kiri-kanan pintu

**Opsi B — Menengah (estimasi 35-50 juta):**
- Cat ulang + tambah aksen panel GRC atau roster di area atas jendela
- Pagar hollow baru + pilaster/kolom tipis
- Tambah teras mini (2x1.5m) dengan lantai keramik abu
- Kanopi baja hollow (bukan polycarbonate, lebih rapi)
- Tanaman tropis di area teras

**Opsi C — Maksimal dalam budget (estimasi 50-65 juta):**
- Cat ulang + aksen batu alam andesit di area carport
- Pagar kombinasi bata-hollow modern dengan lampu spot
- Teras 2x2m dengan pergola kayu WPC ringan
- Roster panel sebagai secondary skin area jendela tengah
- Landscape mini: batu kerikil + tanaman tropis rendah

---

## Langkah 3: Deskripsi Visual per Opsi (Layer 2 — Visual)

**Prompt ke AI:**

```
Berdasarkan Opsi B yang sudah dijelaskan (renovasi menengah 35-50 juta),
deskripsikan secara detail tampak visual hasil akhir yang diinginkan:

- Warna cat fasad: rekomendasikan kombinasi warna yang cocok untuk minimalis modern tropis
- Panel GRC/roster: di mana tepatnya? Ukuran kira-kira? Warna?
- Pagar: tipe hollow, tinggi berapa? Dengan atau tanpa tiang kolom?
- Teras mini: material lantai apa? Ada step naik atau langsung datar?
- Kanopi: material dan bentuk yang paling tahan di iklim Tangerang?
- Tanaman: jenis apa yang cocok, rendah perawatan, tahan panas?

Deskripsikan sedetail mungkin sehingga saya bisa menjelaskan ini ke kontraktor
atau bisa menjadi basis untuk eksplorasi visual lebih lanjut.
```

**Output:** Deskripsi visual yang bisa dijadikan brief untuk kontraktor atau input untuk tools AI visual.

---

## Langkah 4: Estimasi Biaya Kasar (Layer 4 — Cost)

**Prompt ke AI:**

```
Berdasarkan Opsi B renovasi fasad rumah tipe 72 di Tangerang
(cat ulang, panel GRC, pagar hollow, teras mini, kanopi baja ringan):

Buat estimasi biaya kasar dalam tabel per item, untuk:
- Lokasi: Tangerang, Banten
- Kualitas material: menengah (bukan ekonomis, bukan premium)
- Tahun estimasi: 2025-2026

Kolom tabel: Item | Volume | Satuan | Range Harga Satuan | Range Total

Setelah tabel, sertakan:
- Subtotal material + upah
- Overhead kontraktor (estimasi 15-20%)
- Contingency 10%
- TOTAL RANGE

Tambahkan:
- Asumsi upah yang dipakai
- 3 item yang paling berpotensi membuat biaya naik
- Disclaimer bahwa ini perlu dikonfirmasi survey kontraktor
```

**Output yang diharapkan (contoh):**

| Item | Volume | Satuan | Range Harga Satuan | Range Total |
|------|--------|--------|--------------------|-------------|
| Cat eksterior premium (Dulux/Nippon) | 80 | m² | 75.000 - 110.000 | 6 - 8,8 juta |
| Plester ulang area rusak | 12 | m² | 100.000 - 150.000 | 1,2 - 1,8 juta |
| Panel GRC aksen | 6 | m² | 280.000 - 420.000 | 1,7 - 2,5 juta |
| Pagar hollow besi + cat | 7 | m | 650.000 - 950.000 | 4,6 - 6,7 juta |
| Kolom tiang pagar (2 bh) | 2 | unit | 400.000 - 700.000 | 0,8 - 1,4 juta |
| Teras mini (3 m²) + keramik | 3 | m² | 350.000 - 500.000 | 1 - 1,5 juta |
| Kanopi baja hollow + zincalum | 3 | m² | 500.000 - 750.000 | 1,5 - 2,3 juta |
| Tanaman + pot | 1 | set | 300.000 - 600.000 | 0,3 - 0,6 juta |
| Lampu eksterior | 3 | titik | 250.000 - 450.000 | 0,75 - 1,35 juta |
| **Subtotal** | | | | **17,8 - 26,9 juta** |
| Overhead 15-20% | | | | 2,7 - 5,4 juta |
| Contingency 10% | | | | 1,8 - 2,7 juta |
| **TOTAL ESTIMASI** | | | | **Rp 22,3 - 35 juta** |

*Asumsi: upah tukang Tangerang Rp 130-170k/hari. Material menengah. Belum termasuk PPN.*

---

## Langkah 5: Buat Brief untuk Kontraktor

**Prompt ke AI:**

```
Buat brief renovasi fasad yang bisa saya bawa ke kontraktor saat survey.

Brief harus berisi:
1. Deskripsi kondisi saat ini
2. Tujuan renovasi
3. Opsi yang ingin saya pertimbangkan (dengan deskripsi visual Opsi B)
4. Batasan yang tidak boleh dilanggar
5. Budget range yang saya punya
6. Pertanyaan yang perlu saya tanyakan ke kontraktor

Format: dokumen singkat 1-2 halaman yang mudah dipahami kontraktor
```

---

## Langkah 6: Validasi Manusia (Layer 7)

Setelah workflow AI selesai, Pak Arief melakukan:

1. **Cetak atau simpan brief** yang dihasilkan
2. **Datang ke 3 kontraktor lokal** untuk minta penawaran berdasarkan brief yang sama
3. **Bandingkan penawaran** dengan estimasi AI sebagai benchmark
4. **Pilih kontraktor** berdasarkan: harga (bandingkan dengan range AI), referensi kerja sebelumnya, dan kenyamanan komunikasi
5. **Survey lapangan** kontraktor terpilih sebelum tanda tangan kontrak
6. **Konfirmasi harga material** di toko setempat untuk item besar

**Hasil:** Pak Arief datang ke kontraktor dengan brief yang jelas, ekspektasi yang realistis, dan benchmark harga yang sudah ada. Diskusi dengan kontraktor jadi lebih produktif dan terarah.

---

## Catatan Pelajaran dari Workflow Ini

- Workflow ini menghemat waktu "bingung mulai dari mana" — dari yang bisa berminggu-minggu jadi 2-3 jam
- Estimasi AI ternyata lebih rendah dari penawaran kontraktor karena tidak memperhitungkan biaya mobilisasi dan bongkar bersih — ini normal, bukan salah AI
- Salah satu kontraktor menyarankan penggantian plesteran yang lebih luas dari yang diperkirakan setelah survey — ini tidak bisa dideteksi AI dari foto
- Brief yang jelas membuat kontraktor lebih mudah memberi penawaran yang comparable (apple-to-apple)

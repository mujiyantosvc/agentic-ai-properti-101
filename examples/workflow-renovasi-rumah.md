# Workflow: Renovasi Rumah Lama di Indonesia

**Kasus:** Rumah lama usia 20 tahun, kondisi umum masih oke tapi terlihat sangat ketinggalan zaman. Tujuan: tampak lebih modern tanpa harus bongkar besar-besaran.

---

## Konteks

Bu Sinta (38 tahun, guru SMP) mewarisi rumah dari orang tuanya di kawasan perumahan Yogyakarta. Rumah usia 22 tahun, tipe 54, kondisi struktural masih bagus tapi:
- Tampak depan: cat kuning pudar, ornamen plester tempel bergaya 90-an
- Carport: kanopi besi dan asbes lama, berkarat
- Pagar: besi model lama, banyak yang bengkok
- Interior: keramik motif lama, plafon triplex menguning
- Kamar mandi: masih jongkok, keramik kecil tahun 90-an

Bu Sinta mau pindah ke sini tahun depan bersama suami. Budget total: 80-120 juta. Ingin tahu: prioritas mana dulu, dan mana yang bisa ditunda?

---

## Input yang Disiapkan

- Foto tampak depan, tampak samping
- Foto kamar mandi, dapur, ruang tamu
- Foto kondisi carport dan pagar
- Info ukuran: LT 120m², LB 54m², 3 kamar, 2 kamar mandi

---

## Langkah 1: Analisis Prioritas (Layer 3 — Reasoning)

**Prompt:**

```
Saya punya rumah warisan usia 22 tahun, tipe 54 di Yogyakarta.
Kondisi: struktural masih bagus, tapi secara estetika sangat tertinggal.
Masalah yang ada:
- Tampak depan: cat kusam, ornamen plester 90-an, kanopi asbes tua
- Pagar besi lama, bengkok
- Interior: keramik motif 90-an, plafon triplex menguning
- 2 kamar mandi: keramik kecil tua, satu masih jongkok
- Dapur: keramik lama, tidak ada kitchen set

Akan ditinggali sendiri (keluarga 2 orang, belum ada anak).
Budget total: 80-120 juta.
Timeline: mau mulai renovasi dalam 3 bulan.

Bantu saya:
1. Prioritaskan renovasi berdasarkan: keamanan → fungsi → estetika
2. Mana yang paling memberikan dampak besar dengan biaya relatif terjangkau?
3. Mana yang bisa ditunda ke fase 2 nanti?
4. Hal apa yang WAJIB dicek di rumah lama sebelum mulai renovasi apapun?
5. Urutan pengerjaan yang tepat (mana yang harus selesai sebelum yang lain)
```

**Output yang diharapkan dari AI:**

**Prioritas 1 — Wajib Dicek Dulu (sebelum mulai apapun):**
- Kondisi instalasi listrik (rumah 22 tahun — kabel bisa sudah getas)
- Kondisi pipa air (bocor, korosi, tekanan)
- Kondisi rangka atap (cek rembes, kondisi kayu/baja ringan)
- Kondisi pondasi dan dinding (retak struktural vs. retak rambut biasa)

**Prioritas 2 — Untuk Ditinggali Segera (dampak fungsi):**
- Kamar mandi (ganti ke duduk, tile baru, shower) — kenyamanan harian
- Dapur (minimal kitchen set sederhana, tile baru)
- Plafon (kalau ada yang rusak atau bocor)
- Instalasi listrik (kalau hasil cek ada masalah)

**Prioritas 3 — Estetika Signifikan (dampak visual besar):**
- Tampak depan + pagar + carport
- Cat seluruh interior

**Bisa Ditunda ke Fase 2:**
- Keramik lantai interior (mahal, bongkar dulu keramik lama — disruptif)
- Interior custom (wardrobe, dll.)

**Urutan Pengerjaan:**
1. Cek & perbaikan kondisi tersembunyi (listrik, pipa, atap)
2. Kamar mandi
3. Dapur
4. Cat interior
5. Tampak depan + pagar + carport
6. Lantai (terakhir, setelah semua pekerjaan kotor selesai)

---

## Langkah 2: Estimasi Biaya Per Prioritas

**Prompt:**

```
Berdasarkan analisis prioritas tadi, buat estimasi kasar biaya per fase
untuk renovasi rumah 54 m² di Yogyakarta.

Fase 1 (wajib segera): 2 kamar mandi + dapur + cat interior + inspeksi kondisi tersembunyi
Fase 2 (tambahan): tampak depan + pagar + carport

Untuk tiap fase, buat estimasi tabel per item pekerjaan.
Kualitas material: menengah.
Lokasi: Yogyakarta (referensi harga upah dan material Jogja 2025-2026).

Sertakan:
- Range per item (bukan angka tunggal)
- Total per fase
- Total keseluruhan
- Asumsi
- Warning untuk hal yang bisa membuat biaya naik
- Disclaimer validasi survey
```

**Output contoh (Fase 1):**

| Item | Volume | Satuan | Range/Satuan | Range Total |
|------|--------|--------|--------------|-------------|
| Inspeksi listrik + perbaikan minor | 1 | paket | 1,5 - 4 juta | 1,5 - 4 juta |
| Renovasi KM 1 (bongkar, keramik baru, closet duduk, shower) | 2x2m | paket | 8 - 14 juta | 8 - 14 juta |
| Renovasi KM 2 (idem, skala lebih kecil) | 1,5x2m | paket | 6 - 10 juta | 6 - 10 juta |
| Dapur: tile dinding, tile lantai, kitchen set sederhana | 3x3m | paket | 12 - 22 juta | 12 - 22 juta |
| Cat interior (2 lapis, wall sealer + cat) | 150 m² | m² | 35.000 - 55.000 | 5,3 - 8,3 juta |
| Plafon: perbaikan area bermasalah | 20 m² | m² | 80.000 - 130.000 | 1,6 - 2,6 juta |
| **Subtotal** | | | | **34,4 - 60,9 juta** |
| Overhead kontraktor 15-20% | | | | 5,2 - 12,2 juta |
| Contingency 10% | | | | 3,4 - 6,1 juta |
| **Total Fase 1** | | | | **Rp 43 - 79,2 juta** |

*Catatan: Renov kamar mandi adalah item yang paling fluktuatif. Kondisi pipa & struktur lama yang baru terlihat saat bongkar sering jadi surprise cost.*

---

## Langkah 3: Brief Renovasi untuk Kamar Mandi

**Prompt (lebih spesifik untuk area prioritas):**

```
Buat brief detail renovasi kamar mandi 1 (ukuran 2x2m):
- Dari: closet jongkok, keramik kecil tahun 90-an, tidak ada shower
- Ke: closet duduk modern, keramik 30x60 atau 60x60, shower head, wastafel sederhana

Gaya: bersih, minimalis, warna netral
Budget kamar mandi 1: maksimal 14 juta

Brief harus mencakup:
1. Daftar pekerjaan yang perlu dilakukan (bongkar, pasang, finishing)
2. Spesifikasi material yang direkomendasikan
3. Apa yang perlu ditanyakan ke tukang sebelum mulai
4. Hal yang sering jadi masalah di renovasi kamar mandi lama
5. Pertanyaan kunci untuk kontraktor: kondisi pipa eksisting
```

---

## Langkah 4: Konten Before-After untuk Dokumentasi

**Prompt:**

```
Saya selesai renovasi kamar mandi rumah lama saya dan ingin mendokumentasikannya
untuk media sosial — bukan untuk jual, tapi untuk berbagi pengalaman.

Before: kamar mandi lama 90-an, jongkok, keramik kecil kuning-hijau tua
After: closet duduk, keramik abu 60x60, shower nikel hitam, cermin simple

Buat:
1. Caption Instagram yang personal dan informatif (bukan iklan properti)
   - Cerita tentang proses, bukan produk
   - Informasi berguna untuk orang yang mau renovasi
   - Soft mention biaya range (bukan angka pasti)
2. 3 tips renovasi kamar mandi yang saya pelajari dari pengalaman ini
```

---

## Langkah 5: Validasi Manusia

Sebelum Bu Sinta mulai konstruksi:

**Cek wajib sebelum tanda tangan kontrak:**
- [ ] Kontraktor sudah survey fisik seluruh area yang akan direnovasi
- [ ] Listrik sudah dicek teknisi listrik (bukan hanya kontraktor umum)
- [ ] Kondisi pipa air sudah dicek — ada rencana penanganan jika ada yang rusak
- [ ] Scope pekerjaan tertulis jelas dalam SPK/kontrak
- [ ] Ada klausul untuk kondisi tak terduga (tambahan biaya maksimal berapa?)
- [ ] Jadwal pembayaran termin (jangan bayar lebih dari 30% di awal)
- [ ] Referensi proyek kontraktor sudah dicek (minimal 1-2 referensi yang bisa dihubungi)

---

## Pelajaran dari Workflow Ini

1. **Rumah lama = lebih banyak hal tersembunyi.** Estimasi AI lebih sering meleset untuk rumah lama karena kondisi eksisting tidak terlihat dari foto. Alokasikan contingency lebih besar (15-20% bukan 10%).

2. **Prioritas fungsi sebelum estetika.** Renovasi kamar mandi dan dapur memberikan dampak kenyamanan harian yang jauh lebih besar daripada tampak depan yang cantik — terutama untuk rumah yang akan ditinggali.

3. **Urutan pengerjaan itu penting.** Renovasi lantai sebelum kamar mandi selesai = buang uang. AI membantu merencanakan urutan yang tepat.

4. **Budget bisa habis di fase 1.** Penting untuk menetapkan budget per fase dari awal, bukan budget total yang ambigu.

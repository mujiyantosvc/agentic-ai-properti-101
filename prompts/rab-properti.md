# Prompts: RAB dan Estimasi Biaya Properti

Prompt untuk menghasilkan estimasi biaya awal yang realistis — dengan asumsi yang eksplisit dan disclaimer yang tepat.

> **Prinsip RAB Realism Guardrail:** Setiap estimasi yang baik harus menyertakan luas/volume, lokasi, jenis pekerjaan, kualitas material, asumsi upah, range harga, dan disclaimer validasi. Semua prompt di bawah sudah dirancang untuk memenuhi prinsip ini.

---

## Prompt 1: Estimasi RAB Kasar untuk Perencanaan Awal

```
Saya butuh estimasi biaya kasar untuk keperluan perencanaan awal — 
bukan untuk kontrak, tapi untuk tahu apakah ide saya realistis secara finansial.

Data proyek:
- Jenis pekerjaan: [renovasi fasad / renovasi interior / bangun baru / dll.]
- Lokasi: [kota/kabupaten]
- Luas area yang dikerjakan: [X m² atau dimensi spesifik]
- Kondisi eksisting: [baru beli / perlu bongkar dulu / kondisi baik]

Deskripsi pekerjaan (sebisa mungkin spesifik):
- [Item 1]
- [Item 2]
- [Item 3]

Kualitas material: [ekonomis / menengah / premium]
Tahun estimasi: [2025 / 2026]

Format output yang diinginkan:
- Tabel per item pekerjaan: volume, satuan, range harga satuan, range total
- Asumsi yang digunakan (upah, material, overhead)
- Subtotal, overhead, contingency 10%, total range
- 3 hal yang paling berpotensi membuat biaya naik signifikan
- Disclaimer bahwa ini perlu dikonfirmasi kontraktor setelah survey lapangan

PENTING: Gunakan range harga (misal: Rp 50.000 - 80.000/m²), 
bukan angka tunggal. Angka tunggal dari estimasi kasar menyesatkan.
```

---

## Prompt 2: Estimasi Renovasi Ringan (Cat, Keramik, Plafon)

```
Estimasi biaya renovasi ringan untuk:
Lokasi: [kota]
Luas yang direnovasi: [X m² total]

Pekerjaan:
1. Pengecatan dinding interior: [X m²], cat [ekonomis/menengah/premium]
2. Pengecatan plafon: [X m²]  
3. Penggantian keramik lantai: [X m²], keramik [ekonomis/menengah/premium]
4. Penggantian keramik dinding: [X m²]
5. Perbaikan plafon gypsum area [X m²]
6. [tambah item sesuai kebutuhan]

Asumsi yang perlu dipertimbangkan:
- Upah tukang per hari di lokasi tersebut
- Apakah ada pekerjaan bongkar sebelum pasang ulang?
- Biaya angkut material
- Biaya buang puing

Output: tabel rinci per item + total range + asumsi + warning + disclaimer validasi
```

---

## Prompt 3: Estimasi Renovasi Sedang (Kamar Mandi, Dapur)

```
Saya ingin estimasi renovasi kamar mandi / dapur.

Data:
- Area: kamar mandi ukuran [X x X m] / dapur [X x X m]
- Lokasi: [kota]
- Kondisi saat ini: [deskripsi kondisi existing]
- Yang mau dikerjakan:
  [ ] Bongkar keramik lama dan pasang baru
  [ ] Ganti closet jongkok ke duduk (atau sebaliknya)
  [ ] Ganti wastafel / bak cuci
  [ ] Ganti shower
  [ ] Perbaikan instalasi air (pipa, valve)
  [ ] Ganti exhaust fan / ventilasi
  [ ] Perbaikan instalasi listrik (stop kontak, lampu)
  [ ] Cat ulang / waterproofing ulang
  [ ] Kitchen set baru (untuk dapur)
  [ ] Lainnya: [X]
- Kualitas material: [ekonomis/menengah/premium]

Yang perlu disebutkan secara khusus:
- Kondisi pipa eksisting tidak diketahui (seringkali ini yang membuat biaya naik)
- Apakah ada rembes atau kebocoran yang perlu ditangani?

Output: rincian per item, range harga, asumsi, warning untuk surprise cost,
dan disclaimer validasi survey lapangan.
```

---

## Prompt 4: Estimasi Biaya Bangun Baru

```
Saya ingin estimasi biaya bangun rumah baru.

Data:
- Lokasi: [kota/kabupaten]
- Luas bangunan yang direncanakan: [X m²]
- Jumlah lantai: [1/2]
- Jumlah kamar tidur: [X], kamar mandi: [X]
- Spesifikasi kasar:
  - Struktur: beton konvensional
  - Dinding: bata merah / bata ringan (hebel)
  - Atap: [genteng metal/flat beton/hip roof genteng tanah liat]
  - Lantai: keramik [X]
  - Plafon: gypsum / GRC
  - Finishing: [cat tembok standar / lainnya]
  - MEP (listrik, air): standar
- Tidak termasuk: furnitur, AC, interior custom
- Kualitas keseluruhan: [ekonomis / menengah / menengah ke atas]
- Tahun rencana pembangunan: [2025/2026]

Berikan estimasi per komponen:
1. Pekerjaan tanah dan pondasi
2. Struktur (kolom, balok, plat)
3. Pekerjaan dinding
4. Pekerjaan atap
5. Pekerjaan finishing (lantai, plafon, cat)
6. Instalasi MEP (listrik, air bersih, sanitasi)
7. Pekerjaan eksterior (pagar, carport, teras)

Plus: total range, asumsi per komponen, faktor yang bisa membuat naik signifikan,
dan catatan bahwa ini estimasi konseptual sebelum ada gambar kerja.
```

---

## Prompt 5: Estimasi Biaya Renovasi Interior

```
Estimasi biaya renovasi interior [rumah/apartemen].

Data:
- Lokasi: [kota]
- Tipe: [rumah tapak/apartemen]
- Luas total yang direnovasi: [X m²]
- Ruangan yang direnovasi: [ruang tamu, kamar tidur utama, 2 kamar tidur lain, 1 kamar mandi, dapur]

Item pekerjaan interior:
1. Pengecatan ulang semua dinding: [X m²]
2. Penggantian lantai keramik ke [vinyl/granit/karpet]: [X m²]
3. Penggantian plafon gypsum [seluruh/sebagian]: [X m²]
4. Pintu dan kusen baru: [X set]
5. Kitchen set baru ukuran [X meter]
6. Wardrobe built-in kamar utama: [X x X meter]
7. Pencahayaan (downlight, lampu TL): [X titik]
8. AC [tipe/kapasitas]: [X unit]
9. Sanitasi kamar mandi: [sebutkan item spesifik]

Kualitas material: menengah
Lokasi: [kota], untuk referensi harga upah dan material

Output: tabel per item + total range + catatan khusus untuk item yang fluktuatif harganya +
disclaimer bahwa harga material perlu dikonfirmasi ke toko/supplier setempat.
```

---

## Prompt 6: Perbandingan Material

```
Saya perlu memilih antara beberapa pilihan material untuk [item pekerjaan].
Bantu saya membandingkan pilihan dari sisi biaya, daya tahan, dan kesesuaian
untuk kondisi di Indonesia.

Item yang dibandingkan: [keramik vs. granit / gypsum vs. GRC / bata merah vs. hebel / dll.]

Konteks penggunaan: [kamar mandi / ruang tamu / eksterior / dll.]
Iklim: [tropis panas/lembab, curah hujan tinggi]

Untuk tiap pilihan, berikan:
1. Range harga per m² atau unit (material saja, belum termasuk pasang)
2. Kelebihan untuk kondisi Indonesia
3. Kekurangan atau risiko
4. Perkiraan usia material sebelum perlu penggantian
5. Rekomendasi untuk tipe pengguna [budget terbatas / ingin tahan lama / estetika]

Format: tabel perbandingan + rekomendasi akhir dengan alasan
```

---

## Prompt 7: Estimasi Biaya per M² Berdasarkan Tipe Konstruksi

```
Saya butuh referensi biaya konstruksi per m² sebagai benchmark.

Lokasi: [kota]
Periode: [2025/2026]

Berikan estimasi biaya per m² untuk:
1. Bangun baru struktur standard (beton konvensional, finishing ekonomis)
2. Bangun baru finishing menengah
3. Bangun baru finishing premium
4. Renovasi ringan (cat, keramik, plafon)
5. Renovasi sedang (dengan pekerjaan M/E dan bongkar pasang)
6. Renovasi berat (bongkar besar, struktur baru, finishing ulang)

Untuk masing-masing:
- Range biaya per m²
- Apa yang biasanya sudah termasuk
- Apa yang biasanya tidak termasuk
- Faktor yang membuat biaya di luar range normal

Catatan: ini untuk keperluan perencanaan awal, bukan penawaran.
Harga aktual tergantung kondisi spesifik, material yang dipilih,
dan negosiasi dengan kontraktor.
```

---

## Catatan Penting untuk Semua Prompt RAB

Output dari prompt di atas adalah **estimasi konseptual** yang berguna untuk:

✅ Menentukan apakah ide renovasi realistis secara finansial  
✅ Menyiapkan budget planning awal  
✅ Menjadi benchmark saat menerima penawaran dari kontraktor  
✅ Memahami item pekerjaan apa saja yang perlu dianggarkan  

Tidak bisa digunakan untuk:

❌ Dasar kontrak dengan kontraktor  
❌ Pengajuan KPR renovasi  
❌ Jaminan bahwa proyek bisa selesai dengan budget tersebut  
❌ Pengganti survey lapangan dan penawaran resmi  

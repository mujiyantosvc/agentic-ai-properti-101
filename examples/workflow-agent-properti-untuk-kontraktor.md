# Workflow: AI Agent Properti untuk Kontraktor

**Kasus:** Kontraktor renovasi menerima calon klien baru via Instagram, perlu merespons cepat dan profesional sebelum survey lapangan dilakukan.

---

## Konteks

Pak Yudi (44 tahun, kontraktor renovasi residensial Bandung) dapat DM Instagram dari calon klien:

> *"Halo pak, saya mau tanya renovasi kamar mandi dan fasad rumah saya. Kira-kira harganya berapa ya?"*

Masalah yang dihadapi Pak Yudi:
- Sering dapat pertanyaan seperti ini tapi tidak ada info yang cukup
- Kalau kasih angka tanpa info → angkanya ngawur, bisa terlalu murah atau terlalu mahal
- Kalau tidak respons cepat → calon klien sudah hubungi kontraktor lain
- Kalau respons terlalu panjang → calon klien tidak baca

Pak Yudi butuh: sistem yang membantu merespons cepat, mengumpulkan info yang dibutuhkan, dan memberi gambaran awal tanpa berkomitmen pada angka yang belum berdasarkan survey.

---

## Langkah 1: Respons Pertama yang Cepat dan Profesional

**Prompt ke AI:**

```
Saya kontraktor renovasi residensial di Bandung.
Dapat DM dari calon klien: "Mau tanya renovasi kamar mandi dan fasad, berapa?"

Buat template respons pertama yang:
1. Dibalas dalam format WA (informal tapi profesional)
2. Konfirmasi saya terima pesannya dan siap bantu
3. Jelaskan secara singkat kenapa saya perlu info lebih dulu sebelum beri estimasi
   (jangan terkesan males atau menghindari pertanyaan)
4. Minta 4-5 informasi dasar yang paling penting:
   - Lokasi (kota/kecamatan)
   - Ukuran area yang mau direnovasi
   - Kondisi saat ini (foto sangat membantu)
   - Ada budget range yang sudah dipikirkan?
   - Kapan rencananya mau mulai?
5. Undang untuk kirim foto atau video kondisi saat ini

Panjang: maksimal 100 kata, readable di HP
Tone: seperti kontraktor berpengalaman yang profesional, bukan terlalu formal
```

**Output contoh:**

> Halo, terima kasih sudah reach out. Saya siap bantu untuk renovasi kamar mandi dan fasad.
>
> Sebelum saya bisa kasih gambaran biaya, perlu beberapa info dulu biar estimasinya lebih akurat:
> - Lokasi rumahnya di mana? (Kota/kecamatan)
> - Ukuran kamar mandi yang mau direnovasi? (panjang x lebar)
> - Lebar fasad yang mau dikerjakan?
> - Sudah ada gambaran budget? (range oke, tidak perlu angka pasti)
> - Kalau bisa, kirim foto kondisi sekarang — sangat membantu untuk estimasi awal
>
> Setelah dapat info ini, saya bisa kasih gambaran kasar dulu sebelum kita atur jadwal survey. 🙏

---

## Langkah 2: Susun Pertanyaan Klarifikasi yang Lengkap

Setelah respons pertama, calon klien mengirim foto dan info dasar. Pak Yudi butuh checklist pertanyaan yang lebih lengkap untuk dilengkapi sebelum survey.

**Prompt ke AI:**

```
Saya kontraktor renovasi, akan melakukan survey untuk renovasi:
1. Kamar mandi 2 x 2,5 meter
2. Fasad rumah (tampak depan + pagar)

Lokasi: Bandung, rumah tipe 60 usia 10 tahun.
Dari foto yang dikirim klien: kondisi KM keramik lama, closet jongkok.
Fasad: cat pudar, pagar besi lama.

Buatkan:
1. Daftar pertanyaan yang perlu saya tanyakan ke klien SEBELUM survey
   (untuk menghemat waktu survey dan mengidentifikasi potensi masalah lebih awal)
2. Daftar hal yang wajib saya cek saat survey fisik
3. Foto yang perlu saya minta dari klien sebelum survey
4. Red flags yang perlu diwaspadai untuk renovasi KM rumah usia 10 tahun
```

**Output yang diharapkan:**

**Pertanyaan pre-survey ke klien:**
- Apakah pernah ada kebocoran atau rembes di KM atau dinding sekitarnya?
- Closet mau diganti ke duduk atau biarkan jongkok?
- Wastafel mau dipertahankan atau diganti?
- Ada shower sekarang? Kalau iya, mau dipertahankan atau upgrade?
- Air di rumah dari PDAM atau sumur? Ada water heater?
- Untuk fasad: cat mau warna apa? Ada referensi gaya yang sudah dipikirkan?
- Pagar mau diganti total atau cukup dicat ulang?
- Ada budget range yang bisa dipakai sebagai acuan?

**Checklist wajib saat survey fisik:**
- Kondisi pipa air eksisting (tekan tembok cek rembes tersembunyi)
- Kondisi saluran pembuangan
- Kondisi dinding di sekitar KM (kelembaban, retak)
- Kondisi plafon (kalau di bawah lantai 2 — cek rembes)
- Kondisi instalasi listrik di KM (grounding, posisi stop kontak)
- Untuk fasad: kondisi plester (cek di balik cat yang mengelupas)
- Kondisi pondasi pagar

---

## Langkah 3: Estimasi Kasar Pre-Survey untuk Acuan Diskusi

Pak Yudi ingin memberikan gambaran kasar biaya sebelum survey, agar klien tidak shock saat survey dilakukan.

**Prompt ke AI:**

```
Buat estimasi kasar pre-survey untuk renovasi:
1. Kamar mandi 2 x 2,5 meter di Bandung
   - Bongkar keramik lama
   - Pasang keramik baru (menengah)
   - Ganti closet jongkok ke duduk (menengah)
   - Perbaikan pipa minor (asumsi tidak ada masalah besar)
   - Shower head baru
   - Cat plafon KM

2. Fasad rumah tipe 60 (lebar kira-kira 7 meter)
   - Cat ulang dengan cat eksterior premium
   - Perbaikan plester yang rusak (estimasi 10-15% area)
   - Pagar besi: cat ulang atau ganti hollow (dua opsi)

Lokasi: Bandung, kualitas material menengah, tahun 2025-2026.

PENTING:
- Berikan RANGE, bukan angka tunggal
- Sertakan asumsi yang dipakai
- Sertakan: "ini estimasi pre-survey, bisa berubah setelah cek kondisi lapangan"
- Sertakan: kondisi apa yang bisa membuat biaya naik signifikan

Tujuan: angka yang bisa saya share ke klien sebagai gambaran awal,
bukan angka yang akan saya gunakan sebagai dasar kontrak.
```

---

## Langkah 4: Template Proposal Awal Setelah Survey

Setelah survey dilakukan, Pak Yudi butuh template proposal yang bisa diisi dan dikirim dalam waktu 24-48 jam.

**Prompt ke AI:**

```
Buat template dokumen proposal renovasi yang profesional untuk kontraktor kecil-menengah.
Proposal untuk: renovasi kamar mandi + fasad rumah tinggal.

Template harus mencakup:
1. Header (nama kontraktor, tanggal, untuk klien siapa)
2. Ringkasan proyek (apa yang akan dikerjakan, lokasi, estimasi waktu)
3. Scope pekerjaan detail (per area, per item pekerjaan)
4. Material yang digunakan (nama material, spesifikasi, toko/brand)
5. Estimasi biaya per item (tabel: item, volume, satuan, harga satuan, total)
6. Total biaya + pajak
7. Jadwal pembayaran termin (saran umum untuk renovasi)
8. Estimasi waktu pengerjaan
9. Yang tidak termasuk dalam scope (untuk hindari dispute)
10. Catatan kondisi lapangan yang perlu diperhatikan
11. Syarat dan ketentuan singkat
12. Tanda tangan persetujuan

Format: Word-friendly, bisa diisi bagian kosong
Sertakan catatan: "Proposal ini berlaku 14 hari sejak tanggal dikeluarkan"
```

---

## Langkah 5: Konten Portofolio untuk Media Sosial

Setelah proyek selesai, Pak Yudi bisa membuat konten portofolio.

**Prompt ke AI:**

```
Saya kontraktor yang baru selesai mengerjakan renovasi kamar mandi + fasad rumah.
Punya 5 foto before dan 5 foto after.
Durasi proyek: 3 minggu. Nilai proyek: 45-50 juta.
Lokasi: Bandung Selatan.

Buat konten untuk profil Instagram kontraktor:

1. Caption foto after kamar mandi (single post)
   - Informasi yang berguna untuk calon klien
   - Mention scope pekerjaan secara natural
   - Soft CTA untuk tanya/konsultasi
   - Tidak menyebut harga spesifik proyek ini

2. Caption carousel before-after fasad (3 foto before + 3 foto after)
   - Ceritakan proses singkat (persiapan → pengerjaan → hasil)
   - Apa lesson learned atau tips dari proyek ini
   - Ajakan untuk diskusi kebutuhan serupa

3. Tips konten 1: "3 hal yang sering luput saat renovasi kamar mandi"
   - Berdasarkan pengalaman nyata proyek ini (generalized)
   - Format carousel 4-5 slide
```

---

## Etika Kerja Kontraktor dengan AI

Workflow ini membantu kontraktor bekerja lebih efisien — tapi ada beberapa hal yang tidak boleh dikompromikan:

### Survey Lapangan Wajib Sebelum Angka Final

Tidak ada estimasi AI yang bisa menggantikan survey fisik. Kondisi pipa tersembunyi, struktur dinding, kondisi instalasi yang tidak terlihat dari foto — semua ini hanya bisa dideteksi di lapangan.

**Jangan pernah membuat kontrak berdasarkan estimasi pre-survey saja.**

### Transparansi ke Klien

Jika ada kondisi yang baru ditemukan saat konstruksi berlangsung dan membutuhkan biaya tambahan:
- Informasikan segera, jangan tunggu sampai proyek selesai
- Jelaskan kondisinya dengan foto atau video
- Dapatkan persetujuan tertulis sebelum lanjutkan pekerjaan tambahan

### Jangan Over-promise untuk Mendapatkan Proyek

AI bisa membantu membuat proposal yang terlihat profesional dan menarik — tapi isi proposal harus realistis. Jangan cantumkan timeline yang tidak bisa dipenuhi atau harga yang tidak bisa dipertahankan hanya untuk menang tender.

### Portofolio Harus Foto Nyata

Tidak boleh menggunakan rendering AI atau foto orang lain sebagai "portofolio" pekerjaan kamu. Ini bisa menyesatkan klien dan merusak kepercayaan jangka panjang.

---

## Checklist Sebelum Mulai Pekerjaan

Sebelum tanda tangan SPK dan terima uang muka:

- [ ] Survey lapangan sudah dilakukan
- [ ] Scope pekerjaan tertulis jelas dan disetujui klien
- [ ] Material yang digunakan spesifik (brand, tipe, ukuran)
- [ ] Jadwal pembayaran termin tertulis
- [ ] Ada klausul untuk pekerjaan tambahan yang tidak terduga
- [ ] Estimasi waktu pengerjaan realistis
- [ ] SPK/kontrak ditandatangani kedua pihak
- [ ] Foto kondisi before sudah diambil sebagai dokumentasi

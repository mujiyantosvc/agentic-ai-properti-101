# Workflow: AI Agent Properti untuk Agen

**Kasus:** Agen properti dengan 6 listing aktif ingin membuat konten yang lebih baik dan sistem follow-up lead yang lebih efisien — tanpa harus hire tim marketing.

---

## Konteks

Reza (29 tahun, agen properti independen di Surabaya) punya 6 listing aktif, rata-rata 8-12 leads masuk per minggu lewat Instagram dan WhatsApp. Masalahnya:

- Konten listing semua terlihat sama — foto + spesifikasi + harga
- Follow-up leads tidak konsisten — kadang cepat, kadang terlupakan
- Deskripsi tiap properti pakai template yang sama persis
- Tidak ada sistem untuk mengetahui leads mana yang lebih hot

Tujuan: Bangun sistem kerja dengan AI yang bisa diulang untuk tiap listing baru, dan lebih efisien dalam mengelola leads.

---

## Bagian 1: Paketkan Tiap Listing

### Langkah 1: Siapkan Data Listing

Untuk tiap listing, kumpulkan:
- Spesifikasi teknis (LT, LB, kamar, fasilitas)
- Foto (minimal 5 foto representatif)
- Keunggulan unik yang tidak ada di listing lain
- Target pembeli (siapa yang paling mungkin beli ini)
- Cerita atau konteks properti (kalau ada yang menarik)

### Langkah 2: Buat Deskripsi Listing yang Berbeda

**Prompt:**

```
Saya agen properti. Buat deskripsi listing untuk properti berikut yang
TIDAK terlihat seperti template generik:

Data properti:
- Tipe: rumah 2 lantai, LT 150m², LB 180m²
- Lokasi: Rungkut Asri, Surabaya Timur
- Kamar tidur: 4, kamar mandi: 3
- Fasilitas: garasi 2 mobil, taman belakang, dapur kering+basah terpisah
- Kondisi: second, usia 8 tahun, terawat baik, semi-furnish (kitchen set + water heater)
- Keunggulan spesifik: taman belakang jarang ada di cluster ini,
                        lokasi pojok (hook), dekat pintu tol MERR 5 menit

- Harga: Rp 1.650.000.000 (bisa KPR)
- Status: SHM + IMB lengkap
- Target pembeli: keluarga profesional, dual income, anak 1-2

Deskripsi harus:
- Mulai dari sesuatu yang konkret dan spesifik, bukan "rumah mewah di lokasi strategis"
- Menyebutkan taman belakang sebagai elemen emosional (ruang main anak, BBQ keluarga)
- Faktual, semua yang disebutkan bisa diverifikasi
- Panjang: 200-250 kata
- Akhiri dengan ajakan kunjungan yang natural
```

### Langkah 3: Buat Set Konten per Listing

**Prompt:**

```
Dari listing Rungkut Asri tadi, buat paket konten lengkap:

1. Tiga variasi caption Instagram:
   - Versi A: hooks ke keluarga muda profesional (dual income, anak kecil)
   - Versi B: hooks ke investor yang ingin disewakan
   - Versi C: fokus pada keunggulan lokasi (akses tol, fasilitas sekitar)

2. Script TikTok/Reels 30 detik — tur singkat dengan narasi
   Struktur: hook → masalah umum keluarga Surabaya → solusi (properti ini) → CTA ringan

3. FAQ untuk listing ini (7 pertanyaan yang paling sering muncul untuk tipe properti ini):
   - Format: pertanyaan + jawaban singkat
   - Sertakan satu pertanyaan tentang KPR

4. Template pesan pertama untuk membalas DM yang hanya tulis "Halo mau tanya rumahnya"
```

---

## Bagian 2: Sistem Follow-up Lead

### Langkah 4: Buat Sistem Kategorisasi Lead

**Prompt:**

```
Bantu saya buat kriteria kategorisasi leads untuk agen properti.

Kategori:
- HOT: kemungkinan akan serius dalam 1-2 minggu
- WARM: serius tapi masih riset/pertimbangkan, timeline 1-3 bulan
- COLD: hanya window shopping atau timeline sangat panjang/tidak jelas

Untuk tiap kategori, berikan:
1. Sinyal yang menunjukkan lead ada di kategori ini
   (berdasarkan pertanyaan atau perilaku mereka)
2. Frekuensi follow-up yang tepat
3. Jenis informasi yang paling berguna dikirim
4. Kapan sebaiknya pindahkan ke kategori lain
5. Kapan sebaiknya berhenti follow-up

Sertakan juga: pertanyaan kualifikasi yang bisa ditanyakan di awal
tanpa terkesan langsung "jualan"
```

**Output yang diharapkan:**

**Sinyal HOT Lead:**
- Tanya jadwal kunjungan spesifik
- Tanya proses KPR atau syaratnya
- Tanya apakah harga bisa dikurang dan berapa min
- Menyebut timeline: "bulan depan pindah", "kalau deal bisa segera"
- Kirim foto KTP atau bertanya tentang booking fee

**Sinyal WARM Lead:**
- Tanya foto lebih banyak atau video
- Tanya harga saja tanpa follow-up lanjutan
- Tanya fasilitas detail tapi tidak ada response setelah info dikirim
- Minta denah
- Sudah kunjungan tapi "masih pikir-pikir"

**Sinyal COLD Lead:**
- Hanya tanya harga lalu diam
- Jawab "nanti ya" untuk jadwal kunjungan
- Timeline: "mungkin tahun depan"
- Tidak balas setelah 2 kali follow-up

### Langkah 5: Buat Template Follow-up per Kategori

**Prompt:**

```
Buat template follow-up WhatsApp untuk tiap kategori lead di bawah ini.
Properti yang ditawarkan: rumah Rungkut Asri (2 lantai, 4KT, taman belakang, 1.65M).

Template yang dibutuhkan:

1. HOT LEAD — setelah kunjungan 2 hari lalu, belum ada keputusan
   Tujuan: dorong secara lembut, beri informasi tambahan yang relevan

2. WARM LEAD — sudah minta foto/video 5 hari lalu, belum ada respons
   Tujuan: re-engage tanpa terkesan mengejar

3. COLD LEAD — tanya harga 2 minggu lalu, tidak ada kabar
   Tujuan: one last touch yang ringan, kalau tidak respons, stop dulu

4. Setelah kunjungan yang berakhir dengan "kami akan diskusikan dulu"
   Tujuan: follow-up setelah 3 hari, natural, tidak memaksa

Untuk tiap template:
- Tone: personal, bukan copy-paste template yang terasa robot
- Panjang: 60-90 kata maksimal (pesan WA yang terlalu panjang sering tidak dibaca)
- Harus ada: satu informasi atau nilai baru (bukan hanya "sudah ada keputusan?")
```

---

## Bagian 3: Etika yang Tidak Boleh Dilanggar

Workflow ini membantu efisiensi — tapi ada batas yang tidak boleh dilanggar:

### Jangan Manipulasi Informasi Properti

- Semua data dalam listing (luas, kamar, fasilitas, harga, legalitas) **harus akurat dan bisa diverifikasi**
- Jangan sebut "strategis", "mewah", atau "eksklusif" tanpa konteks konkret
- Jangan sembunyikan kelemahan properti yang signifikan (dekat SUTET, kondisi banjir, sengketa, dll.)

### Jangan Ciptakan Urgensi Palsu

- "Unit terakhir!" padahal masih ada 3 lainnya
- "Harga naik minggu depan" tanpa dasar
- "Ada calon pembeli lain yang serius" sebagai tekanan

### Privasi Data Lead

- Data leads (nama, nomor, kebutuhan) adalah informasi pribadi
- Jangan sharing data lead ke pihak lain tanpa izin
- Simpan data dengan aman

### Disclosure

- Jika AI membantu menulis konten, tidak ada kewajiban untuk disclose — tapi konten harus tetap **akurat secara faktual**
- Yang tidak boleh: biarkan AI mengarang fakta properti yang tidak kamu verifikasi

---

## Hasil yang Bisa Diukur

Dengan workflow ini, Reza bisa:
- Produksi konten 6 listing dalam satu sesi kerja 3-4 jam (vs. biasanya 2-3 hari)
- Punya template follow-up yang konsisten dan tidak terasa spam
- Mengalokasikan energi ke HOT leads, tidak habis waktu untuk COLD leads
- Bisa onboard listing baru lebih cepat karena ada sistem yang bisa diulang

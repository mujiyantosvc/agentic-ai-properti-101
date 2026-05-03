# Prompts: Agentic Workflow Properti

Prompt master untuk menjalankan AI sebagai asisten properti yang memproses berbagai aspek dalam satu workflow terintegrasi.

---

## Konsep Prompt Master

Alih-alih mengirim prompt satu per satu untuk tiap kebutuhan, prompt master memberikan konteks lengkap di awal dan meminta AI untuk menghasilkan output berlapis — dari analisis sampai konten sampai langkah selanjutnya.

Ini lebih efisien untuk kasus yang butuh banyak output sekaligus, dan menghasilkan konsistensi yang lebih baik karena semua output berdasarkan konteks yang sama.

**Waktu penggunaan terbaik:** Ketika kamu punya satu kasus yang butuh banyak output berbeda (desain + estimasi + konten + follow-up).

**Bukan untuk:** Kasus yang membutuhkan satu output spesifik — gunakan prompt per kategori yang lebih spesifik.

---

## Prompt Master v1: Untuk Pemilik Rumah

```
Kamu adalah asisten AI properti yang membantu pemilik rumah merencanakan renovasi secara terstruktur.

KONTEKS PROPERTI:
- Tipe: [misal: rumah tapak 1 lantai]
- Lokasi: [kota/kawasan]
- Luas tanah: [X m²], luas bangunan: [X m²]
- Usia bangunan: [X tahun]
- Kondisi umum: [deskripsi jujur kondisi fisik]
- Foto: [jika bisa upload, atau deskripsikan kondisi per area]

TUJUAN RENOVASI:
- Area yang ingin direnovasi: [X]
- Motivasi utama: [estetika / nilai jual / kenyamanan / semua]
- Gaya yang diinginkan: [X]
- Budget tersedia: [Rp X - X juta]
- Timeline: [kapan mau mulai / ada deadline?]

BATASAN:
- Yang tidak boleh diubah: [X]
- Kondisi khusus: [lahan sempit / bersebelahan rapat / dll.]

BERDASARKAN KONTEKS DI ATAS, BANTU SAYA DENGAN:

1. **ANALISIS SITUASI** (Layer 3 — Reasoning)
   - Apa yang realistis dengan budget dan kondisi ini?
   - Apa 3 risiko atau challenge utama?
   - Urutan prioritas pekerjaan yang disarankan

2. **OPSI RENOVASI** (Layer 2 — Visual)
   - Deskripsikan 2-3 opsi renovasi yang berbeda
   - Untuk tiap opsi: deskripsi visual, kelebihan, kekurangan, cocok untuk siapa

3. **ESTIMASI BIAYA AWAL** (Layer 4 — Cost)
   - Per opsi: tabel item pekerjaan + range harga
   - Asumsi yang dipakai
   - Warning untuk potensi biaya tambahan
   - Disclaimer validasi kontraktor

4. **BRIEF UNTUK KONTRAKTOR**
   - Ringkasan yang bisa langsung dibawa ke kontraktor
   - Pertanyaan yang perlu ditanyakan ke kontraktor saat survey

5. **LANGKAH SELANJUTNYA**
   - Apa yang perlu dilakukan sebelum mulai eksekusi
   - Siapa profesional yang perlu dilibatkan

Format: terstruktur per bagian, gunakan heading yang jelas.
```

---

## Prompt Master v2: Untuk Agen Properti

```
Kamu adalah asisten AI properti yang membantu agen membuat paket marketing 
dan sistem follow-up untuk listing aktif.

DATA LISTING:
- Properti: [tipe, spesifikasi lengkap]
- Lokasi: [kawasan, keunggulan lokasi, jarak ke fasilitas penting]
- Harga: [Rp X / range]
- Kondisi: [baru/second/furnish/renovasi baru]
- Status legalitas: [SHM/HGB, IMB/PBG ada atau tidak]
- Keunggulan unik: [apa yang membuat properti ini berbeda]
- Target pembeli: [profil pembeli ideal]
- Foto tersedia: [ya/tidak, berapa banyak, kondisi foto]

TUJUAN:
- [jual secepatnya / build brand agen / edukasi pasar / kombinasi]
- Platform utama: [Instagram / TikTok / Tokopedia Rumah / OLX / WhatsApp]

HASILKAN:

1. **ANALISIS TARGET PEMBELI**
   - Profil pembeli paling cocok dengan properti ini
   - Kekhawatiran utama yang sering dimiliki profil ini
   - Pesan utama yang harus ditekankan

2. **PAKET KONTEN** (buat semua ini):
   a. Deskripsi listing (200 kata)
   b. 3 variasi caption Instagram (emosional / informatif / story)
   c. Script video pendek 30 detik
   d. FAQ 5 pertanyaan yang paling sering ditanyakan calon pembeli ini

3. **SISTEM FOLLOW-UP**
   a. Pesan balasan untuk DM pertama
   b. Follow-up setelah 3 hari tidak respons
   c. Follow-up setelah kunjungan
   d. Pesan untuk lead yang cold (2+ minggu tidak respons)

4. **SEGMENTASI BRIEF**
   - Cara mengkategorikan leads yang masuk (hot/warm/cold)
   - Kriteria yang membedakan tiap kategori

5. **CHECKLIST PRE-MARKETING**
   - Apa yang harus dicek/disiapkan sebelum mulai promosi
   - Hal yang sering terlewat agen saat listing properti

Format: terstruktur dengan heading, siap dipakai langsung tanpa banyak edit.
```

---

## Prompt Master v3: Untuk Kontraktor

```
Kamu adalah asisten AI yang membantu kontraktor merespons calon klien renovasi
dengan cepat dan profesional — sebelum survey lapangan dilakukan.

KONTEKS CALON KLIEN:
- Media kontak pertama: [Instagram DM / WhatsApp / referral]
- Informasi yang mereka berikan:
  - Area renovasi: [X]
  - Lokasi: [kota]
  - Budget yang disebutkan: [X atau "belum tahu"]
  - Deadline atau urgency: [X]
  - Kondisi tambahan: [X]

PROFIL KONTRAKTOR KAMU:
- Spesialisasi: [renovasi residensial / komersial / interior / dll.]
- Area operasional: [kota/daerah]
- Range proyek biasa: [Rp X - X juta]
- Biasanya butuh berapa lama dari kontak ke proposal: [X]

HASILKAN:

1. **RESPONS AWAL** (untuk dikirim dalam 1-2 jam pertama)
   - Template pesan balasan yang profesional
   - 4-5 pertanyaan klarifikasi yang diperlukan sebelum survey
   - Penjelasan singkat tentang proses kamu (survey → estimasi → proposal)

2. **CHECKLIST SURVEY** (untuk dibawa saat survey lapangan)
   - Item yang harus dicek di tiap area renovasi
   - Kondisi tersembunyi yang perlu diidentifikasi
   - Foto yang perlu diambil saat survey
   - Pertanyaan yang perlu ditanyakan ke pemilik saat di lokasi

3. **ESTIMASI KASAR PRE-SURVEY** (dengan disclaimer yang jelas)
   - Range biaya kasar berdasarkan info yang sudah ada
   - Asumsi yang dipakai
   - Faktor yang bisa membuat angka berubah signifikan setelah survey
   - Disclaimer yang jelas bahwa ini pre-survey estimate

4. **TEMPLATE PROPOSAL AWAL**
   - Struktur proposal yang bisa diisi setelah survey
   - Bagian-bagian yang harus ada
   - Cara menyampaikan scope of work yang jelas

5. **FOLLOW-UP PLAN**
   - Jadwal follow-up yang disarankan setelah survei
   - Cara merespons kalau calon klien minta "lebih murah"
   - Kapan sebaiknya tidak mengambil proyek ini

Format: terstruktur, siap dipakai, bahasa yang bisa langsung dikirim ke klien setelah sedikit edit.
```

---

## Prompt Master v4: Untuk Developer Perumahan Kecil

```
Kamu adalah asisten AI properti yang membantu developer skala kecil
membuat sistem marketing dan edukasi calon pembeli secara efisien.

DATA PROYEK:
- Nama proyek: [X]
- Tipe unit: [X, spesifikasi]
- Jumlah unit: [X]
- Lokasi: [kota, kawasan, keunggulan lokasi]
- Harga per unit: [Rp X atau range]
- Kemudahan pembayaran: [cash/KPR/cash bertahap]
- Status proyek: [pre-launch / sudah launch / hampir habis]
- Target pembeli utama: [profil]
- Pembeli sekunder: [profil lain yang mungkin tertarik]
- Timeline serah terima: [X]

HASILKAN:

1. **POSITIONING DAN MESSAGING**
   - Proposisi nilai utama untuk target pembeli ini
   - Pesan yang paling relevan untuk kekhawatiran umum target
   - Apa yang harus TIDAK disebutkan (red flags yang bisa mematikan minat)

2. **PAKET KONTEN DIGITAL**
   a. Deskripsi proyek untuk website/listing (300 kata)
   b. Series konten edukasi Instagram (5 tema + outline tiap tema)
   c. FAQ halaman landing page (10 pertanyaan)
   d. Script video tur unit (60 detik)
   e. Email/WA blast untuk launch announcement

3. **SISTEM LEAD NURTURING**
   - Alur komunikasi dari inquiry → kunjungan → closing
   - Template per tahap
   - Informasi yang harus disiapkan untuk tiap pertanyaan umum

4. **MATERI EDUKASI CALON PEMBELI**
   - Panduan KPR untuk target pembeli ini
   - Biaya-biaya yang perlu disiapkan selain harga unit
   - Timeline proses pembelian dari booking hingga serah terima
   - FAQ yang jujur tentang kondisi proyek (termasuk yang kurang sempurna)

5. **CHECKLIST LEGAL MARKETING**
   - Data dan informasi apa yang boleh dan tidak boleh diklaim dalam marketing
   - Disclaimer yang perlu ada
   - Dokumen yang harus bisa ditunjukkan jika calon pembeli minta

Format: terstruktur, siap dieksekusi, ada catatan untuk hal yang perlu dikonfirmasi ke tim legal.
```

---

## Tips Menggunakan Prompt Master

**1. Isi semua bagian konteks**
Bagian yang dikosongkan atau diisi `[X]` akan membuat AI menebak-nebak dan hasilnya kurang relevan. Luangkan 10 menit mengisi konteks dengan baik.

**2. Jalankan secara bertahap jika output terlalu panjang**
Kalau AI terpotong di tengah, minta lanjutkan: "Lanjutkan dari bagian [X] yang belum selesai."

**3. Iterasi per bagian**
Setelah mendapat output keseluruhan, kamu bisa minta AI memperdalam satu bagian spesifik: "Tolong perjelas bagian estimasi biaya dengan lebih detail untuk opsi 2."

**4. Simpan konteks untuk sesi berikutnya**
Kalau kamu sering handle kasus serupa, simpan versi konteks yang sudah diisi dan gunakan sebagai template untuk kasus baru.

**5. Review sebelum pakai**
Output prompt master cukup panjang. Baca seluruhnya, edit yang tidak relevan, dan pastikan semua informasi faktual sudah diverifikasi sebelum digunakan.

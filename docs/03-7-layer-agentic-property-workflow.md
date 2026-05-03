# 03 — 7-Layer Agentic Property Workflow

*Framework untuk memahami bagaimana AI dapat membantu proses properti secara berlapis dan terstruktur.*

---

## Mengapa Perlu Ada Lapisan?

Ketika orang memakai AI untuk properti tanpa framework, yang sering terjadi adalah:
- Hasil bagus tapi tidak bisa diulang
- Tidak tahu kenapa satu prompt berhasil dan yang lain tidak
- Tidak tahu di mana letak masalah ketika hasilnya jelek

**7-Layer Agentic Property Workflow** adalah cara untuk memetakan proses itu secara eksplisit — sehingga kamu tahu di layer mana kamu sedang bekerja, apa yang dibutuhkan di layer itu, dan apa risikonya kalau layer itu dilewati.

Ini bukan proses yang selalu harus diikuti secara kaku dari layer 1 ke 7. Tergantung kasusnya, kamu mungkin mulai dari layer 2, atau hanya butuh layer 4-5 saja. Yang penting adalah kamu tahu ada lapisan-lapisan ini dan apa konsekuensi dari melewati salah satunya.

---

## Ringkasan 7 Layer

| Layer | Nama | Pertanyaan Utama |
|-------|------|-----------------|
| 1 | Context Layer | Siapa yang butuh apa, di mana, dengan budget berapa? |
| 2 | Visual Layer | Seperti apa kondisi dan referensi visualnya? |
| 3 | Reasoning Layer | Apa yang realistis dan apa yang perlu diperhatikan? |
| 4 | Cost Layer | Kira-kira berapa dan apa asumsinya? |
| 5 | Content Layer | Bagaimana mengkomunikasikan ini ke audiens yang tepat? |
| 6 | Lead Layer | Siapa yang paling siap untuk diajak maju? |
| 7 | Human Validation Layer | Apa yang harus dikonfirmasi sebelum keputusan nyata? |

![Diagram 7-Layer Agentic Property Workflow](../assets/7-layer-workflow-diagram.png)

---

## Detail Tiap Layer

### Layer 1: Context Layer

**Fungsi:** Memahami seluruh konteks sebelum AI mulai mengerjakan apapun.

**Pertanyaan utama:**
- Tipe properti apa? (rumah tapak, apartemen, ruko, kos, kavling)
- Lokasi di mana? (kota, iklim, kepadatan, akses)
- Siapa penggunanya? (pemilik sendiri, disewa, dijual)
- Apa tujuannya? (renovasi, bangun baru, jual, beli, konten)
- Berapa budgetnya? (range yang realistis)
- Apa batasan yang tidak boleh dilanggar?

**Input ideal:**
- Property brief (lihat template di [templates/property-ai-brief.md](../templates/property-ai-brief.md))
- Informasi dasar dari klien atau pemilik

**Output:**
- Konteks yang bisa dipakai di semua layer berikutnya
- Daftar pertanyaan klarifikasi jika ada informasi yang kurang

**Risiko jika dilewati:**
- AI menghasilkan output yang tidak relevan dengan situasi nyata
- Estimasi biaya jauh meleset karena tidak ada konteks lokasi
- Rekomendasi desain tidak sesuai dengan iklim atau budaya setempat

---

### Layer 2: Visual Layer

**Fungsi:** Mengumpulkan dan menginterpretasi semua input visual yang relevan.

**Pertanyaan utama:**
- Bagaimana kondisi fisik properti saat ini?
- Apa referensi gaya yang diinginkan?
- Apa yang harus dipertahankan dari kondisi eksisting?

**Input ideal:**
- Foto kondisi eksisting (semua sisi luar, ruangan utama)
- Denah atau sketsa kasar (tidak harus gambar teknis)
- Foto referensi gaya yang diinginkan
- Foto lingkungan sekitar

**Output:**
- Analisis kondisi visual eksisting
- Interpretasi referensi gaya
- Identifikasi elemen yang bisa dipertahankan vs. perlu diubah
- Draft visualisasi opsi desain

**Risiko jika dilewati:**
- Desain yang dihasilkan generik, tidak kontekstual
- AI tidak bisa mendeteksi masalah yang terlihat di foto (cat mengelupas, kondisi atap, dll.)
- Referensi gaya ambigu sehingga output tidak sesuai ekspektasi

**Catatan penting:**
Foto tidak harus bagus secara estetika — yang penting informatif. Foto dari sudut yang menunjukkan kondisi nyata (dengan segala kekurangannya) lebih berguna dari foto yang terlalu di-filter.

---

### Layer 3: Reasoning Layer

**Fungsi:** AI membantu menganalisis kemungkinan, risiko, dan prioritas berdasarkan layer 1 dan 2.

**Pertanyaan utama:**
- Apa yang realistis dilakukan dengan budget dan kondisi ini?
- Apa potensi masalah teknis yang perlu diperhatikan?
- Apa urutan prioritas yang paling masuk akal?
- Apa yang sering salah pada proyek tipe ini?

**Input ideal:**
- Konteks dari layer 1
- Visual dari layer 2
- Pengalaman atau kekhawatiran spesifik dari pemilik/klien

**Output:**
- Analisis opsi yang realistis
- Daftar risiko potensial
- Urutan prioritas pengerjaan
- Pertanyaan yang perlu dijawab sebelum lanjut ke eksekusi

**Risiko jika dilewati:**
- Langsung loncat ke desain atau estimasi biaya tanpa analisis → rawan surprise cost
- Tidak ada pemikiran tentang urutan pekerjaan yang benar
- Masalah struktural atau teknis tidak teridentifikasi sejak awal

**Penting:** Layer ini paling sering dilewati — orang langsung ingin lihat gambar atau dapat angka. Padahal layer ini yang mencegah proyek jadi lebih mahal dari rencana.

---

### Layer 4: Cost Layer

**Fungsi:** Menghasilkan estimasi biaya awal yang membantu mengukur apakah ide realistis secara finansial.

**Pertanyaan utama:**
- Berapa kira-kira biaya untuk setiap opsi yang ada?
- Apa asumsi yang dipakai dalam estimasi ini?
- Di mana risiko biaya yang bisa naik signifikan?
- Apakah budget yang ada cukup untuk tujuan yang diinginkan?

**Input ideal:**
- Scope pekerjaan dari layer 3
- Lokasi (untuk referensi harga material dan upah)
- Kualitas material yang diinginkan (ekonomis, menengah, premium)
- Tahun estimasi (harga material fluktuatif)

**Output:**
- Estimasi biaya per item pekerjaan (dalam range, bukan angka tunggal)
- Asumsi yang digunakan secara eksplisit
- Warning untuk item yang bisa membengkak
- Rekomendasi untuk validasi lebih lanjut

**Risiko jika dilewati:**
- Klien punya ekspektasi biaya yang tidak realistis
- Proyek dimulai tanpa dana yang cukup
- Kontraktor dan klien tidak punya titik awal yang sama untuk negosiasi

**Prinsip penting (RAB Realism Guardrail):**
Estimasi AI yang baik harus selalu disertai: luas/volume, lokasi, jenis pekerjaan, kualitas material, asumsi upah, range harga (bukan satu angka), dan disclaimer validasi. Lebih detail di [docs/06-ai-untuk-rab-dan-estimasi-biaya.md](06-ai-untuk-rab-dan-estimasi-biaya.md).

---

### Layer 5: Content Layer

**Fungsi:** Mengubah informasi yang sudah dikumpulkan di layer 1-4 menjadi materi komunikasi yang siap digunakan.

**Pertanyaan utama:**
- Bagaimana menyampaikan properti ini kepada audiens yang tepat?
- Konten apa yang dibutuhkan dan di platform mana?
- Apa yang membuat properti ini menarik bagi calon pembeli atau penyewa?

**Input ideal:**
- Data properti dari layer 1
- Visual dari layer 2
- Keunggulan dan differensiator dari layer 3
- Konteks harga dari layer 4
- Target audiens yang spesifik

**Output:**
- Deskripsi properti untuk listing
- Caption media sosial (Instagram, TikTok, Facebook)
- Script video pendek
- Artikel blog atau konten edukasi
- FAQ yang menjawab kekhawatiran umum calon pembeli

**Risiko jika dilewati:**
- Konten generik yang tidak menonjolkan keunggulan spesifik
- Pesan yang tidak sesuai dengan audiens target
- Kehilangan momentum dari lead yang masuk karena tidak ada konten follow-up

---

### Layer 6: Lead Layer

**Fungsi:** Mengorganisir dan memprioritaskan calon pembeli atau klien berdasarkan level kesiapan mereka.

**Pertanyaan utama:**
- Siapa yang paling serius dan siap untuk diajak maju?
- Apa pesan yang tepat untuk tiap segmen lead?
- Kapan waktu yang tepat untuk follow-up?
- Bagaimana menghindari kesan terlalu memaksa?

**Input ideal:**
- Data dari form/DM/inquiry yang masuk
- Riwayat interaksi dengan calon pembeli
- Informasi yang sudah mereka tanyakan
- Timeline kebutuhan mereka

**Output:**
- Segmentasi lead (hot/warm/cold)
- Template follow-up yang disesuaikan per segmen
- Jadwal follow-up yang tidak terlalu agresif
- Skrip untuk menjawab pertanyaan umum

**Risiko jika dilewati:**
- Follow-up terlalu random, terlalu sering, atau kurang relevan
- Kehilangan lead yang sebenarnya serius karena tidak di-nurture
- Tidak ada sistem yang bisa diulang ketika leads bertambah

---

### Layer 7: Human Validation Layer

**Fungsi:** Memastikan semua output AI divalidasi oleh manusia yang relevan sebelum dipakai sebagai dasar keputusan nyata.

**Pertanyaan utama:**
- Apa yang perlu diverifikasi sebelum keputusan final?
- Siapa profesional yang perlu dilibatkan?
- Apa yang bisa salah kalau tidak divalidasi?

**Yang harus divalidasi:**
- Struktur bangunan: arsitek atau insinyur sipil
- Estimasi biaya: kontraktor atau quantity surveyor
- Desain teknis: arsitek berlisensi
- Legalitas: notaris, PPJB, AJB, IMB/PBG
- Kondisi lapangan: survey fisik sebelum kontrak
- Material dan harga: konfirmasi langsung ke supplier atau toko

**Risiko jika dilewati:**
- Keputusan diambil berdasarkan data yang salah
- Proyek melebihi budget karena estimasi AI tidak akurat untuk kondisi spesifik
- Masalah hukum dari legalitas yang tidak dicek

---

## Contoh Kasus: Rumah Lama Tipe 45 Ingin Renovasi Tampak Depan

Skenario: Pak Budi punya rumah tipe 45 di perumahan Surabaya, bangunan 2010, mau renovasi tampak depan. Budget 35-55 juta. Tidak mau ubah posisi pagar dan pintu.

### Layer 1 — Context

Input:
```
- Tipe: rumah tapak 1 lantai
- Lokasi: Surabaya (iklim panas, dekat pantai)
- Luas bangunan: 45 m2, luas tanah: 72 m2
- Kondisi: baik secara struktur, cat pudar, fasad terkesan lawas
- Tujuan: estetika + nilai properti
- Budget: 35-55 juta
- Batasan: posisi pagar, pintu utama, carport tidak boleh diubah
- Pengguna: pemilik sendiri, tidak jual
```

Output: AI punya cukup konteks untuk bekerja di layer selanjutnya.

### Layer 2 — Visual

Input: 3 foto (tampak depan, samping kiri, carport area), 5 foto referensi fasad minimalis modern yang Pak Budi suka.

Output: AI mengidentifikasi kondisi cat, jenis plester yang terlihat, model pagar eksisting, orientasi rumah (hadap barat, perlu diperhatikan untuk material fasad).

### Layer 3 — Reasoning

AI menganalisis:
- Cat ulang saja tidak cukup untuk tampak yang signifikan berubah
- Penambahan elemen vertikal (GRC panel, batu alam) di area tertentu bisa beri efek besar tanpa biaya tinggi
- Iklim Surabaya panas: hindari material yang menyerap panas berlebihan di fasad
- Risiko: cat fasad berkualitas rendah akan mengelupas cepat di iklim Surabaya — perlu cat exterior premium

### Layer 4 — Cost

Estimasi kasar (asumsi material menengah, upah Surabaya 2025-2026):

| Item | Estimasi |
|------|----------|
| Pengecatan eksterior (cat premium 2 lapis) | 8-14 juta |
| Plester ulang area rusak | 3-6 juta |
| Panel GRC/roster accent | 8-15 juta |
| Pagar baru (besi hollow, cat powder coating) | 5-12 juta |
| Teras kecil (keramik 2x2m) | 2-4 juta |
| Lampu eksterior | 1-3 juta |
| **Total estimasi** | **27-54 juta** |

*Catatan: angka ini adalah estimasi kasar. Harga aktual tergantung kondisi lapangan, ketersediaan material, dan biaya tukang setempat. Wajib divalidasi kontraktor.*

### Layer 5 — Content (tidak relevan untuk kasus ini)

Pak Budi tidak jual, jadi layer ini dilewati.

### Layer 6 — Lead (tidak relevan untuk kasus ini)

Juga dilewati untuk pengguna pribadi.

### Layer 7 — Human Validation

Pak Budi menggunakan brief + estimasi ini untuk:
1. Mendapatkan 3 penawaran dari kontraktor lokal
2. Mengecek referensi tukang via tetangga
3. Survey lapangan kontraktor untuk cek kondisi plester yang rusak
4. Konfirmasi harga material di toko bangunan setempat
5. Putuskan kontraktor berdasarkan penawaran aktual, bukan estimasi AI

---

## Kapan Tidak Semua Layer Diperlukan

| Kasus | Layer yang Relevan |
|-------|--------------------|
| Pemilik rumah renovasi sendiri | 1, 2, 3, 4, 7 |
| Agen properti buat konten listing | 1, 2, 5, 6 |
| Kontraktor susun proposal | 1, 2, 3, 4, 7 |
| Kreator konten properti | 1, 2, 5 |
| Developer jual unit baru | 1, 2, 4, 5, 6, 7 |
| Calon pembeli riset properti | 1, 3, 4 |

---

## Lanjut ke Praktik

Setelah memahami framework ini, kita akan masuk ke use case konkret di setiap jenis pengguna.

Lanjut ke: [04 — Use Case AI dalam Bisnis Properti](04-use-case-ai-dalam-bisnis-properti.md)

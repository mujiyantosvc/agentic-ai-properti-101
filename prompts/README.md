# Prompts — Panduan Penggunaan

Folder ini berisi kumpulan prompt siap pakai untuk berbagai kebutuhan properti. Semua prompt sudah dirancang dengan konteks Indonesia dan sudah melewati prinsip-prinsip dasar prompt engineering untuk properti.

---

## Cara Memakai Prompt di Sini

1. **Buka file prompt yang relevan** untuk kebutuhan kamu
2. **Pilih prompt** yang paling sesuai dengan situasimu
3. **Sesuaikan bagian dalam kurung kotak `[...]`** dengan informasi nyata
4. **Tempel ke AI** yang kamu gunakan (ChatGPT, Claude, Gemini, dll.)
5. **Review hasilnya** sebelum digunakan — jangan pernah pakai output AI tanpa cek ulang

---

## Prinsip Prompt Properti yang Baik

Setiap prompt yang bagus untuk properti harus mengandung setidaknya beberapa elemen berikut:

### 1. Konteks Siapa dan Untuk Apa

AI tidak tahu kamu siapa dan sedang mengerjakan apa. Berikan konteks minimal:

```
Saya agen properti yang sedang membuat konten listing untuk...
Saya kontraktor yang sedang merespons calon klien...
Saya pemilik rumah yang ingin merencanakan renovasi...
```

### 2. Tipe Properti

Rumah tapak tipe 36 berbeda dengan apartemen studio berbeda dengan ruko 3 lantai. Sebutkan secara spesifik.

### 3. Lokasi

Minimal kota, idealnya kecamatan atau kawasan. Ini mempengaruhi referensi harga, iklim, dan gaya yang relevan.

```
Lokasi: Surabaya Barat
Kawasan: Citraland
Iklim: tropis panas, curah hujan tinggi di musim barat
```

### 4. Gaya atau Tujuan yang Diinginkan

Jangan pakai istilah ambigu seperti "yang bagus" atau "yang modern". Sebutkan gaya spesifik atau referensi:

```
Gaya: minimalis modern tropis
Tone: profesional tapi hangat
Target audiens: pasangan muda 25-35 tahun, first home buyer
```

### 5. Batasan

Apa yang tidak boleh ada, tidak boleh berubah, atau tidak boleh dilakukan:

```
Jangan ubah posisi pintu dan jendela eksisting
Jangan menyebut harga (akan diisi manual)
Jangan pakai istilah teknis yang tidak dipahami awam
Budget terbatas: jangan sarankan material premium
```

### 6. Format Output yang Diinginkan

Tentukan bentuk output yang kamu inginkan:

```
Format: tabel per item pekerjaan dengan range harga
Panjang: maksimal 150 kata
Struktur: hook - value - CTA
Output: 3 variasi caption yang berbeda tone
```

### 7. Validasi dan Disclaimer

Untuk prompt estimasi biaya, selalu minta AI menyertakan asumsi dan disclaimer:

```
Sertakan: asumsi yang digunakan, range harga (bukan angka tunggal),
dan catatan bahwa hasil perlu divalidasi kontraktor/estimator.
```

---

## File yang Tersedia

| File | Kegunaan |
|------|----------|
| [desain-rumah.md](desain-rumah.md) | Prompt eksplorasi visual desain rumah |
| [renovasi-rumah.md](renovasi-rumah.md) | Prompt perencanaan dan visualisasi renovasi |
| [rab-properti.md](rab-properti.md) | Prompt estimasi biaya dan RAB konseptual |
| [marketing-properti.md](marketing-properti.md) | Prompt konten marketing properti |
| [lead-follow-up.md](lead-follow-up.md) | Prompt follow-up calon pembeli/klien |
| [agentic-workflow-properti.md](agentic-workflow-properti.md) | Prompt master workflow agentic properti |

---

## Catatan Penting

- **Selalu edit output** — prompt yang bagus sekalipun menghasilkan output yang perlu disesuaikan
- **Verifikasi angka** — semua estimasi biaya harus dikonfirmasi ke sumber yang relevan
- **Cek fakta properti** — data lokasi, fasilitas, harga harus akurat sebelum dipublikasi
- **Tambahkan sentuhan personal** — output AI sering terasa terlalu "buku teks". Tambahkan suara dan pengalaman kamu sendiri

# Panduan Kontribusi

Terima kasih sudah tertarik untuk berkontribusi ke repository ini. Setiap kontribusi — sekecil apapun — membantu membuat resource ini lebih berguna untuk komunitas properti Indonesia.

---

## Siapa yang Bisa Berkontribusi?

Semua orang yang punya sesuatu yang berguna untuk dibagikan:

- Agen properti yang punya prompt atau workflow yang terbukti efektif
- Kontraktor atau arsitek yang ingin berbagi perspektif teknis
- Developer properti yang punya pengalaman menggunakan AI dalam proses marketing
- Kreator konten yang punya formula konten yang berhasil
- Peneliti atau mahasiswa yang punya insight dari studi tentang AI dan properti
- Developer/programmer yang ingin berkontribusi secara teknis (otomasi, tools)

Tidak perlu jadi ahli AI atau programmer. Kalau kamu punya pengalaman nyata, itu sudah cukup.

---

## Jenis Kontribusi yang Diterima

### 1. Memperbaiki Typo atau Informasi yang Salah

Paling mudah dan selalu dibutuhkan. Kalau kamu menemukan:
- Typo atau salah ketik
- Informasi yang sudah tidak akurat (harga, regulasi, dll.)
- Link yang rusak
- Penjelasan yang membingungkan

Buat pull request dengan perubahan yang jelas dan keterangan singkat kenapa perubahan ini diperlukan.

### 2. Menambahkan Prompt Baru

Kalau kamu punya prompt yang terbukti menghasilkan output yang berguna untuk properti, tambahkan ke file yang relevan di folder `prompts/`.

**Syarat prompt yang bisa diterima:**
- Sudah pernah kamu gunakan dan menghasilkan output yang berguna
- Spesifik untuk kebutuhan properti (bukan prompt generik)
- Ada konteks yang jelas (kapan dan untuk siapa digunakan)
- Tidak mengandung instruksi yang berpotensi menghasilkan konten tidak akurat

### 3. Menambahkan Studi Kasus

Studi kasus dari pengalaman nyata sangat berharga. Yang kami cari:

- Kasus spesifik (bukan cerita umum)
- Ada detail tentang apa yang berhasil dan apa yang tidak
- Ada konteks properti Indonesia (bukan hanya translate dari case Western)
- Jujur tentang batasan dan kegagalan, bukan hanya cerita sukses

Format studi kasus baru: buat file baru di `docs/` atau `examples/` dengan prefix yang sesuai.

### 4. Menambahkan Workflow

Workflow dari pengalaman nyata sangat berguna untuk pembaca yang ingin belajar dari contoh konkret. Tambahkan ke folder `examples/`.

**Standar workflow yang baik:**
- Ada konteks dan skenario yang jelas
- Ada input yang dibutuhkan
- Ada langkah-langkah yang bisa diikuti
- Ada output yang diharapkan
- Ada catatan tentang validasi manusia yang diperlukan

### 5. Menambahkan Referensi

Kalau kamu tahu sumber daya, artikel, riset, atau tools yang relevan dan belum ada di sini, silakan tambahkan dengan penjelasan singkat tentang mengapa berguna.

---

## Aturan Kontribusi

### Wajib Dipatuhi

**1. Konten harus edukatif**
Setiap kontribusi harus punya nilai pembelajaran yang jelas. Tidak ada konten yang semata-mata untuk promosi.

**2. Jangan membuat backlink spam**
Link ke website atau platform pihak ketiga harus relevan dan contextual — bukan daftar link tanpa nilai, bukan anchor text manipulatif. Satu atau dua link yang benar-benar relevan jauh lebih baik dari sepuluh link yang dipaksakan.

**3. Jangan klaim berlebihan**
Hindari klaim yang tidak bisa diverifikasi: "terbukti meningkatkan 50%", "paling efektif", "satu-satunya cara". Kalau ada data, cantumkan sumbernya.

**4. Tidak boleh menyalin konten orang lain**
Semua kontribusi harus orisinil atau merupakan adaptasi dengan atribusi yang jelas. Jangan paste artikel atau konten orang lain tanpa izin.

**5. Verifikasi informasi teknis**
Kalau kontribusimu berisi informasi teknis (harga material, regulasi, proses hukum), pastikan sudah diverifikasi. Informasi yang salah tentang properti bisa merugikan pembaca secara nyata.

**6. Gunakan bahasa Indonesia yang baik**
Konten utama menggunakan Bahasa Indonesia. Istilah teknis yang tidak ada padanannya boleh dibiarkan dalam Bahasa Inggris, tapi penjelasannya dalam Bahasa Indonesia.

### Sangat Disarankan

- Tambahkan contoh nyata, bukan hanya teori
- Sebutkan batasan atau hal yang perlu divalidasi
- Jelaskan konteks Indonesia yang relevan (iklim, budaya, regulasi)
- Gunakan format yang konsisten dengan file-file yang sudah ada

---

## Cara Berkontribusi (Teknis)

### Via Pull Request (Direkomendasikan)

1. Fork repository ini
2. Buat branch baru: `git checkout -b kontribusi/nama-topik`
3. Buat perubahan atau tambahkan file
4. Commit: `git commit -m "docs: tambah prompt untuk [topik]"`
5. Push: `git push origin kontribusi/nama-topik`
6. Buat pull request dengan deskripsi yang jelas

### Via GitHub Issues

Kalau kamu tidak familiar dengan Git/GitHub, kamu bisa:
1. Buka tab Issues di repository ini
2. Buat issue baru dengan label yang sesuai
3. Tuliskan konten atau masukan kamu di sana
4. Maintainer akan meninjau dan mengimplementasikan jika sesuai

### Via Email

Untuk kontribusi yang lebih panjang atau kompleks, kamu bisa kirimkan konten ke maintainer repository.

---

## Proses Review

Semua pull request akan direview sebelum di-merge. Review mencakup:

- Kesesuaian dengan standar konten di atas
- Akurasi informasi teknis yang kritis
- Konsistensi gaya penulisan dengan konten yang sudah ada
- Relevansi untuk audiens utama repository ini

Feedback akan diberikan secara konstruktif. Kalau ada perubahan yang diminta, itu bukan penolakan — hanya perbaikan sebelum konten siap dipublikasikan.

---

## Atribusi

Kontributor yang melakukan perubahan signifikan akan dicantumkan di commit history dan dapat disebutkan di changelog atau catatan release.

Kami tidak bisa menjamin atribusi individual untuk setiap perubahan kecil, tapi semua kontribusi dihargai.

---

## Pertanyaan?

Kalau ada pertanyaan tentang apakah kontribusimu sesuai atau bagaimana cara terbaik berkontribusi, buka issue dengan label "question" — kami dengan senang hati membantu.

---

*Repository ini dikelola secara sukarela. Mohon sabar untuk respons review — semua kontribusi akan ditinjau sebaik mungkin.*

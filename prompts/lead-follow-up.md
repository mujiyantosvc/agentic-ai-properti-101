# Prompts: Lead Follow-up Properti

Prompt untuk mengelola dan menindaklanjuti calon pembeli atau klien dengan cara yang terasa natural — bukan spam, bukan terlalu memaksa.

---

## Prinsip Follow-up yang Baik

Sebelum menggunakan prompt di bawah, ingat beberapa prinsip:

1. **Beri nilai di tiap pesan** — jangan follow-up hanya untuk "mengingatkan". Setiap pesan harus ada informasi atau nilai baru untuk penerimanya.
2. **Sesuaikan dengan tahap lead** — pesan untuk orang yang baru bertanya beda dengan yang sudah kunjungan tapi belum putuskan.
3. **Beri jalan keluar yang mudah** — kalau orang tidak tertarik, biarkan mereka mundur dengan nyaman. Follow-up yang terlalu agresif merusak reputasi.
4. **Pakai nama, sebutkan konteks** — "Hai Pak Budi, melanjutkan obrolan soal rumah di BSD kemarin..." lebih personal dari template kosong.

---

## Prompt 1: Follow-up Lead Baru (Pertama Kali DM)

```
Buat template pesan pertama untuk membalas lead yang baru menghubungi via DM/WA.

Konteks:
- Mereka mengirim: [deskripsi pesan pertama mereka, misal: "Halo, mau tanya soal rumahnya"]
- Platform: [Instagram DM / WhatsApp]
- Properti yang ditanyakan: [deskripsi singkat]

Template yang dibutuhkan:
1. Sambutan yang ramah tapi tidak berlebihan
2. Konfirmasi bahwa kamu siap membantu
3. 2-3 pertanyaan ringan untuk memahami kebutuhan mereka
   (JANGAN langsung tanya budget — terlalu early dan terkesan ingin jualan)
4. Ajak mereka untuk berbagi lebih banyak tentang kebutuhan mereka

Tone: santai tapi profesional, seperti teman yang kebetulan kerja di properti
Panjang: 50-80 kata — jangan terlalu panjang untuk pesan pertama
```

**Contoh output:**

> Hai, terima kasih sudah reach out!
>
> Untuk rumah yang ditanyakan tadi — senang saya bantu. Sebelum saya kasih detail lebih banyak, boleh saya tanya dulu:
>
> Kira-kira sedang cari untuk ditinggali sendiri atau untuk investasi? Dan area mana yang paling cocok untuk aktivitas sehari-hari kamu — kantor, sekolah, atau ada fasilitas tertentu yang jadi prioritas?
>
> Nanti saya bisa sesuaikan info yang relevan buat situasi kamu.

---

## Prompt 2: Follow-up Setelah Tanya Harga

```
Buat pesan follow-up untuk lead yang sudah tanya harga tapi tidak ada respons lanjutan
setelah [2-3 hari].

Konteks:
- Mereka tanya: [apa yang mereka tanyakan]
- Kamu sudah kasih: [apa yang sudah kamu berikan]
- Sudah berapa lama tidak ada respons: [X hari]

Yang diinginkan:
- Tidak terkesan mendesak atau mengejar-ngejar
- Beri informasi tambahan yang berguna, bukan sekadar "sudah ada keputusan?"
- Buka pintu untuk diskusi lebih lanjut atau pertanyaan lain
- Kalau mereka tidak cocok dengan properti ini, tawarkan untuk bantu cari yang lebih sesuai

Tone: santai, tidak ada deadline atau urgensi palsu
Panjang: 60-90 kata
```

**Contoh output:**

> Halo Pak/Bu [nama], semoga kabarnya baik.
>
> Sekedar mau berbagi — minggu ini ada beberapa pertanyaan masuk soal [properti yang sama], jadi saya pikir mungkin ada info yang bisa saya tambahkan yang berguna.
>
> Salah satu yang sering ditanyakan: soal cicilan estimasi kalau KPR 15-20 tahun. Kalau mau saya hitung range-nya berdasarkan harga sekarang, bisa saya kirimkan.
>
> Atau kalau ada hal lain yang mau ditanyakan — atau kalau ini ternyata kurang sesuai kebutuhan — saya siap bantu cari opsi lain yang lebih cocok.

---

## Prompt 3: Follow-up Setelah Minta Desain atau Informasi Tambahan

```
Buat follow-up untuk lead yang sudah minta informasi tambahan
(foto lebih banyak, denah, atau pertanyaan spesifik) tapi belum ada respons setelah dikirim.

Konteks:
- Informasi yang sudah dikirim: [X]
- Kapan dikirim: [X hari yang lalu]

Tujuan:
- Konfirmasi mereka sudah terima info
- Tanya apakah ada pertanyaan lanjutan
- Tidak terkesan mengejar

Tambahkan juga: satu informasi baru yang relevan — update harga, ada unit lain yang baru, atau tips melihat properti yang berguna.
```

---

## Prompt 4: Follow-up Setelah Konsultasi atau Kunjungan

```
Buat pesan follow-up untuk lead yang sudah melakukan kunjungan atau konsultasi,
tapi belum ada keputusan.

Konteks:
- Kapan kunjungan: [X hari lalu]
- Hal yang dibahas / kekhawatiran yang mereka ungkapkan saat kunjungan: [X]
- Status: [masih mempertimbangkan / ada properti lain yang juga dilihat / butuh izin pasangan/ortu]

Pesan harus:
1. Ucapkan terima kasih sudah menyempatkan kunjungan
2. Bahas satu kekhawatiran spesifik yang mereka sampaikan dan berikan informasi tambahan
3. Tawarkan untuk membantu jika ada pertanyaan lanjutan
4. Jangan minta keputusan — biarkan mereka yang mengontrol pace

Jika mereka menyebutkan sedang bandingkan dengan properti lain:
- Jangan jelekkan properti lain
- Fokus pada keunggulan unik properti ini yang relevan dengan kebutuhan mereka yang sudah diketahui

Tone: hangat, profesional, tidak ada tekanan
```

---

## Prompt 5: Follow-up untuk Lead yang Tidak Merespons Lama

```
Buat follow-up untuk lead yang sudah lama tidak merespons (2+ minggu / 1 bulan).

Konteks:
- Terakhir interaksi: [X waktu lalu]
- Status terakhir: [tanya harga / sudah kunjungan / sedang pertimbangkan]

Pendekatan:
- Jangan bertanya "masih berminat?" secara langsung
- Beri kabar terbaru yang relevan (perubahan harga, ketersediaan unit, info baru)
- Buka pintu untuk percakapan baru tanpa terkesan mendesak
- Kalau tidak ada respons setelah ini, stop follow-up dan simpan kontaknya untuk
  future reference

Tone: santai, tidak ada FOMO dipaksakan, tidak ada "ini penawaran terakhir"
Panjang: pendek — 40-60 kata, bukan pesan panjang yang melelahkan
```

**Contoh output:**

> Hai [nama], sudah cukup lama tidak ngobrol.
>
> Ada satu update soal unit yang pernah kamu tanya — harganya ada adjustment kecil bulan ini. Kalau masih relevan, saya bisa kasih info terbaru.
>
> Kalau posisinya sekarang memang belum tepat, juga tidak masalah — simpan nomor saya kalau suatu saat butuh bantuan lagi.

---

## Prompt 6: Segmentasi Leads

```
Bantu saya mengkategorikan dan memprioritaskan leads berikut ini.

List leads (sertakan info yang kamu punya tentang tiap lead):
1. [Nama/inisial]: [kapan kontak, apa yang ditanya, respons terakhir, level engagement]
2. [dst.]

Kategorikan ke dalam:
- HOT: sudah tanya jadwal kunjungan / menyebut waktu yang konkret / bertanya soal proses akad/KPR
- WARM: sudah tanya detail tapi belum konkret soal waktu / minta video/foto tambahan
- COLD: hanya tanya harga dan hilang / tidak ada respons setelah info dikirim

Untuk masing-masing kategori, rekomendasikan:
- Frekuensi follow-up yang tepat
- Tipe konten/informasi yang paling berguna dikirim
- Kapan sebaiknya berhenti follow-up

Tujuan: prioritaskan energi ke leads yang paling siap, jangan habiskan waktu untuk leads yang belum siap secara tidak proporsional.
```

---

## Prompt 7: Membalas Klien Renovasi yang Tanya via DM

```
Buat template membalas calon klien renovasi yang pertama kali menghubungi via DM Instagram.

Mereka mengirim pesan: [copy pesan mereka]
Konteks dari profil/postingan yang mereka lihat: [misal: kontraktor, tukang renovasi, desainer]

Tujuan balasan:
1. Respons cepat yang menunjukkan kamu profesional
2. Klarifikasi kebutuhan mereka (area renovasi, lokasi, gambaran budget)
3. Jelaskan proses awal: survey dulu → estimasi → proposal
4. Undang untuk konsultasi awal / survey

Yang harus dihindari:
- Langsung kasih angka tanpa info yang cukup
- Terlalu panjang untuk pesan pertama
- Terkesan terburu-buru mau "dapat proyek"

Tone: profesional kontraktor, bukan sales
Panjang: 80-100 kata
```

---

## Prompt 8: Follow-up Setelah Closing

```
Buat pesan follow-up pasca-closing untuk menjaga hubungan baik dan mendorong referral.

Konteks:
- Apa yang baru diselesaikan: [jual-beli / selesai renovasi / serah terima unit]
- Kapan: [X waktu lalu]
- Hal yang diingat dari proses: [kalau ada momen yang berkesan]

Pesan harus:
1. Ucapkan selamat atas keputusan/penyelesaian
2. Konfirmasi kesiapan untuk membantu jika ada pertanyaan lanjutan
3. Tanya (dengan cara yang natural): apakah ada teman/keluarga yang mungkin butuh bantuan serupa?
4. Tidak terkesan mengeksploitasi momen closing untuk jualan

Ini bukan pesan minta review — lebih ke menjaga hubungan yang sudah ada.
Panjang: 60-80 kata.
```

---

## Catatan Etis untuk Follow-up

- **Jangan manipulasi**: hindari pesan yang menciptakan urgensi palsu ("ini unit terakhir!", "penawaran berakhir besok!" padahal tidak)
- **Respek keputusan "tidak"**: kalau seseorang bilang tidak tertarik, hargai itu
- **Data pribadi**: simpan data lead dengan aman dan tidak sembarangan dibagikan
- **Akurasi informasi**: semua informasi properti dalam follow-up harus akurat dan bisa dipertanggungjawabkan

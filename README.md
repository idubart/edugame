# 🎮 Genza Education – Petualangan Belajar Kelas IV SD

Website belajar interaktif bergaya game untuk persiapan **Event Kompetisi SAS Kelas IV SD**.
Satu file HTML statis (tanpa framework, tanpa build), jadi mudah di-host di GitHub Pages atau Vercel.

## ✨ Fitur

- 4 mata pelajaran: **Matematika, Pendidikan Pancasila, IPAS, Bahasa Indonesia**
- Materi interaktif: visualisasi pecahan, jam analog, garis bilangan KPK, bangun ruang, daur hidup kupu-kupu, transformasi energi, dan lainnya
- **Petualangan Quiz**: 10 level dengan peta petualangan, skor, streak, konfeti, dan pembahasan
- **Suara**: efek bunyi (Web Audio API) dan pembacaan materi dalam Bahasa Indonesia (Web Speech API)
- Maskot **Foxy 🦊** yang memberi tips belajar
- Responsif untuk HP, tablet, dan laptop

## 🗂️ Struktur

```
genza-education/
├── index.html     # seluruh aplikasi (HTML + CSS + JS)
├── vercel.json    # konfigurasi Vercel
├── .gitignore
└── README.md
```

## 🚀 Menjalankan Lokal

Cukup buka `index.html` di browser. Atau dengan server lokal:

```bash
npx serve .
```

## ☁️ Deploy ke Vercel

1. Push repo ini ke GitHub.
2. Buka https://vercel.com/new dan login dengan GitHub.
3. Import repo `genza-education`.
4. Framework Preset: **Other**. Kosongkan Build Command dan Output Directory.
5. Klik **Deploy**. Setiap `git push` berikutnya otomatis ter-deploy ulang.

## 📖 Panduan Bermain

**Belajar materi**
1. Pilih mata pelajaran di bilah menu atas.
2. Baca kartu materi, lalu klik elemen interaktif (lingkaran pecahan, bangun ruang, tahapan daur hidup, dll.).
3. Tekan tombol **🔊 Dengarkan** untuk mendengar penjelasan.
4. Jawab mini-latihan (misalnya soal buku di Matematika dan soal "Sampah Plastik" di Bahasa Indonesia) untuk mendapat ⭐ di beranda.

**Petualangan Quiz**
1. Buka menu **⚔️ Petualangan Quiz**, tekan **🚀 Mulai Petualangan!**
2. Jawab 10 tantangan (5 Matematika, 2 Pancasila, 2 IPAS, 1 Bahasa).
3. Jawaban benar = 10 poin + bonus 2 poin per streak berturut-turut. Jawaban salah mengulang streak dari 0.
4. Baca pembahasan, tekan **➡️ Lanjut**.
5. Di akhir ada hasil: 🏆 ≥ 80%, 🌟 ≥ 50%, 💪 di bawahnya. Tekan **🔄 Main Lagi** untuk mengulang.

**Tips**
- Tombol 🔊/🔇 (kanan bawah) menyalakan atau mematikan semua suara.
- Klik Foxy 🦊 (kiri bawah) untuk tips belajar.
- Suara bahasa Indonesia bergantung pada voice yang tersedia di browser/perangkat (paling baik di Chrome/Edge).

## 🛠️ Menambah Soal Quiz

Edit array `quizQuestions` di `index.html`:

```js
{
  subject: 'math',
  emoji: '🔢',
  scene: '🏰 Nama Lokasi',
  question: 'Teks soal',
  options: ['A', 'B', 'C', 'D'],
  correct: 0,           // indeks jawaban benar (mulai dari 0)
  explanation: 'Pembahasan'
}
```

## 📄 Lisensi

Hak cipta © Genza Education. Atur lisensi sesuai kebutuhan Anda.

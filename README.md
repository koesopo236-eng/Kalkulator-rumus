# Kalkulator Rumus

Aplikasi kalkulator berisi rumus-rumus siap pakai. Pilih rumus, isi angkanya, langsung dapat hasil. Ringan, tanpa iklan, tanpa internet, dan open source.

## Rumus yang tersedia

- **Geometri**: luas dan keliling lingkaran, luas persegi panjang, luas segitiga, volume tabung, volume bola, Pythagoras
- **Fisika**: kecepatan, gaya, energi kinetik, hukum Ohm, massa jenis
- **Keuangan**: bunga sederhana, bunga majemuk, persentase
- **Aljabar**: persamaan kuadrat

## Cara mencoba

Buka `index.html` di browser HP atau komputer. Tidak perlu install apa pun.

## Menambah rumus baru

Buka `index.html`, cari objek `KATEGORI`, lalu tambahkan entri baru:

```js
{ nama: "Luas trapesium", rumus: "½ × (a + b) × t",
  input: [["a","Sisi sejajar a"],["b","Sisi sejajar b"],["t","Tinggi (t)"]],
  hitung: v => "Luas = " + fmt(0.5 * (v.a + v.b) * v.t) }
```

## Rencana

- [ ] Pencarian rumus
- [ ] Riwayat perhitungan
- [ ] Bungkus jadi aplikasi Android (Capacitor) dan rilis lewat F-Droid
- [ ] Terjemahan bahasa lain

## Berkontribusi

Pull request sangat diterima, terutama untuk rumus baru dan perbaikan bug.

## Lisensi

MIT. Lihat berkas `LICENSE`.

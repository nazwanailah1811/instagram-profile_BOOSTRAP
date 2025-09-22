
# Instagram Profile Clone (Bootstrap 5)

## Struktur File
```
index.html
assets/
  css/custom.css
  img/ (profile.jpg, 1.jpg ... 12.jpg)
```

## Cara Menjalankan
1. Buka file `index.html` di browser (Chrome/Edge/Firefox).  
2. Tampilan akan responsif sesuai ukuran layar.  

## Dependencies
- Bootstrap 5 (CDN).

---

## Jawaban Pertanyaan README

**1. Mengapa memilih konfigurasi col tertentu untuk tiap breakpoint?**  
Agar feed foto tetap rapi dan mudah dibaca di semua device.  
- Mobile: 1 kolom → layar kecil, fokus per foto.  
- Tablet: 2–3 kolom → memanfaatkan ruang lebih luas.  
- Desktop: 4 kolom → optimal untuk layar besar.  

**2. Bagaimana memastikan tombol Follow/Edit Profile tetap mudah dijangkau di mobile?**  
Menggunakan utilitas Bootstrap `order-*` agar tombol bisa berpindah posisi.  
Di mobile tombol muncul di atas/bawah sesuai kenyamanan, di desktop lebih sejajar dengan username.  

**3. Jika postingan bertambah jadi 50, apa potensi masalah dan solusi gridnya?**  
Masalah: halaman akan panjang dan berat di-load.  
Solusi: gunakan **pagination** atau **infinite scroll** (lazy load). Grid Bootstrap tetap bisa dipakai, hanya data yang ditampilkan perlu dibatasi per halaman.  
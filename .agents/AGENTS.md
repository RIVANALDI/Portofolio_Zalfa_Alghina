### CSS Variables for Light/Dark Mode Contrast
Setiap kali mengimplementasikan fitur pertukaran tema (Light/Dark Mode toggle) menggunakan Tailwind CSS:
1. Selalu petakan warna utama (seperti `.text-primary`, `.bg-primary`, `.border-primary`) ke variabel CSS `--primary-color` yang disesuaikan kontrasnya:
   - Mode Terang (Light): Menggunakan warna gelap dengan kontras tinggi (misal: `#0062a1` atau `#3e3ef8`).
   - Mode Gelap (Dark): Menggunakan warna terang (misal: `#9ccaff`).
2. Pastikan efek gradien pudar seperti `from-surface` ditimpa di CSS agar menggunakan variabel `--surface-container` (bukan statis gelap).
3. Selalu periksa apakah `themeToggle` memperbarui kelas ikon secara aman menggunakan `.querySelector('.material-symbols-outlined')` daripada menimpa `.innerText` elemen tombol secara keseluruhan.

### Scope Isolation for Global Scripts
Ketika menambahkan skrip JavaScript di file HTML mentah (raw HTML pages):
1. Selalu bungkus skrip tingkat halaman ke dalam IIFE (Immediately Invoked Function Expression) seperti `(() => { ... })()` atau blok `{ ... }` jika menggunakan deklarasi `const` atau `let`.
2. Hal ini mutlak diperlukan untuk mencegah tabrakan deklarasi global (terutama jika ada skrip inline di bagian `<head>` yang menggunakan nama variabel serupa, seperti `savedTheme` atau `htmlEl`).


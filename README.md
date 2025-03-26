LINK WEB : https://ffaawwaazz.github.io/Undangan-Pernikahan/

# Undangan-Pernikahan

Berikut adalah ringkasan struktur inti dari kode HTML dan CSS yang bisa dimasukkan ke dalam README GitHub:

---

# RD Wedding - Undangan Pernikahan Digital

## Struktur Proyek
Proyek ini adalah undangan pernikahan digital berbasis web statis yang dibuat menggunakan **HTML, CSS, dan JavaScript**. Berikut adalah struktur utama proyek:

### 1. **HTML (`index.html`)**
   - **Header & Navbar:** Menampilkan nama pasangan dan navigasi ke berbagai bagian halaman.
   - **Home Section:** Menampilkan nama pasangan dengan tampilan estetis.
   - **Akad & Resepsi:** Informasi waktu dan lokasi acara dengan gambar pendukung.
   - **Countdown Timer:** Hitungan mundur ke hari pernikahan.
   - **Peta Lokasi:** Embedded Google Maps untuk memudahkan tamu.
   - **Gallery:** Koleksi gambar terkait pernikahan.
   - **RSVP Form:** Formulir untuk konfirmasi kehadiran.
   - **Footer:** Informasi pembuat undangan.

### 2. **CSS (`style.css`)**
   - **Font Import:** Menggunakan font dari Google Fonts (`Inria Serif`, `Style Script`, `Niconne`).
   - **Global Styles:** Reset margin, padding, dan scroll behavior.
   - **Background:** Menggunakan gambar latar tetap dan efek transparansi.
   - **Navbar Styling:** Navbar dengan efek transparan dan shadow.
   - **Content Layout:** Grid dan flexbox untuk penyusunan elemen.
   - **Animations:** Efek hover, animasi garis, dan elemen bergerak.

### 3. **JavaScript (inline di HTML)**
   - **Countdown Timer:** Menghitung waktu mundur menuju hari pernikahan dan menampilkan secara real-time.

## Teknologi yang Digunakan
- **HTML5** untuk struktur halaman
- **CSS3** untuk tampilan dan animasi
- **JavaScript** untuk fitur interaktif (countdown timer)
- **Google Fonts & Icons** untuk estetika teks dan simbol

---

Berikut beberapa penjelasan singkat dari beberapa bagian kode:  

### **1. Navbar (Navigasi)**
```html
<nav class="navbar">
  <div class="navwrapper">
    <h1 class="brand">Aditya & Bella</h1>
    <menu class="navmenu">
      <a href="#home">Home</a>
      <a href="#akad">Akad</a>
      <a href="#resepsi">Resepsi</a>
      <a href="#countdown">Count Down</a>
      <a href="#map">Map</a>
      <a href="#gallery">Gallery</a>
      <a href="#rsvp">RSVP</a>
    </menu>
    <audio controls autoplay>
      <source src="Daniel Brown keys - Last Universe.mp3" type="audio/mpeg" />
    </audio>
  </div>
</nav>
```
🔹 **Fungsi:** Menampilkan navigasi tetap di bagian atas halaman.  
🔹 **Audio:** Musik otomatis dimainkan saat halaman dibuka.  

### **2. Home Section (Judul & Nama Pasangan)**
```html
<section id="home">
  <h2 class="titl">Our Wedding</h2>
  <h1 class="nmtitl">Aditya & Bella</h1>
  <div class="content">
    <div class="c1">
      <h2>Aditya Budi Cahya</h2>
      <h4>Putra dari Bapak Dharma dan Ibu Eka</h4>
    </div>
    <div>
      <h1>|</h1>
    </div>
    <div class="c1">
      <h2>Bella Citra Aulia</h2>
      <h4>Putri dari Bapak Eko dan Ibu Dewi</h4>
    </div>
  </div>
</section>
```
🔹 **Fungsi:** Menampilkan nama pasangan dan latar belakang keluarga mereka.  
🔹 **Struktur CSS:** Dibuat menggunakan flexbox untuk tata letak yang rapi.  

### **3. CSS untuk Background dan Font**
```css
body {
  font-family: "Inria Serif", sans-serif;
  background-image: url("https://images.pexels.com/photos/1323712/pexels-photo-1323712.jpeg");
  background-size: cover;
  background-attachment: fixed;
}
```
🔹 **Fungsi:**  
- Mengatur font utama menggunakan *Google Fonts*.  
- Menampilkan gambar latar belakang yang tetap (tidak bergerak saat scroll).  

### **4. Countdown Timer (Hitung Mundur ke Hari Pernikahan)**
```js
var countDownDate = new Date("Oct 5, 2024 08:00:00").getTime();
var x = setInterval(function () {
  var now = new Date().getTime();
  var distance = countDownDate - now;
  var days = Math.floor(distance / (1000 * 60 * 60 * 24));
  var hours = Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
  var minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));
  var seconds = Math.floor((distance % (1000 * 60)) / 1000);
  document.getElementById("timee").innerHTML = days + "d " + hours + "h " + minutes + "m " + seconds + "s ";
  if (distance < 0) {
    clearInterval(x);
    document.getElementById("timee").innerHTML = "EXPIRED";
  }
}, 1000);
```
🔹 **Fungsi:**  
- Menghitung mundur waktu menuju hari pernikahan.  
- Menampilkan jumlah hari, jam, menit, dan detik yang tersisa.  
- Menampilkan teks **"EXPIRED"** setelah waktu habis.  

---

Itu beberapa penjelasan singkatnya! 😃

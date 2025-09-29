# lab2wab
## Nama : Alya Febrianti
## Kelas : TI.24.A1
## NIM : 312410692

# Praktikum 2: CSS Dasar

## Tujuan

1. Memahami konsep dasar CSS.
2. Memahami aturan penulisan CSS.
3. Memahami penggunaan selector (elemen, class, id).
4. Menerapkan pengaturan CSS pada HTML.

---

## Langkah Praktikum

Seluruh langkah mengikuti instruksi modul, mulai dari membuat HTML, menambahkan internal CSS, inline CSS, eksternal CSS, hingga penggunaan selector ID dan class.

---

## Pertanyaan & Jawaban

### **1. Eksperimen CSS dengan CSS Cheat Sheet**

Eksperimen dilakukan dengan menambahkan properti baru seperti `background`, `font-size`, `text-transform`, dll.

```css
body {
  background-color: #f0f0f0;
  font-family: Arial, sans-serif;
}

h1 {
  font-size: 32px;
  color: darkblue;
  text-align: center;
  text-transform: uppercase;
}

p {
  font-size: 16px;
  color: #333;
  line-height: 1.6;
  margin: 20px;
}
```

📌 Hasil: Tampilan menjadi lebih menarik dengan judul besar biru, paragraf rapi, dan latar belakang abu-abu.

---

### **2. Perbedaan `h1 {...}` dengan `#intro h1 {...}`**

* `h1 { ... }` → berlaku untuk semua elemen `<h1>`.
* `#intro h1 { ... }` → hanya berlaku untuk `<h1>` yang ada di dalam elemen dengan `id="intro"`.

Contoh:

```css
h1 {
  color: blue;
}

#intro h1 {
  color: red;
}
```

```html
<h1>Judul 1</h1>
<div id="intro">
  <h1>Judul 2</h1>
</div>
```

📌 Hasil:

* "Judul 1" → **biru**
* "Judul 2" → **merah**

---

### **3. Prioritas Internal, Eksternal, dan Inline CSS**

Urutan prioritas CSS:

1. **Inline CSS** → tertinggi
2. **Internal CSS**
3. **Eksternal CSS**

Contoh:

```html
<head>
  <link rel="stylesheet" href="style.css"> <!-- Eksternal -->
  <style>
    p { color: green; } <!-- Internal -->
  </style>
</head>
<body>
  <p style="color: red;">Teks ini berwarna apa?</p> <!-- Inline -->
</body>
```

📌 Hasil: teks berwarna **merah** karena inline CSS mengalahkan internal maupun eksternal.

---

### **4. ID vs Class pada CSS**

Selector **ID lebih spesifik** dibandingkan Class, sehingga ID akan menang.

Contoh:

```html
<p id="paragraf-1" class="text-paragraf">Contoh teks</p>
```

```css
#paragraf-1 {
  color: blue;
}

.text-paragraf {
  color: green;
}
```

📌 Hasil: teks berwarna **biru** karena aturan ID (`#paragraf-1`) lebih kuat dibanding class (`.text-paragraf`).

---



<img width="959" height="302" alt="hasil 1" src="https://github.com/user-attachments/assets/b190a6ae-efb5-4690-97ee-6167a00f79e6" />

<img width="950" height="498" alt="hasil" src="https://github.com/user-attachments/assets/f5d96bb2-7688-4c8e-a2b9-bca80d8f41cd" />

<img width="959" height="360" alt="hasil 3" src="https://github.com/user-attachments/assets/f6838f81-eb12-45fe-9ffa-db4f9055a932" />

<img width="959" height="338" alt="hasil 4" src="https://github.com/user-attachments/assets/498479b3-7a62-41e1-90c9-cdf183a379c9" />

<img width="957" height="353" alt="image" src="https://github.com/user-attachments/assets/022d851c-538c-4123-ac56-daa01cca58f7" />

<img width="956" height="399" alt="image" src="https://github.com/user-attachments/assets/57f8922c-12dc-46ee-bc27-29d7207af3cf" />










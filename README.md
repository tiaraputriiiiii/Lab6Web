# Lab6Web

```
Nama    : Tiara Putri
NIM     : 312210064
Kelas   : TI.22.A.1
MATKUL  : Pemrograman Web 1
```

## **Daftar Isi**

**1. [Instruksi Praktikum](#instruksi-praktikum)**  
**2. [Langkah-langkah Praktikum](#langkah-langkah-praktikum)**

## **Instruksi Praktikum**

1. Persiapkan text editor misalnya VSCode.
2. Buat folder baru dengan nama Lab3Web
3. Ikuti langkah-langkah praktikum yang akan dijelaskan berikutnya.
4. Lakukan validasi dokumen html dengan mengakses http://validator.w3.org

## **Langkah-langkah Praktikum**

Berikut adalah langkah-langkah umum untuk membuat sebuah website dengan HTML dan Bootstrap:

**1. Persiapkan Tools dan Lingkungan Kerja:**

Pastikan Anda memiliki teks editor seperti Visual Studio Code, Sublime Text, atau Notepad++ untuk menulis kode.
Unduh Bootstrap dari situs resmi mereka atau gunakan versi Bootstrap dari CDN (Content Delivery Network).
Inisialisasi Proyek:

Buat direktori proyek untuk website Anda.
Buat file HTML baru dan beri nama index.html.
Struktur Dasar HTML:

Mulai dengan kode HTML dasar, termasuk elemen `html`, `head`, dan `body`.
Tambahkan tag <meta> untuk mengatur karakter set dan viewport.
Sisipkan referensi ke Bootstrap CSS di bagian <head>.
html

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <!-- Tambahkan link ke Bootstrap CSS -->
    <link
      href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css"
      rel="stylesheet"
    />
    <title>Nama Website Anda</title>
  </head>
  <body>
    <!-- Konten Website Anda akan ditambahkan di sini -->
    <!-- Tambahkan referensi ke Bootstrap JavaScript di bagian bawah body -->
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>
  </body>
</html>
```

**2. Membangun Tampilan dengan Bootstrap:**

Gunakan kelas-kelas Bootstrap seperti container, row, dan col untuk membangun tata letak halaman.
Tambahkan elemen HTML, teks, dan gambar sesuai kebutuhan.
Anda dapat menggunakan komponen Bootstrap seperti navigasi, jumbotron, dan card untuk mempercepat pembuatan tampilan.
Berikut adalah struktur dasar : 
```html
<body>
    <div class="container">

        <header>
            <h1>Layout Sederhana</h1>
        </header>

        <nav>
            <a href="#" class="active">Home</a>
            <a href="#article">Artikel</a>
            <a href="#about">About</a>
            <a href="#contact">Kontak</a>
        </nav>

        <section id="hero">
            <h1>Hello World!</h1>
            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem
                elit, iaculis innisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla,
                vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc
                pretium ac.</p>
            <a href="home.html" class="btn btn-large">Learn more &raquo;</a>
        </section>

        <section id="wrapper">
            <section id="main">
                <div class="row">
                    <div class="box">
                        <img src="https://dummyimage.com/120/db7d25/fff.png" alt="" class="image-circle">
                        <h3>Heading</h3>
                        <p>Donec sed odio dui. Etiam porta sem malesuada magna mollis
                            euismod.</p>
                        <a href="#" class="btn btn-default">View detail</a>
                    </div>
                    <div class="box">
                        <img src="https://dummyimage.com/120/3e73e6/fff.png" alt="" class="image-circle">
                        <h3>Heading</h3>
                        <p>Donec sed odio dui. Etiam porta sem malesuada magna mollis
                            euismod.</p>
                        <a href="#" class="btn btn-default">View detail</a>
                    </div>
                    <div class="box">
                        <img src="https://dummyimage.com/120/71e6d4/fff.png" alt="" class="image-circle">
                        <h3>Heading</h3>
                        <p>Donec sed odio dui. Etiam porta sem malesuada magna mollis
                            euismod.</p>
                        <a href="#" class="btn btn-default">View detail</a>
                    </div>
                </div>

                <hr class="divider" />
                <article class="entry" id="article">
                    <h2>First featurette heading.</h2>
                    <img src="https://dummyimage.com/150/7b8a70/fff.png" alt="">
                    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem
                        elit, iaculis in nisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla,
                        vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc
                        pretium ac.</p>
                </article>

                <hr class="divider" />
                <article class="entry">
                    <h2>First featurette heading.</h2>
                    <img src="https://dummyimage.com/150/7b8a70/fff.png" alt="" class="right-img">
                    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem
                        elit, iaculis in nisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla,
                        vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc
                        pretium ac.</p>
                </article>
            </section>

            <aside id="sidebar">
                <div class="widget-box">
                    <h3 class="title">Widget Header</h3>
                    <ul>
                        <li><a href="#">Widget Link</a></li>
                        <li><a href="#">Widget Link</a></li>
                        <li><a href="#">Widget Link</a></li>
                        <li><a href="#">Widget Link</a></li>
                        <li><a href="#">Widget Link</a></li>
                    </ul>
                </div>

                <div class="widget-box">
                    <h3 class="title">Widget Text</h3>
                    <p>Vestibulum lorem elit, iaculis in nisl volutpat, malesuada tincidunt
                        arcu. Proin in leo fringilla, vestibulum mi porta, faucibus felis. Integer
                        pharetra est nunc, nec pretium nunc pretium ac.</p>
                </div>
            </aside>
        </section>

        <footer>
            <p>&copy; 2021 - Universitas Pelita Bangsa</p>
        </footer>
    </div>
```

**Ouput sebelum diberi style bootstrap**

![1](https://github.com/tiaraputriiiiii/Lab6Web/assets/115775237/1a8d4c64-ba92-4201-b354-35d96a927940)

![2](https://github.com/tiaraputriiiiii/Lab6Web/assets/115775237/e1fee979-6a9b-4940-8859-8ac0e7b8e543)

**3. Custom CSS (Opsional):**

Jika Anda ingin menyesuaikan tampilan lebih lanjut, Anda dapat menambahkan CSS kustom Anda sendiri. Buat file CSS terpisah atau tambahkan gaya langsung ke dalam tag `style` di bagian `head HTML`. Ini adalah tambahan css styles pada website ini:
```html
    <!-- Css styles -->
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: "Open Sans", sans-serif;
            font-size: 100%;
        }

        #container {
            height: 1300px;
        }

        nav a.active,
        nav a:hover {
            background-color: #68a4e8;
        }

        .widget-box li:hover a {
            background-color: #eee;
        }

        .row:after,
        .row:before,
        .entry:after,
        .entry:before {
            content: "";
            display: table;
        }

        .row:after,
        .entry:after {
            clear: both;
        }
    </style>
```

**4. Ini adalah keseluruhan program**
```html
<body class="text-body-secondary lh-1">
    <div class="container w-75 shadow-lg p-3 mb-0 bg-body-tertiary rounded" id="container">

        <header class="p-3">
            <h1 class="mt-2 mb-2 me-1 ms-1 text-body-tertiary fw-bold">Layout Sederhana</h1>
        </header>

        <nav class="bg-primary d-block">
            <a href="#"
                class="active pt-3 pb-3 ps-3 pe-3 text-white fs-6 fw-bold text-decoration-none d-inline-block">Home</a>
            <a href="#article"
                class="pt-3 pb-3 ps-3 pe-3 text-white fs-6 fw-bold text-decoration-none d-inline-block">Artikel</a>
            <a href="#about"
                class="pt-3 pb-3 ps-3 pe-3 text-white fs-6 fw-bold text-decoration-none d-inline-block">About</a>
            <a href="#contact"
                class="pt-3 pb-3 ps-3 pe-3 text-white fs-6 fw-bold text-decoration-none d-inline-block">Kontak</a>
        </nav>

        <section id="hero" class="bg-dark-subtle pb-5 pt-5 pe-3 ps-3 mb-2">
            <h1 class="mb-4 fs-1 fw-bold">Hello World!</h1>
            <p class="mb-3 fs-5 lh-base">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem
                elit, iaculis innisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla,
                vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc
                pretium ac.</p>
            <a href="home.html" class="btn btn-large">Learn more &raquo;</a>
        </section>

        <section id="wrapper" class="m-0 position-relative">
            <section id="main" class="float-start w-75 p-2 ">
                <div class="row">
                    <div class="box pt-0 pb-0 pe-2 d-block float-none w-25">
                        <img src="https://dummyimage.com/120/db7d25/fff.png" alt="" class="rounded-circle ms-4">
                        <h3 class="mt-2 mb-2 me-0 ms-0 text-center fs-4 fw-bold">Heading</h3>
                        <p class="lh-base fs-6 mb-2 text-center">Donec sed odio dui. Etiam porta sem malesuada magna
                            mollis
                            euismod.</p>
                        <a href="#" class="ms-5 fw-medium fs-6 btn bg-dark-subtle p-2 rounded">View detail</a>
                    </div>
                    <div class="box pt-0 pb-0 pe-2 ps-2 d-block float-start w-25 align-items-center">
                        <img src="https://dummyimage.com/120/3e73e6/fff.png" alt="" class="rounded-circle ms-4">
                        <h3 class="mt-2 mb-2 me-0 ms-0 text-center fs-4 fw-bold">Heading</h3>
                        <p class="lh-base fs-6 mb-2 text-center">Donec sed odio dui. Etiam porta sem malesuada magna
                            mollis
                            euismod.</p>
                        <a href="#" class="ms-5 fw-medium fs-6 btn bg-dark-subtle p-2 rounded">View detail</a>
                    </div>
                    <div class="box pt-0 pb-0 pe-2 ps-2 d-block float-start w-25 align-items-center">
                        <img src="https://dummyimage.com/120/71e6d4/fff.png" alt="" class="rounded-circle ms-4">
                        <h3 class="mt-2 mb-2 me-0 ms-0 text-center fs-4 fw-bold">Heading</h3>
                        <p class="lh-base fs-6 mb-2 text-center">Donec sed odio dui. Etiam porta sem malesuada magna
                            mollis
                            euismod.</p>
                        <a href="#" class="ms-5 fw-medium fs-6 btn bg-dark-subtle p-2 rounded">View detail</a>
                    </div>
                </div>

                <hr class="divider border-0 border-top border-light-subtle mb-3 mt-3 me-0 ms-0" />
                <article class="entry mb-2 mt-2 me-0 ms-0" id="article">
                    <h2 class="mb-2 fs-3 fw-bold">First featurette heading.</h2>
                    <img src="https://dummyimage.com/150/7b8a70/fff.png" alt="" class="float-start rounded ms-2">
                    <p class="lh-base">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem
                        elit, iaculis in nisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla,
                        vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc
                        pretium ac.</p>
                </article>

                <hr class="divider  border-0 border-top border-light-subtle mb-3 mt-3 me-0 ms-0" />
                <article class="entry mb-2 mt-2 me-0 ms-0">
                    <h2 class="mb-3 fs-3 fw-bold">First featurette heading.</h2>
                    <img src="https://dummyimage.com/150/7b8a70/fff.png" alt="" class="float-end rounded ms-2">
                    <p class="lh-base">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem
                        elit, iaculis in nisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla,
                        vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc
                        pretium ac.</p>
                </article>
            </section>

            <aside id="sidebar" class="float-start w-25 p-3">
                <div class="widget-box border border-secondary mb-3">
                    <h3 class="title pt-2 pb-2 ps-2 pe-2 bg-primary text-white fs-4">Widget Header</h3>
                    <ul class="list-unstyled">
                        <li class="border-bottom border-secondary"><a
                                class="pt-2 pb-2 pe-3 ps-3 text-success-emphasis d-block text-decoration-none"
                                href="#">Widget Link</a></li>
                        <li class="border-bottom border-secondary"><a
                                class="pt-2 pb-2 pe-3 ps-3 text-success-emphasis d-block text-decoration-none"
                                href="#">Widget Link</a></li>
                        <li class="border-bottom border-secondary"><a
                                class="pt-2 pb-2 pe-3 ps-3 text-success-emphasis d-block text-decoration-none"
                                href="#">Widget Link</a></li>
                        <li class="border-bottom border-secondary"><a
                                class="pt-2 pb-2 pe-3 ps-3 text-success-emphasis d-block text-decoration-none"
                                href="#">Widget Link</a></li>
                        <li class="border-bottom border-secondary"><a
                                class="pt-2 pb-2 pe-3 ps-3 text-success-emphasis d-block text-decoration-none"
                                href="#">Widget Link</a></li>
                    </ul>
                </div>

                <div class="widget-box border border-secondary mb-3">
                    <h3 class="title pt-2 pb-2 ps-2 pe-2 bg-primary text-white fs-4">Widget Text</h3>
                    <p class="p-2 lh-base">Vestibulum lorem elit, iaculis in nisl volutpat, malesuada tincidunt
                        arcu. Proin in leo fringilla, vestibulum mi porta, faucibus felis. Integer
                        pharetra est nunc, nec pretium nunc pretium ac.</p>
                </div>
            </aside>
        </section>

    </div>
    <footer class="w-75 text-white bg-dark mx-auto p-2 text-center">
        <p>&copy; 2021 - Universitas Pelita Bangsa</p>
    </footer>


    <!-- Feather icon -->
    <script>
        feather.replace();
    </script>

    <!-- Bootstrap -->
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js"
        integrity="sha384-C6RzsynM9kWDrMNeT87bh95OGNyZPhcTNXj1NW7RuBCsyN/o0jlpcV8Qyq46cDfL"
        crossorigin="anonymous"></script>
</body>
```

**Output sesudah menggunakan style bootstrap**

![4](https://github.com/tiaraputriiiiii/Lab6Web/assets/115775237/b69a9cdc-8920-4687-97a1-1fc0fa04c207)

![3](https://github.com/tiaraputriiiiii/Lab6Web/assets/115775237/e4a70029-1b0f-435c-af67-3f0f13daf91f)

## Selesai, Terima kasih 🙏

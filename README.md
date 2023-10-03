# Lab2Web
Nama : Anggita Risqi Nur Clarita

NIM : 312210450

Kelas : TI.22.A.4

## DAFTAR ISI <br>
| No | Description | Link |
|-----|------|-----|
|1|Modul Praktikum 2|[Click Here](https://drive.google.com/file/d/1r0GF11LB_VK3VlfDubBQJqBekDm2m0Rf/view)|
|2|Praktikum|[Click Here](#praktikum)|
|3|Pertanyaan dan Tugas|[Click Here](#pertanyaan-dan-tugas)|

## Praktikum
> ### Instruksi Praktikum
> 1. Persiapkan text editor misalnya **VSCode**.
>
> 2. Buat file baru dengan nama `lab2_css_dasar.html`
>
> 3. Buat struktur dasar dari dokumen HTML.
>
> 4. Ikuti langkah-langkah praktikum yang akan dijelaskan berikutnya.

## Langkah-langkah Praktikum
### Persiapan membuka VSCode.
![image](https://github.com/AnggitaRisqiNC/Lab2Web/blob/main/screenshot/1.png)


### Kemudian buat file baru dengan nama `lab2_css_dasar.html`.
![image](https://github.com/AnggitaRisqiNC/Lab2Web/blob/main/screenshot/2.png)


1. ### Membuat Dokumen HTML
    ```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>CSS Dasar</title>
    </head>
    <body>
        <header>
            <h1>CSS Internal dan <i>Inline CSS</i></h1>
        </header>
        <nav>
            <a href="lab2_css_dasar.html">CSS Dasar</a>
            <a href="lab2_css_eksternal.html">CSS Eksternal</a>
            <a href="lab1_tag_dasar.html">HTML Dasar</a>
        </nav>
        <!-- CSS ID Selector -->
        <div id="intro">
            <h1>Hello World</h1>
            <p>Kami sedang belajar HTML dan CSS dasar, pada mata kuliah <b>Pemrograman Web</b> di <i>Universitas Pelita Bangsa</i>. Pelajaran pertama yang kami dapat adalah membuat tampilan web sederhana dalam rangka mengenal tag-tag dasar HTML dan CSS.</p>
            <!-- CSS Class Selector -->
            <a class="button btn-primary" href="#intro">Informasi selengkapnya.</a>
        </div>
    </body>
    </html>
    ```

    **Output**
    
    ![image](https://github.com/AnggitaRisqiNC/Lab2Web/blob/main/screenshot/3.png)
    **Keterangan** : Disini saya menggunakan Microsoft Edge untuk melihat hasilnya.


2. ### Mendeklarasikan CSS Internal
    ```html
    <head>
        <title>CSS Dasar</title>
        <style>
            body {
                font-family:'Open Sans', sans-serif;
            }
            header {
                min-height: 80px;
                border-bottom:1px solid #77CCEF;
            }
            h1 {
                font-size: 24px;
                color: #0F189F;
                text-align: center;
                padding: 20px 10px;
            }
            h1 i {
                color:#6d6a6b;
            }
        </style>
    </head>
    ```

    **Output**
    
    ![image](https://github.com/AnggitaRisqiNC/Lab2Web/blob/main/screenshot/4.png)
    **Keterangan** : Script HTML tersebut digunakan untuk mendeklarasikan CSS Internal.


3. ### Menambahkan Inline CSS
    ```html
    <p style="text-align: center; color: #ccd8e4;">
    ```

    **Output**

    ![image](https://github.com/AnggitaRisqiNC/Lab2Web/blob/main/screenshot/5.png)
    **Keterangan** : Script HTML tersebut digunakan untuk mendeklarasikan inline CSS pada tag `<p>`.


4. ### Membuat CSS Eksternal
    ```css
    nav {
        background: #20A759;
        color:#fff;
        padding: 10px;
    }
    nav a {
        color: #fff;
        text-decoration: none;
        padding:10px 20px;
    }
    nav .active,
    nav a:hover {
        background: #0B6B3A;
    }
    ```

    Kemudian tambahkan tag `<link>` untuk merujuk file css yang sudah dibuat pada bagian `<head>`.

    ```html
    <head>
        <!-- menyisipkan css eksternal -->
        <link rel="stylesheet" href="style_eksternal.css" type="text/css">
    </head>
    ```

    **Output**

    ![image](https://github.com/AnggitaRisqiNC/Lab2Web/blob/main/screenshot/6.png)
    **Keterangan** : Disini diperintahkan untuk membuat file baru dengan nama `style_eksternal.css`, kemudian mendeklarasikan CSS seperti script yang telah tersedia.


5. ### Menambahkan CSS Selector
    ```css
    /* ID Selector */
    #intro {
        background: #418fb1;
        border: 1px solid #099249;
        min-height: 100px;
        padding: 10px;
    }
    #intro h1 {
        text-align: left;
        border: 0;
        color: #fff;
    }
    /* Class Selector */
    .button {
        padding: 15px 20px;
        background: #bebcbd;
        color: #fff;
        display: inline-block;
        margin: 10px;
        text-decoration: none;
    }
    .btn-primary {
        background: #E42A42;
    }
    ```

    **Output**

    ![image](https://github.com/AnggitaRisqiNC/Lab2Web/blob/main/screenshot/7.png)
    **Keterangan** : Script diatas digunakan untuk menambahkan CSS Selector menggunakan ID dan Class Selector pada file `style_eksternal.css`.


## Pertanyaan dan Tugas

1. **Lakukan eksperimen dengan mengubah dan menambah properti dan nilai pada kode CSS dengan mengacu pada CSS Cheat Sheet yang diberikan pada file terpisah dari modul ini!**
    
    ![image](https://github.com/AnggitaRisqiNC/Lab2Web/blob/main/screenshot/8.png)

2. **Apa perbedaan pendeklarasian CSS elemen `h1 {...}` dengan `#intro h1 {...}`? berikan penjelasannya!**

    * Pendeklarasian `#intro h1 {...}` hanya akan mengubah tampilan elemen `h1` yang memiliki ID `intro`.
    ![image](https://github.com/AnggitaRisqiNC/Lab2Web/blob/main/screenshot/9.png)


    * Sedangkan pendeklarasian CSS elemen `h1 {...}` akan mengubah tampilan seluruh elemen yang memiliki tag `h1`.
    ![image](https://github.com/AnggitaRisqiNC/Lab2Web/blob/main/screenshot/10.png)

3. **Apabila ada deklarasi CSS secara internal, lalu ditambahkan CSS eksternal dan inline CSS pada elemen yang sama. Deklarasi manakah yang akan ditampilkan pada browser? Berikan penjelasan dan contohnya!**

    Jika terdapat deklarasi CSS secara Internal, eksternal, dan inline pada elemen yang sama, maka deklarasi CSS yang akan ditampilkan pada browser adalah **Inline CSS**. Hal ini disebabkan karena inline CSS memiliki specificity yang lebih tinggi dibandingkan dengan CSS internal dan eksternal.

    * Contoh Deklarasi **CSS Eksternal** (di script HTML)
    ![image](https://github.com/AnggitaRisqiNC/Lab2Web/blob/main/screenshot/11.png)

    * Contoh Deklarasi **CSS Eksternal** (di script CSS)
    ![image](https://github.com/AnggitaRisqiNC/Lab2Web/blob/main/screenshot/12.png)

    * Contoh Deklarasi **Inline CSS** (di script HTML)
    ![image](https://github.com/AnggitaRisqiNC/Lab2Web/blob/main/screenshot/13.png)

    * **Hasil Output yang ditampilkan**
    ![image](https://github.com/AnggitaRisqiNC/Lab2Web/blob/main/screenshot/14.png)

4. **Pada sebuah elemen HTML terdapat ID dan Class, apabila masing-masing selector tersebut terdapat deklarasi CSS, maka deklarasi manakah yang akan ditampilkan pada browser? Berikan penjelasan dan contohnya!** 
    ```html
    <p id="paragraf-1" class="text-paragraf">
    ```

    Jika terdapat deklarasi CSS pada ID dan Class pada elemen HTML yang sama, maka deklarasi CSS yang akan ditampilkan pada browser adalah **ID CSS**. Hal ini disebabkan karena ID CSS memiliki specificity yang lebih tinggi dibandingkan dengan Class CSS.

    ![image](https://github.com/AnggitaRisqiNC/Lab2Web/blob/main/screenshot/14.png)

## Finish
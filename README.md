## link website = https://future-fashion.adaptable.app/

## TUGAS 5

1. Manfaat element selector yaitu memungkinkan kita untuk mengubah properti semua elemen yang punya tag HTML yang sama. Dengan memanfaatkan element selector maka waktu mendesain jadi lebih praktis selain itu kode jadi lebih mudah terbaca.

element selector cocok digunakan jika ingin mengkustom kesamaan desain di setiap tag HTML yang sama.

2. HTML5 Tag yang kuketahui: (! digunakan untuk )
    - <!br> : break di baris
    - <!div> : untuk buaat section 
    - <!audio> : untuk file audio
    - <!video> : untuk file video
    - <!nav> : elemen untuk navigasi 
    - <!p> : untuk paragraf
    - <!span> : untuk mengelilingi bagian di teks (berguna ketika ingin mendesain bagian tertentu di teks)
    - <!th> : untuk tabel header
    - <!td> : untuk tabel sel
    - <!ul> : untuk membuat daftar tak berurut
    - <!body> : menentukan elemen body

3. Margin => mengosongkan area di sekitar tepian tag HTML (membuat jarak suatu elemen dengan elemen luar)

Padding => mengosongkan area disekitar konten HTML (membuat jarak suatu elemen dengan elemen didalamnya)

4. CSS tailwind => atomic CSS, memudahkan pemakaian CSS dengan kelas-kelas utilitas yang sederhana dan praktis.

Bootstrap => menyediakan komponen UI yang bisa dipakai sesuai kebutuhan.

CSS tailwind lebih cocok dipakai dibanding bootstrap untuk proyek yang memerlukan design yang kompleks karena penggunaannya sangat fleksibel. Sedangkan bootstrap lebih cocok digunakan dibanding tailwind CSS ketika ingin membuat proyek yang instan.

5. Implementasi checklist 
    sebelum mengkustomisasi web, saya mengkonfigurasi tailwind css terlebih dahulu dengan membuat folder baru bernama tailwind dan menginstall tailwindcss serta menginitnya.

    setelah itu, saya mengkonfigurasi path ke templates di tailwind.config.js

    kemudian, saya menambahkan @tailwind di atas file global.css di folder tailwind. lalu saya membuat folder dist untuk tempat file statis dan dist/css/tailwind.css untuk menampung hasil kompilasi css

    setelah itu, saya menjalankan build process tailwind 

    * Kustomisasi halaman login
        - saya membuat semua elemen ke tengah dengan flex flex-col justify-center items-center
        - saya membuat backgroundnya dengan warna di tailwind bg-violet-300

    * Kustomisasi halaman register
        - kurang lebih sama dengan di halaman login, hanya paling marginnya yang ada berbeda. untuk mengatur margin saya memanfaatkan utilitas tailwind bernama m-suatunilai

    * Kustomisasi halaman tambah inventori
        - sama dengan halaman login

    * Kustomisasi halaman daftar inventori
        - saya membuat background halaman main menjadi warna biru dan menambahkan gambar dengan memanfaatkan direktori statis 
        - setiap objek di Items di iterasi ke dalam bentuk card. card disini memanfaatkan tag elemen div. saya menambahkan warna background dengan css biasa karena sudah terlanjur menggunakan css biasa sebelumnya. di dalam div ada tag elemen2 lain seperti p, a, dan sebagainya
        - di tiap card saya menambahkan button untuk menambahkan dan mengurangi amount, saya juga menambahkan button untuk edit dan delete. fungsi untuk ke empat util tersebut saya buat di views.py dan menambahkan url nya di urls.py yang ada di main
        - button edit dan delete saya masukan dalam 1 div kemudian diatur stylenya menjadi display: inline; agar mereka berada dalam baris yang sama
        - untuk designnya sendiri saya mengganti warna tiap button dengan memanfaatkan css. kemudian button + dan - saya buat agak bulat dengan memanfaatkan border-radius di stylenya 
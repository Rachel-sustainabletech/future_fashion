link website = https://future-fashion.adaptable.app/

1. berikut implementasi yang saya lakukan: 
    - membuat proyek baru django baru dengan membuat direktori, mengaktifkan virtual environment, dan menjalankan perintah django-admin startproject future_fashion .
    - membuat aplikasi main dengan menjalankan perintah python manage.py startapp main dan menambahkan 'main' ke INSTALLED_APPS yang ada di settings.py direktori proyek
    - membuat routing dengan menambahkan path('main/', include('main.urls')) di urls.py proyek agar setiap urls yang ada di main bisa diakses
    - membuat model pada aplikasi main dengan nama Item yang punya atribut berupa name, amount, description, dan price
    - membuat fungsi di views.py bernama show_main yang dimana show_main menampilkan main.html yang ada di templates. saya memanfaatkan context untuk menampilkan nama dan kelas
    - membuat file urls.py di aplikasi main yang berisi app_name = 'main' serta urls pattern diri sendiri dengan menyertakan suatu fungsi di view
    - melakukan deployment dengan mendeploy repositori github saya yang bernama future_fashion  
    - membuat file bernama README.md yang berisi tautan app adaptable beserta jawaban uraian
    - tambahan selain yang di tutorial: saya membuat suatu direktori bernama static untuk menampung data-data dan gambar yang ingin digunakan di web. saya juga mendefinisikan konfigurasi url staticnya di settings.py. ada dibagian paling bawah dengan tagar static

2. berikut bagan request client ke web aplikasi Django
<br>
[Bagan](Client.png)
<br>
ketika user melakukan browser (mengirim request), internet akan mengirim http/https request ke web server. aplikasi django yang ada di web server pun mengelola request dengan mengarahkan ke view yang dikehendaki. view yang menjadi jembatan antara model dan template akan mendapat dan mengirimkan data ke model serta mendapat tampilan dari template. kemudian view akan mengirimkan http response berupa html yang nantinya web server akan mengembalikan response tersebut ke user untuk ditampilkan di browser. 

3. virtual environment memungkinkan pengembangan dari suatu proyek yang kita kerjakan inklusif. maksudnya apa yang kita kerjakan di suatu proyek django yang menggunakan virtual environment tidak akan mempengaruhi proyek lainnya seperti dependency yang diinstall dan lain sebagainya. 

Kita tetap bisa membuat aplikasi web berbasis django tanpa menggunakan venv. tetapi risikonya ada kemungkinan crash karena kebutuhan tiap2 proyek ada bisa jadi berbeda

4. MVC merupakan singkatan dari Model View Controller. Model berperan untuk menyimpan data, view berperan sebagai tempat untuk menyimpan presentasi tampilan website, dan controller mengatur alur tampilan yang ada di view (sebagai jembatan antara model dan view)

MVT merupakan singkatan Model View Template. Model berperan untuk menyimpan data, template berperan sebagai tempat untuk menyimpan tampilan, dan view mengatur alur tampilan yang ada di template (jembatan antara template dan model)

perbedaan MVC dan MVT hanya terletak di istilah tetapi arsitekturnya sama. perbedaannya Controller di MVC bertindak seperti View di MVT, sedangkan View di MVC berperan seperti Template di MVT. 

istilah MVC merupakan istilah umum yang digunakan di dunia pengembangan perangkat lunak, sedangkan MVT merupakan istilah lain dari MVC yang digunakan di komunitas django

MVVM merupakan singkatan dari Model View ViewModel. Model berperan untuk menyimpan dan mengelola data, view berperan untuk menampung tampilan, dan ViewModel berperan jembatan antara Model dan View serta tempat logika tampilan. 

ViewModel tidak hanya berperan sebagai jembatan antara Model dan View tetapi juga tempat untuk mengelola logika tampilan sehingga Model bisa fokus pada data saja, pemrosesan datanya diserahkan pada ViewModel. Intinya pemisahan View dan Model di ViewModel arsitektur MVVM lebih ketat dibanding di arsitektur MVC. 
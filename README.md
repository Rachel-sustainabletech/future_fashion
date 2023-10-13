## link website = https://future-fashion.adaptable.app/

## TUGAS 6

1. Asynchronous programming => Operasi dilakukan secara berurutan

Synchronous programming => Beberapa operasi dilakukan secara bersamaan

2. Event driven programming => 

3. Penerapan asynchronous programming pada AJAX => 

4. Penerapan AJAX dengan Fetch API => 

Penerapan AJAX dengan library jQuery => AJAX memanfaatkan asynchronous programming untuk 

5. Cara mengimplementasikan checklist di atas: 
    - pertama-tama saya membuat fungsi untuk mengembalikan data JSON
    - kemudian saya membuat fungsi add_item_ajax di views.py
    - selanjutnya saya mengimpor csrf_exempt di berkas views.py dan menambahkannya di atas fungsi add_item_ajax
    - saya menambahkan tag div yang memiliki id product table. kemudian saya membuat fungsi getProducts() dan refreshProducts() di dalam tag script yang ada di main.html 
    - setelah itu saya membuat modal bootstrap sebagai form untuk menambahkan produk dan button yang berfungsi untuk menampilkan modal
    - lalu saya membuat fungsi dengan nama addProduct() yang akan akan menyimpan form modal yang ada
# COOKIE-PHP

# Cookie

Cookie memiliki kegunaan yang hampir sama dengan session namun cookie disimpan di dalam komputer user dan dapat di setting waktu berlakunya cookie tersebut, jadi walaupun kamu menutup browser, cookie tersebut tidak akan hancur sampai waktu yang kamu berikan berakhir kecuali kamu menghancurkannya dengan script. Cookie biasanya dipakai untuk membuat halaman yang membutuhkan otentikasi (login).

# Berikut aturan pembuatan session :

    Nama cookie harus diawali alphabet.
    Memasukan nilai cookie berupa string(text) harus diawali dan diakhiri dengan tanda " atau  '.
    Memasukan nilai cookie berupa angka tidak harus diawali dan diakhiri dengan tanda " atau ', namun kamu tetap dapat menggunakan tanda tersebut.
    Memasukan nilai cookie dari variable lainnya tidak harus diawali dan diakhiri dengan tanda ", namun kamu tetap dapat menggunakan tanda tersebut.


# Membuat cookie.

/* Membuat cookie tanpa set waktu */ 

# setcookie("nama cookie", "nilai cookie");

/* Atau dengan menambahkan waktu seperti dibawah ini */ 

# setcookie("nama cookie", "nilai cookie", "waktu masa berlaku cookie");



# Mengambil Nilai cookie.

# $_COOKIE['nama cookie'];

File cookie.php simpan di dalam folder C:\xampp\htdocs\belajar-php

<?php
 
    //Set cookie tanpa waktu

    setcookie("negara", "Indonesia");
 
    //mengerluarkan nilai cookie

    echo $_COOKIE['negara'];
     
?>

Untuk mencoba ketikan url dibawah ini di browser kamu.

http://localhost/belajar-php/cookie.php

Ketika kamu jalankan file cookie.php cookie baru dibuat dan ketika kamu echo $_COOKIE['negara']; akan terjadi error karena cookie tersebut belum dapat dibaca. untuk dapat melihatnya silahkan kamu refresh lagi file cookie.php di browser kamu (tekan f5 atau tekan enter pada url) atau kamu dapat melihatnya pada file cookieKedua.php yang akan kita buat pada step selanjutnya.

Hasilnya.

# Basic of PHP

## Table of Contents

  1. [Introduction](#introduction)
  2. [Environtment](#Environment)
  3. [Content](#content)
     * [1](#1)
     * [2](#2)
     * [3](#3)
     * [4](#4)
     * [Control Structures](#control-structures)
  4. [Write clean code with OOP](#cleancode)
     * [Classes and object](#classes-and-object)
     * [Use the same vocabulary for the same type of variable](#use-the-same-vocabulary-for-the-same-type-of-variable)
     
## Introduction

Mungkin banyak orang yang bertanya menjadi seorang developer hebat harus dimulai dari mana?
1. Niat
2. Kemauan
3. Kerja Keras

3 hal diatas mutlak wajib bagi saya pribadi ketika memulai memutuskan menjadi software engineer khususnya di Backend, So let's try to write some code dude !!

## Environment

```php
function createMicrobrewery(string $breweryName = 'Hipster Brew Co.'): void
{
    // ...
}
```
**[⬆ back to top](#table-of-contents)**

## 2



**[⬆ back to top](#table-of-contents)**

## Content

### 1

### 2

### 3

### 4

### Control Structures

Sebuah program akan mengeksekusi setiap baris kode yang ada di program kita. Namun, Jika ada beberapa array (misal) yang berisi data tapi data dalam array tersebut tidak seperti yang diharapkan. Disinilah kita perlu mengontrol struktur dari setiap baris kode kita. Mengkontrol struktur ibarat lampu lalu lintas, baris kode kita akan dikontrol dengan flow yang kita inginkan. Ada 2 kategori dalam Struktur Control yaitu Perulangan dan Pengkondisian(Conditionals). Jika kita pengen mengetahui fungsionalitas dari baris kode kita hanya untuk beberapa tertentu pakai pengkondisian namun jika perlu dieksekusi berkali2 maka kita perlu menggunakan Perulangan.

- >Pengkondisian<

Pada umumnya pengkondisian mengeksekusi tipe boolean, yang mana jika sesuatu bernilai true maka akan mengeksekusi beberapa baris kode yang kita inginkan.

Misal : 

```php
if(11 > 10){
  echo "Kondisi yang kita inginkan"; //true
}

if(3 > 4 ){
  echo "Kondisi yang kita inginkan tidak jalan";//false
}

```
- Switch Case

Struktur kontrol lainnya yaitu switch case , dengan switch case kita bisa mengontrol keadaan yang kita inginkan layaknya soal pilihan ganda pada ujian. Kondisi akan berjalan pada keadaan yang sesuai dengan case yang sesuai dengan yang kita dapatkan.
```php
$judulFilm = 'Titanic';

switch ($judulFilm) {
  case 'Harry Potter':
        echo "Tidak sesuai keadaan";
        break;
  case 'Titanic':
        echo "Sesuai keadaan   ";
        break;
  default:
        echo "Kondisi lain";
        break;
}

```
- >Perulangan<

Dalam suatu kasus kita perlu cek kondisi dari baris kode kita dalam beberapa kali waktu dalam satu kali eksekusi. Disinilah perulangan diperlukan , ada beberapa metode dalam perulangan yaitu While, Do...While, For, Foreach.

  - While

  Perulangan termudah menggunakan perulangan While. Perulangan While hanya mengeksekusi beberapa code sampai code tersebut selesai/false di eksekusi.
  ```php
  while ($i < 5) {
    echo $i . "<br>";
    $i++; 
  }
  ```
  - Do While
  
  Perulangan ini hampir mirip dengan while , letak perbedaannya adalah dari evaluasinya. While mengevaluasi beberapa code kemudian melakukan perulangan sampai kondisi false sedangkan do while melakukan perulangan kemudian dievaluasi setidaknya ketika ada kondisi yang tidak sesuai dengan kondisi yang diinginkan , baris code pernah di eksekusi sekali walaupun false. 
  
  ```php
  do {
    echo $i . " yo";
    $i++;
  } while ($i < 0);

  ```
  - For
  
  Diantara perulangan lainnya , for merupakan perulangan yang paling kompleks. For memiliki 4 perulangan, pertama merupakan inisasi , kemudian dilanjutkan evaluasi kondisi exit , jika kondisi tadi benar maka akan lanjut dengan expresi iterasi dan diakhiri dengan evaluasi kondisi exit lagi sampai false.
  
  ```php
  $warga = array("Faisal","Mahendra","chelly");
  echo '<br>';

  for ($i = 0; $i < count($warga); $i++) {
    echo $warga[$i] . "lo ";
  }

  ``` 
  - Foreach
  
  Perulangan ini akan mengeksekusi array dan mengiterasinya sampai array posisi terakhir walapun tidak tau key/posisi dari array tersebut.
  ```php
  foreach ($warga as $key => $warganet) {
    echo $key . "->" . $warganet . "<br>" ;
  }  
  ```

**[⬆ back to top](#table-of-contents)**

## CleanCode

### Classes and object

**Bad:**

```php
$ymdstr = $moment->format('y-m-d');
```

**Good:**

```php
$currentDate = $moment->format('y-m-d');
```

**[⬆ back to top](#table-of-contents)**

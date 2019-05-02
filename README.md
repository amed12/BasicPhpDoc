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

- Pengkondisian

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

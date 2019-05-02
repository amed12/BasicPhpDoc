# Basic of PHP

## Table of Contents

  1. [Introduction](#introduction)
  2. [Environtment](#Environment)
  3. [Cooming soon 3](#3)
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

## 3


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

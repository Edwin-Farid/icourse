---
title: "Kotlin Fundamental"
date: 2023-08-24T10:17:22+08:00
draft: false

showtableofcontents: true
tags: ["Mobile Developer", "Kotlin", "Android", "Dasar Kotlin"]

series: ["Kotlin Mobile Developer"]
series_order: 1
---

# Data Types & Variable

- Char
- String
- Array
- Numbers
- Booleans

```kotlin {linenos=table,linenostart=1}
var identifier: Type = initialization
```

- var and val is a key : var can we put a new value but val cannot
- company is identifier or we call name of variable
- String is type or we call type data
- BlocDev is initialize or we call value

```kotlin {linenos=table,linenostart=1}
var company: String = "BlocDev"
company = "Berkah Tech Indonesia"
```

## Char or Character

```kotlin {linenos=table,linenostart=1}
var vocal = 'A'
println("Voval "+vocal++) // A
println("Voval "+vocal++) // B
println("Voval "+vocal++) // C
println("Voval "+vocal--) // D
println("Voval "+vocal--) // C
```

## String

```kotlin {linenos=table,linenostart=1}
var vocal = 'A'
val textString = "Edwin"
val firstChar = textString[0]
println(firstChar)

for (char in textString){
    print("$char ")
}
```

### Escaped String

- \t: menambah tab ke dalam teks.
- \n: membuat baris baru di dalam teks.
- \’: menambah karakter single quote kedalam teks.
- \”: menambah karakter double quote kedalam teks.
- \: menambah karakter backslash kedalam teks.

```kotlin {linenos=table,linenostart=1}
var dataString = "Kotlin is \"awesome!\""
dataString = "\u00A9 2023" // © 2023
println(dataString)
```

### Raw String

Sebelum Raw String

```kotlin {linenos=table,linenostart=1}

val line = "Line 1\n" +
        "Line 2\n" +
        "Line 3\n" +
        "Line 4\n"
println(line)
```

Setelah Raw String

```kotlin {linenos=table,linenostart=1}
val line = """
    Line 1
    Line 2
    Line 3
    Line 4
""".trimIndent()
println(line)
```

## Functions

```kotlin {linenos=table,linenostart=1}
fun tampilData(nama: String, usia: Int,alamat: String): String {
    return "Hello nama saya $nama berusia $usia beralamat $alamat"
}

fun tampilData(nama: String, usia: Int,alamat: String) = "Hello nama saya $nama berusia $usia beralamat $alamat"

println(tampilData("Edwin",21, "Bermis 2 Selong"))
```

```kotlin {linenos=table,linenostart=1}
fun tampilDataPrint(nama: String, usia: Int, alamat: String): Unit{
    println("Hello nama saya $nama berusia $usia beralamat $alamat")
}

tampilDataPrint(nama = "Edwin", usia = 21, alamat = "Berims 2 Selong cuy")
```

## If Expression

```kotlin {linenos=table,linenostart=1}
    val angkaSatu = 4
    val angkaDua = 9
    val hasil = if (angkaSatu > 5){
        "Angka lebih dari lima" }else {"Angka kurang dari 5"}

    println(hasil)
```

## Bool

```kotlin {linenos=table,linenostart=1}
    val jamBuka = 9
    val jamTutup = 15
    val waktu = 16
    val toko = waktu >= jamBuka && waktu <= jamTutup
    println("Toko sedang buka : $toko")
```

## Numbers

- Int 32 : Mengandung data dengan ukuran 32bit
- Long 64 : Mengandung data dengan ukuran 64bit
- Short 16 : Mengandung data dengan ukuran 16bit
- Byte 8: Mengandung data dengan ukuran 8bit
- Double 64: Mengandung data nilai pecahan dengan ukuran 64bit
- Float 32: Sama dengan double namun dengan ukuran lebih kecil yaitu 32bit

```kotlin {linenos=table,linenostart=1}
    val maxInt = Int.MAX_VALUE // Untuk melihat nilai tertinggi dari int
    val minInt = Int.MIN_VALUE // Untuk melihat nilai terendah dari int

    println(minInt)
```

Konversi ke masing-masing type data

- toByte(): Byte
- toShort(): Short
- toInt(): Int
- toLong(): Long
- toFloat(): Float
- toDouble(): Double
- toChar(): Char

```kotlin {linenos=table,linenostart=1}
    val byteNumber: Byte = 7
    val intNumber: Int = byteNumber.toInt()

    println(intNumber)
```

## Array

```kotlin {linenos=table,linenostart=1}
    val kumpulanArray = arrayOf(1,3,5,7)

    val campuranArray = arrayOf(1,3,5,7,"Kotlin",true)

    campuranArray[4] = "Edwin"

    print(campuranArray[4])
```

Konversi ke masing-masing array

- intArrayOf() : IntArray
- booleanArrayOf() : BooleanArray
- charArrayOf() : CharArray
- longArrayOf() : LongArray
- shortArrayOf() : ShortArray
- byteArrayOf() : ByteArray

## Nullable

NullPointerException(NPE) atau istilahnya The Billioner Dollar Mistake Sebuah
kondisi sebuah nilai mengandung null

Ada beberapa cara mengatasi nilai yang null

- Dengan menambahkan ? pada type data
- Memberikan nilai default ketika data bisa jadi null

```kotlin {linenos=table,linenostart=1}
    val text: String = null //Akan terjadi error, karena nilai mengandung null

    val text: String? = null //Tidak error, karena kita mendefinisikan nilai itu boleh null

    if (text != null){ // Kita juga bisa menggunakan perkondisian untuk mengatasi nilai null
        print(text)
    }
```

## Safe Call Operator & Elvis Operator

### Safe Call Operator

Akan memberikan nilai null. Menggunakan tanda ?.

```kotlin {linenos=table,linenostart=1}
    val text: String? = null

    print(text?.length)
```

### Elvis Operator

Akan memberikan default nilai jika mendapati nilai null. Menggunakan tanda ?:

```kotlin {linenos=table,linenostart=1}
    val text: String? = null

    print(text?.length ?: 7)
```

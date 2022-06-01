## Step Program Kotlin with Gradle

- Buka cmd di folder tujuan, jalankan :
```kotlin
gradle init
```
- Pilih Jenis Proyek
- Pilih bahasa
- Pilih build script
- Masukan Project Name
- Masukan Package Name
- Semua langkah diatas bisa disingkat dengan menuliskan perintah dibawah:
```kotlin
gradle init --type kotlin-application --dsl kotlin --project-name kotlin --package com.dicoding.kotlin
```
- Menjalankan Program
```kotlin
gradle run
```
## Function
```kotlin
fun main() {
    val user = setUser("Alfian", 19)
    println(user)
 
    printUser("Alfian")
}
 
fun setUser(name: String, age: Int) = "Your name is $name, and you $age years old"
 
fun printUser(name: String) {
    println("Your name is $name")
}
 
/*
output :
Your name is Alfian, and you 19 years old
Your name is Alfian
*/
```

## Konversi
- toByte(): Byte
- toShort(): Short
- toInt(): Int
- toLong(): Long
- toFloat(): Float
- toDouble(): Double
- toChar(): Char

example:
```kotlin
fun main() {
    val stringNumber = "23"
    val intNumber = 3
 
    print(intNumber + stringNumber.toInt())
    /*
     output: 26
     */
}
```

## Array
```kotlin
val mixArray = arrayOf(1, 3, 5, 7 , "Dicoding" , true)
```
- intArrayOf() : IntArray
- booleanArrayOf() : BooleanArray
- charArrayOf() : CharArray
- longArrayOf() : LongArray
- shortArrayOf() : ShortArray
- byteArrayOf() : ByteArray

Menggunakan Array()
```kotlin
val intArray = Array(4, { i -> i * i }) // [0, 1, 4, 9]
```

## Nullable
```kotlin
val text: String? = null // ready to go
```
Penanganan:
- Safe Calls -> Proses akan dilewat
```kotlin
val text: String? = null
text?.length
```
- Elvis Operator -> Nilai defaultnya ditentukan
```kotlin
val text: String? = null
val textLength = text?.length ?: 7
```

## String Template
```kotlin
fun main() {
    val name = "Kotlin"
    val old = 3
    print("My name is $name, im $old years old")
}
/*
   output : My name is Kotlin, im 3 years old
*/
```

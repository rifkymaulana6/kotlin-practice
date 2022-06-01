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

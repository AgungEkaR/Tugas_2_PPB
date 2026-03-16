## Biodata
Agung Eka Ramadhan<br>
502231244

## Mata Kuliah
Pemrograman Perangkat Bergerak (E)<br>
Tugas ke-2

---

## Penjelasan Kode

### 1. Fungsi main()

```
void main() {
  runApp(const MyApp());
}
```

Fungsi `main()` adalah bagian utama Flutter.  
Fungsi `runApp()` berfungsi untuk menjalankan aplikasi dengan widget utama yaitu **MyApp**.

---

### 2. MyApp

```
class MyApp extends StatelessWidget
```

`MyApp` merupakan widget utama dari aplikasi. Menggunakan **StatelessWidget** karena tidak memiliki data yang berubah.

Di dalam widget ini terdapat `MaterialApp` yang berfungsi sebagai kerangka dasar Flutter.

hal lain yang terdapat disini antara lain:

- judul aplikasi
- tema aplikasi
- halaman utama yang akan ditampilkan

---

### 3. MaterialApp

```
return MaterialApp(
```
Pada bagian ini digunakan untuk menentukan halaman utama aplikasi yaitu `RowColumnPage`, judulm dan juga tema.

---

### 4. RowColumnPage

```
class RowColumnPage extends StatelessWidget
```

Widget ini merupakan halaman utama aplikasi. Di dalamnya terdapat komponen UI seperti gambar, teks, ikon, dan counter. Karena tampilan pada halaman ini bersifat statis dan tidak memiliki data yang berubah, maka cukup menggunakan stateles.

---

### 5. Scaffold

```
return Scaffold(
```

Kerangka dasar Flutter. Berisi AppBar dan Body yang menampilkan isi utama aplikasi.

---

### 6. AppBar

```
appBar: AppBar(
```

Digunakan untuk menampilkan bagian header aplikasi yang berisi judul **My First App**.

---

### 7. Column

```
body: Column(
```

`Column` digunakan untuk menyusun widget secara vertikal (dari atas ke bawah).

Pada aplikasi ini Column berisi beberapa komponen yaitu:

- gambar
- teks
- ikon kategori
- counter

---

### 8. Container

```
Container(
```

`Container` digunakan untuk mengatur tampilan widget seperti:

- margin
- padding
- warna background
- ukuran widget

Container juga digunakan sebagai tempat meletakkan widget lain agar tampilannya lebih teratur.

---

### 9. AspectRatio

`AspectRatio` digunakan untuk menjaga perbandingan ukuran widget. Pada kode ini menggunakan rasio **1:1** sehingga gambar berbentuk persegi.

---

### 10. Image.network

```
Image.network('https://picsum.photos/200')
```

Widget ini digunakan untuk menampilkan gambar acak yang berasal dari internet.  

---

### 11. Row

```
Row(
```

`Row` digunakan untuk menyusun widget secara horizontal (dari kiri ke kanan).

Pada aplikasi ini Row digunakan untuk menampilkan 3 ikon.

- Food
- Scenery
- People

Setiap ikon terdiri dari **Icon** dan **Text**.

---

### 12. Icon dan Text

Setiap ikon ditampilkan menggunakan kombinasi **Icon** dan **Text**. Pada aplikasi ini terdapat tiga ikon yaitu:

- Food
- Scenery
- People

---

### 13. CounterCard

```
class CounterCard extends StatefulWidget
```

Widget ini menggunakan stateful karena nilai counter dapat berubah ketika tombol ditekan.

Nilai counter disimpan dalam variabel:

```
int _counter = 0;
```

---

### 14. setState()

```
setState(() {
  _counter++;
});
```

`setState()` digunakan untuk memperbarui tampilan ketika nilai counter berubah. Setiap kali tombol ditekan, nilai counter akan bertambah satu dan tampilan pada layar akan ikut diperbarui.

---

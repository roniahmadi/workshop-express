# Langkah 1 - Setting project

Ketika membuat proyek Node.js, Anda akan menginstal banyak hal yang berbeda. Jika Anda ingin berbagi project dengan orang lain, Anda perlu memiliki daftar apa saja  yang harus diinstal, sehingga orang lain tahu apa yang harus diinstal untuk menjalankan proyek tersebut.

Di Node.js, file ini disebut `package.json`. 'Hal-hal yang telah diinstal' disebut sebagai **dependensi**. Membuat file ini adalah langkah pertama dalam mengatur proyek Node.js Anda.

## 1. Membuat file `package.json`

Mari kita mulai dengan membuat file `package.json`. Kami dapat menambahkan hal-hal ke sana sebagai proyek tumbuh. File `package.json` mudah dibuat dari baris perintah. Ketik perintah berikut ke terminal Anda untuk memulai:

```
$ npm init
```

Perintah ini akan menginisialisasi proses selangkah demi selangkah untuk membuat `package.json`. Anda akan melihat sesuatu seperti ini:

![npm init](https://github.com/talkasrul/workshop-express/blob/master/img/initialProject.png?raw=true)

Terminal Anda akan memberi beberapa pertanyaan, tapi tenang itu bukan Quiz:

#### `name`
* npm menyarankan nama default untuk proyek Anda sesuai dalam tanda kurung. Jika Anda ingin memberikan nama yang berbeda, ketik saja nama proyek Anda kemudian tekan `Enter`.
* Jika Anda suka dengan nama default yang disarankan, cukup tekan `Enter`.

#### `version`
* Karena ini proyek pertama Anda, jadi ini akan menjadi versi 1.0.0! Tidak ada yang berubah di sini, jadi cukup tekan `Enter` saja.

#### `description`
* Mendeskripsikan secara sederhana tentang proyek anda. Tulis apapun yang akan mendeskripsikan proyek Anda kemudian tekan `Enter`.

#### `entry point`
* File ini akan menjadi titik awal untuk keseluruhan proyek Anda.
* Mari kita ubah dari `(index.js)` menjadi `app.js`, karena kita akan membangun server aplikasi nanti!
* Ketik `app.js` dan tekan` Enter`.

#### `test command`
* Silahkan lewati saja... tekan `Enter`.

#### `git repository`
* Ini merupakan letak dimana kamu akan menyimpan kode dalam github.  Tekan `Enter`.

#### `keywords`
* (Optional) Ini berguna sebagai kata kunci jika Anda mempublish proyek ke NPM.

#### `author`
* Ini proyek Anda, silahkan masukkan nama atau akun github Anda.

#### `license`
* Pada langkah ini silahkan dilewati saja.

Proses `npm init` telah selesai, silahkan konfirmasi dengan menekan `Enter` maka Anda akan mendapatkan file `package.json` pada folder proyek Anda. Nikmati kode Anda :smile:

### [Langkah 2 >>>>](https://github.com/talkasrul/workshop-express/blob/master/learn/step_02.md)

## Kata Kunci

| Katakunci | Penjelasan |
|-----------|-------------------------------|
| `package.json` | `package.json` adalah file yang digunakan untuk menyimpan informasi proyek Node js, sebagai penamaan dan beberapa dependensi. Baca [disini](http://browsenpm.org/package.json). |
| npm | npm adalah "package manager" untuk Node.js, membantu Anda dalam mengatur semua paket yang dibutuhkan oleh proyek Node js Anda |
| dependencies | Dependencies adalah kode orang lain yang kita pakai pada proyek kita sendiri dengan menginstal dari NPM |

# Step 2 - Install Express

Sebelum menulis kode, Anda harus menginstall librari Express. Kita menggynakan **[Node Package Manager (npm)](https://www.npmjs.com/)** untuk mendownloadnya dengan perintah **`npm install`**.

NPM adalah tempat penyimpanan package yang dapat didownload secara bebas dan terdapat ribuan package yang akan mempermudah Anda dalam mengembangkan proyek Anda sendiri. :smile:

Pada saat kita menginstall Express, maka `package.json` akan melakukan update dengan menambahkan dependensi express kedalam file `package.json`

Jalankan perintah berikut:

`$ npm install express --save`

![proses install express](https://github.com/talkasrul/workshop-express/blob/master/img/installExpress.png?raw=true)

Express yang telah diinstall dapat dilihat pada `package.json`, akan terlihat seperti berikut:

```json
{
  "name": "talkasrul-workshop",
  "version": "1.0.0",
  "description": "",
  "main": "app.js",
  "scripts": {
    "test": "echo \"Error: no test specified\" && exit 1"
  },
  "author": "Asrul H <talkasrul@gmail.com>",
  "license": "ISC",
  "dependencies": {
    "express": "^4.16.4"
  }
}
```



### [Langkah 3 >>>>](https://github.com/talkasrul/workshop-express/blob/master/learn/step_03.md)

## Kata kunci

| Kata kunci | Penjelasan |
|--------|-------------------------------|
| `npm install [package-name]` | Perintah terminal untuk menginstall package atau dependensi dari NPM. |
| `--save` | Ketika ditambahkan `--save` pada perintrah `npm install`, maka package hanya akan diinstall pada proyek itu sendiri. |
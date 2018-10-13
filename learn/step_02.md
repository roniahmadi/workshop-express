# Step 2 - Install Express

Before we write any code, you'll need to install the Express library. We're going to use the **[Node Package Manager (npm)](https://www.npmjs.com/)** to download it using the **`npm install`** command.

NPM is the place to go to download other Node code written by other people.  There are thousands of open-source, 3rd-party Node modules (also known as "packages") by other people that you can download and use in your own projects. 

As we install Express, we'll need to update the `package.json` to add Express as a dependency. We do this so that other people working on the project will know to install Express before running any of the code. This can be done by adding **`--save`** to the end of your command.

Run the following command in your terminal:

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
|--------|:-------------------------------:|
| `npm install [package-name]` | Perintah terminal untuk menginstall package atau dependensi dari NPM. |
| `--save` | Ketika ditambahkan `--save` pada perintrah `npm install`, maka package hanya akan diinstall pada proyek itu sendiri. |
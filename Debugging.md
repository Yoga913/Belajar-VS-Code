# Debugging

1. Membuat Konfigurasi Debugging Pertama Anda
    1. Yang Akan Dibahas
        1. Menjelajahi fitur-fitur alat debugging bawaan
        2. Pelajari bagaimana VS Code melacak konfigurasi debug
        3. Membuat dan menjalankan konfigurasi debug untuk JavaScript di Sisi Klien
    2. Sumber Daya
        1. [Dokumentasi VS Code](https://code.visualstudio.com/docs/editor/debugging)
        2. [Debugger For Chrome](https://marketplace.visualstudio.com/items?itemName=msjsdiag.debugger-for-chrome)
    3. Tips Pro
        1. Debugging yang sebenarnya jauh lebih efisien daripada menggunakan pernyataan console.log(). Luangkan waktu untuk mempelajari alat-alat tersebut dan itu akan membuat Anda menjadi pengembang yang lebih baik.

```json
{
    "type": "chrome",
    "request": "launch",
    "name": "Buka Chrome terhadap localhost",
    "url": "http://localhost:8080",
    "webRoot": "${workspaceFolder}"
}
```

2. Konfigurasi Debugging untuk JavaScript di Sisi Server (Node.js)
    1. Yang Akan Dibahas
        1. Membuat dan menjalankan konfigurasi debug untuk JavaScript di Sisi Server
    2. Sumber Daya
        1. [Dokumentasi VS Code](https://code.visualstudio.com/docs/editor/debugging)

Luncurkan Node (ganti program dengan file server Anda)

```json
{
    "type": "node",
    "request": "launch",
    "name": "Luncurkan Program",
    "program": "${workspaceFolder}/app.js"
}
```

Lampirkan ke Proses (Anda perlu menjalankan aplikasi Anda terlebih dahulu dengan `node --inspect server.js`)

```json
{
    "type": "node",
    "request": "attach",
    "name": "Lampirkan berdasarkan ID Proses",
    "processId": "${command:PickProcess}"
}
```

Lampirkan ke Port (Anda perlu menjalankan aplikasi Anda terlebih dahulu dengan `node --inspect server.js`)

```json
{
    "type": "node",
    "request": "attach",
    "name": "Lampirkan",
    "port": 9229
}
```

Lampirkan ke Port menggunakan Nodemon (Anda perlu menjalankan aplikasi Anda terlebih dahulu dengan `nodemon --inspect server.js`)

```json
{
    "type": "node",
    "request": "attach",
    "name": "Lampirkan",
    "port": 9229,
    "restart": true
}
```

3. Debugging Aplikasi Angular CLI
    1. Yang Akan Dibahas
        1. Membuat dan menjalankan konfigurasi debug untuk Angular
    2. Sumber Daya
        1. [Dokumentasi VS Code](https://code.visualstudio.com/docs/editor/debugging)

Aplikasi Angular CLI (Anda perlu memulai aplikasi Angular Anda sendiri dengan `npm start` atau `ng serve`)

```json
{
    "type": "chrome",
    "request": "launch",
    "name": "Buka Chrome terhadap localhost untuk Angular",
    "url": "http://localhost:4200",
    "webRoot": "${workspaceFolder}"
}
```

4. Debugging Aplikasi Create React App
    1. Yang Akan Dibahas
        1. Membuat dan menjalankan konfigurasi debug untuk Angular
    2. Sumber Daya
        1. [Dokumentasi VS Code](https://code.visualstudio.com/docs/editor/debugging)

Aplikasi Create React App (Anda perlu memulai aplikasi Anda dengan `npm start`)

```json
{
    "type": "chrome",
    "request": "launch",
    "name": "Buka Chrome terhadap localhost untuk React",
    "url": "http://localhost:3000",
    "webRoot": "${workspaceFolder}/src"
}
```

5. Debugging Aplikasi Vue CLI
    1. Yang Akan Dibahas
        1. Membuat dan menjalankan konfigurasi debug untuk Angular
    2. Sumber Daya
        1. [Dokumentasi VS Code](https://code.visualstudio.com/docs/editor/debugging)
        2. [Debugging Vue CLI Apps in VS Code](https://vuejs.org/v2/cookbook/debugging-in-vscode.html)

Aplikasi Vue CLI (Anda perlu memulai aplikasi Anda dengan `npm start`)

```json
{
    "type": "chrome",
    "request": "launch",
    "name": "vuejs: chrome",
    "url": "http://localhost:8080",
    "webRoot": "${workspaceFolder}/src",
    "breakOnLoad": true,
    "sourceMapPathOverrides": {
    "webpack:///src/*": "${webRoot}/*"
    }
}
```

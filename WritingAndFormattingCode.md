# Menulis dan Memformat Kode

1. Potongan Kode
    1. Yang akan kita bahas
        1. Bagaimana potongan kode dikelola oleh VS Code
        2. Cara membuat dan menggunakan potongan kode kustom
    2. Sumber Daya
        1. [Dokumentasi Potongan Kode VS Code](https://code.visualstudio.com/docs/editor/userdefinedsnippets)
    3. Tips Profesional
        1. Buat potongan kode untuk kode yang sering Anda tulis, menggunakan tab stop untuk mengisi segmen secara dinamis.
2. Bekerja dengan Markdown
    1. Yang akan kita bahas
        1. Cara menulis dan melihat pratinjau Markdown di VS Code
        2. Ekstensi Markdown dengan pintasan tambahan untuk bekerja dengan Markdown
    2. Sumber Daya
        1. [Dokumentasi Markdown VS Code](https://code.visualstudio.com/docs/languages/markdown)
        2. [Template ReadMe](https://github.com/jamesqquick/read-me-template)
        3. [Lembar Kerja Markdown](https://github.com/jamesqquick/markdown-worksheet)
        4. [Lint Markdown](https://marketplace.visualstudio.com/items?itemName=DavidAnson.vscode-markdownlint)
        5. [Pintasan Markdown](https://marketplace.visualstudio.com/items?itemName=mdickin.markdown-shortcuts)
        6. [TOC Markdown](https://marketplace.visualstudio.com/items?itemName=AlanWalk.markdown-toc)
    3. Tips Profesional
        1. Repositori Github terbaik mengandung berkas ReadMe.md yang detail. Gunakan VS Code untuk membuat berkas ReadMe bersama dengan pengembangan.
        2. `ctrlCmd+ Shift + V`  – buka pratinjau markdown
        3. `Cmd + Shift + K V` | `Ctrl + K + V` – buka pratinjau markdown berdampingan
3. Mengatur Kode
    1. Yang akan kita bahas
        1. Mengenali dan menghapus variabel yang tidak terpakai
        2. Mengatur pernyataan impor
        3. Refaktor kode ke berkas baru
        4. Menggunakan panduan indentasi yang disorot
        5. Melipat kode
        6. Mengubah nama variabel
    2. Tips Profesional
        1. `Shift + Alt + F` – memformat dokumen
        2. `ctrlCmd + .` – untuk menampilkan tindakan kode yang tersedia
        3. `Command Palette` -> Organize Imports – mengatur impor
        4. `ctrlCmd + /` – mengalihkan baris komentar
        6. `ctrlCmd + Option [` - meminimalkan wilayah lipatan kode
        7. `ctrlCmd + Option ]` - memaksimalkan wilayah lipatan kode
        8. `ctrlCmd + K ctrlCmd + 0` – meminimalkan semua wilayah lipatan kode
        9. `ctrlCmd + K ctrlCmd + J` – memaksimalkan semua wilayah lipatan kode
4. Membuat Pengaturan Editor Standar dengan Editor Config
    1. Yang akan kita bahas
        1. Bagaimana berkas konfigurasi editor dapat digunakan untuk menetapkan pengaturan editor standar di beberapa editor
        2. Ekstensi Editor Config untuk VS Code agar VS Code dapat mengenali dan menghormati berkas konfigurasi editor
        3. Membuat berkas konfigurasi editor untuk mengganti pengaturan VS Code dan secara otomatis memformat kode saat disimpan
    2. Sumber Daya
        1. [Ekstensi Editor Config untuk VS Code](https://marketplace.visualstudio.com/items?itemName=EditorConfig.EditorConfig)
        2. [Editor Config](https://editorconfig.org/)
    3. Tips Profesional
        1. Tab vs Spasi (dan seterusnya dan seterusnya)... pilih apa yang cocok untuk Anda dan tim Anda
5. Memformat Kode dengan Prettier
    1. Yang akan kita bahas
        1. Cara menginstal ekstensi Prettier untuk VS Code
        2. Membuat konfigurasi Prettier atau menyesuaikan pengaturan Prettier untuk memformat kode
        3. Memformat kode secara manual dan otomatis
    2. Sumber Daya
        1. [Ekstensi Pemformat Kode Prettier](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode)
    3. Tips Profesional
        1. Temukan konfigurasi yang cocok untuk Anda dan tetaplah menggunakan konfigurasi tersebut
6. Linting dan Memformat Kode JavaScript dengan ESLint
    1. Yang akan kita bahas
        1. Cara menginstal paket ESLint
        2. Cara membuat berkas konfigurasi ESLint dan/atau menginstal dan menyesuaikan ekstensi ESLint
        3. Memformat kode secara manual dan otomatis
    2. Sumber Daya
        1. [Ekstensi ESLint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint)
        2. [Panduan Memulai ESLint](https://eslint.org/docs/user-guide/getting-started)
    3. Tips Profesional
        1. Temukan konfigurasi yang cocok untuk Anda dan tetaplah menggunakan konfigurasi tersebut
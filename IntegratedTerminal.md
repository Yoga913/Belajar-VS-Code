# Terminal Terintegrasi

1. Terminal Terintegrasi di VS Code
    1. Yang Akan Dibahas
        1. Cara membuka dan menggunakan Terminal Terintegrasi
        2. Bekerja dengan beberapa terminal
        3. Cara memilih shell terintegrasi Anda
    2. Sumber Daya
        1. [Dokumentasi Terminal Terintegrasi VS Code](https://code.visualstudio.com/docs/editor/integrated-terminal)
    3. Tips Profesional
        1. Beberapa lebih suka menggunakan terminal luar daripada yang terintegrasi ke dalam VS Code. Cobalah terminal terintegrasi dan putuskan sendiri.
        2. `ctrlCmd + Tilde` – beralih terminal terintegrasi
2. Menyesuaikan Pengaturan Terminal Anda Bagian 2
    1. Yang Akan Dibahas
        1. Cara menyesuaikan pintasan untuk berinteraksi dengan jendela terminal seperti berkas di editor (membuka, menutup, dan beralih antara jendela terminal)
    2. Sumber Daya
        1. [Dokumentasi Terminal Terintegrasi VS Code](https://code.visualstudio.com/docs/editor/integrated-terminal)
    3. Tips Profesional
        1. Menggunakan konfigurasi di atas dapat membuatnya jauh lebih cepat dan mudah untuk bekerja dengan beberapa jendela terminal. 

```json
{
    "key": "ctrl+tab",
    "command": "workbench.action.terminal.focusNext",
    "when": "terminalFocus"
},
{
    "key": "ctrl+shift+tab",
    "command": "workbench.action.terminal.focusPrevious",
    "when": "terminalFocus"
},
{
    "key": "cmd+n",
    "command": "workbench.action.terminal.new",
    "when": "terminalFocus"
},
{
    "key": "cmd+w",
    "command": "workbench.action.terminal.kill",
    "when": "terminalFocus"
},
{
    "key": "cmd+r",
    "command": "workbench.action.terminal.rename",
    "when": "terminalFocus"
}
```
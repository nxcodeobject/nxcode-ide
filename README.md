 # NxCode IDE ΓÇö Berkas Unduhan

Folder ini berisi paket siap pakai **NxCode IDE** untuk tiap sistem operasi.
Berkas di sini yang diunggah ke halaman rilis GitHub dan ditautkan dari website.

## Berkas

| Berkas | Sistem | Ukuran | SHA-256 |
| --- | --- | --- | --- |
| `NxCode-IDE-Setup-1.0.8.exe` | Windows 10/11 (64-bit) | ┬▒ 74 MB | `CBCCAB270943B1682C094D3B9BB36EF33148F56C2D9BA4129BE5D3596B61533D` |
| `NxCode-IDE-1.0.8-linux-x64.tar.gz` | Linux (x64) | ± 14 MB | `ABFF954258FC1B7F2CDCC5646641451BF8BDC1AE1C0871C4D5E09BAB1F85D508` |
| `NxCode-IDE-Setup-1.0.7.exe` | Windows 10/11 (64-bit) | ┬▒ 74 MB | `05C534F960965D495DB86FAF67FBD7EB6C7E8125C622A229A2B8ADADB0DD2FA0` |
| `NxCode-IDE-Setup-1.0.6.exe` | Windows 10/11 (64-bit) | ┬▒ 74 MB | `E54947295ACB722E81A6CF3F42D4A0DCCE172446CD3A72753DDAE2BD4A9A7B18` |
| `NxCode-IDE-1.0.6-linux-x64.tar.gz` | Linux (x64) | ┬▒ 14 MB | `45102B592E453EA6207EE596A79AA88122057EF167E87EDAF36025790BDB6356` |
| `NxCode-IDE-Setup-1.0.5.exe` | Windows 10/11 (64-bit) | ┬▒ 57 MB | `D67A53C680A667A1112E1A45CBBB54CDFDCB74D9F1A0F5326071ACBF2E798A6A` |
| `NxCode-IDE-1.0.5-linux-x64.tar.gz` | Linux (x64) | ┬▒ 14 MB | `0194179822E229B0DBD6F658C4D7946A8B0A81C28FF835E46C8D06982A59EF23` |
| `NxCode-IDE-Setup-1.0.4.exe` | Windows 10/11 (64-bit) | ┬▒ 57 MB | `BB2CFFB7D67D7A3B7F746F87B6427B2532309328A6699818B0DC89D5FDC090C6` |
| `NxCode-IDE-Setup-1.0.3.exe` | Windows 10/11 (64-bit) | ┬▒ 54 MB | `B53EF598EE46D81A9896C327DDAB94DF4C544C814F842332F621FC73AC157BB0` |
| `NxCode-IDE-Setup-1.0.2.exe` | Windows 10/11 (64-bit) | ┬▒ 54 MB | `524764F3D48697BA99DC4EAC7CC576509E50C1D8943AFCF8B434C305AE33577C` |
| `NxCode-IDE-Setup-1.0.0.exe` | Windows 10/11 (64-bit) | ┬▒ 54 MB | `8DA7F5CEE66378A96A036DB974E26AB62B2EA7E7ED950506915CC405353B465F` |

### v1.0.8 (Windows & Linux)

- **Menulis**: multi-kursor (`Ctrl+klik`, `Ctrl+Alt+Γåæ/Γåô`, `Ctrl+Shift+L`).
  `Ctrl+Shift` + tahan tombol kiri + geser membuat seleksi blok. `Esc` menyisakan satu kursor.
- **Explorer**: `Ctrl+klik` menandai beberapa file. Salin, hapus, dan tarik ke terminal memakai semua yang ditandai.
- **Terminal**: panel kanan dan bawah tetap responsif saat agen AI menulis banyak berkas. Log dibatasi 5000 baris.

### v1.0.7 (Windows)

- **Jendela baru**: tarik tab file, gambar, atau PDF keluar dari jendela membuka
  jendela baru di dekat kursor (gaya Sublime). Jatuhkan tab ke jendela yang
  sudah ada untuk memindahkannya. Tab panel (Source Control, API, Settings)
  tetap di jendelanya.
- **Paste**: `Ctrl+V` menempel di posisi kursor, bukan sebagai baris baru.
  `Ctrl+Z` mengembalikan kursor ke tempat edit, tidak meloncat ke baris 1.
- **Explorer**: seret file atau folder dari pohon ke terminal kembali menulis
  `@path` di prompt.

### v1.0.6 (Windows & Linux)

- **Perbaikan tampilan font**: bila font editor (Consolas) tidak terpasang,
  editor kini memakai fallback font monospace sistem ΓÇö memperbaiki karakter
  spasi yang tampil dengan garis/artefak akibat substitusi font sembarangan.
- **UX menulis**: `Backspace` di indentasi spasi menghapus satu unit indent
  (bukan satu spasi); `Home` pintar (awal indent Γåö kolom 0); kursor lebih tebal (2px).
- Menulis: `Ctrl+C` tanpa seleksi menyalin baris, `Ctrl+V` baris baru (v1.0.5).
- **Explorer**: menu **"Open in Terminal"** dipindah ke baris ke-2 (setelah
  "New File") karena sering dipakai.

### v1.0.5 (Windows & Linux)

- **Terminal bebas dari shortcut aplikasi**: saat fokus di dalam panel terminal
  (kanan/bawah), shortcut aplikasi tidak lagi mencuri tombol. AI coding agent
  (claude/opencode/vim, dsb.) kini menerima `Ctrl+S`, `Ctrl+W`, `Ctrl+N`,
  `Ctrl+B`, `Ctrl+P`, `Alt+ΓåÉ/ΓåÆ`, dan lainnya secara utuh. Yang tetap aktif dari
  dalam terminal hanya `Ctrl+`` (toggle panel) dan `Ctrl+Shift+P` (command palette).
- **UX editor**: `Tab` mengikuti preferensi indentasi (spasi/tab) + `Shift+Tab`
  outdent; `Alt+Γåæ/Γåô` pindah baris; `Shift+Alt+Γåô` duplikat baris;
  `Alt+Z` toggle word wrap; `Shift+Alt+A` toggle komentar blok.
- **Clipboard**: `Ctrl+C` tanpa seleksi menyalin seluruh baris kursor;
  `Ctrl+V` menempel sebagai baris baru di bawah baris kursor.

### v1.0.4 (Windows)

- **PDF Viewer**: membuka berkas `.pdf` kini menampilkan halaman PDF LANGSUNG di
  dalam editor (bukan teks biner). Navigasi halaman (prev/next), zoom
  (Ctrl+wheel / menu View), fit/actual size, info bar "hal N/total ┬╖ zoom ┬╖ ukuran",
  dan muat-ulang otomatis saat berkas berubah. Render memakai **PDFium**
  (mesin PDF Chromium, BSD) yang ikut di dalam paket.
- **Perbaikan**: ekspor Markdown -> PDF (v1.0.3) sempat mencetak teks
  **mikroskopis** karena ukuran halaman dokumen meleset. Sudah diperbaiki.

### v1.0.3 (Windows)

- **Ekspor Markdown -> PDF**: bar markdown kini `[Markdown | Preview | HTML | PDF]`.
  Tab **PDF** mengekspor dokumen `.md` ke `.pdf` (sibling, A4, margin 15 mm),
  memakai `QPdfWriter` bawaan Qt ΓÇö tanpa dependency eksternal.

### v1.0.2 (Windows)

- **New File** kini otomatis mendaftar **400+ bahasa** dari grammar KSyntaxHighlighting,
  dikelompokkan per kategori (Sources, Markup, Scripts, dst.), dengan 22 bahasa
  umum (HTML, JS, CSS, JSON, Markdown, PHP, C/C++, Python, dll.) tampil di atas
  menu untuk akses cepat.
- Penyuntingan: auto-indent, auto-tutup kurung/kutip/tag, multi-kursor (Ctrl+D),
  go-to-bracket (Ctrl+M), deteksi indentasi, snippet bawaan, dan Find-in-Selection
  dengan Preserve Case.

> macOS belum tersedia ΓÇö SDK NXC belum menyediakan aset untuk platform itu.

## Cara Pasang

### Windows

1. Unduh `NxCode-IDE-Setup-1.0.7.exe`.
2. Jalankan. Karena belum ditandatangani, Windows SmartScreen mungkin muncul ΓÇö
   pilih **More info** lalu **Run anyway**.
3. Ikuti wizard: folder instal, shortcut Start Menu / Desktop, lalu selesai.

Installer bersifat per-user (tidak butuh admin) dan memperbarui instalasi lama
(sekarang AppId tetap). Runtime Visual C++ sudah ikut di dalam paket.

### Linux

```bash
tar -xzf NxCode-IDE-1.0.6-linux-x64.tar.gz
cd NxCode-IDE-1.0.6-linux-x64
./editor
```

Jenjang minimum: distribusi Linux 64-bit dengan **Qt 6** terpasang
(mis. `sudo apt install qt6-base-dev qt6-svg-dev` di Ubuntu/Debian), serta
`libnxc.so.0` dari **NXC SDK 0.3.5** (Linux) tersedia di `LD_LIBRARY_PATH`:

```bash
export LD_LIBRARY_PATH="$HOME/.nxc/sdk/nxc-sdk-0.3.5-qt6.8.3-linux/lib:$LD_LIBRARY_PATH"
./editor
```

Catatan: paket ini **belum self-contained** ΓÇö Qt 6 dan `libnxc.so.0` diambil
dari sistem. Untuk mesin tanpa Qt, perlu bundel Qt (AppImage/linuxdeployqt).

## Kebutuhan Umum

- Windows 10 (1809+) / 11 64-bit, **atau** Linux 64-bit dengan Qt 6.
- Perangkat keras standar; tidak butuh GPU khusus.

## Verifikasi Integritas

```powershell
# Windows
Get-FileHash .\NxCode-IDE-Setup-1.0.7.exe -Algorithm SHA256
```

```bash
# Linux
sha256sum NxCode-IDE-1.0.6-linux-x64.tar.gz
```

Bandingkan hasilnya dengan tabel di atas.

## Dibangun Dari

- NXC SDK **0.3.5** (Qt 6.8.3).
- Windows: Visual Studio 2022 (MSVC), Inno Setup.
- Linux: GCC 15 + Qt 6, Ninja.

Sumber kode & lisensi ada di repo aplikasi. Nama produk: **NxCode IDE**
(Nusantara eXtreme Development Object Model).

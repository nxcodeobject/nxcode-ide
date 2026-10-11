 # NxCode IDE — Berkas Unduhan

Folder ini berisi paket siap pakai **NxCode IDE** untuk tiap sistem operasi.
Berkas di sini yang diunggah ke halaman rilis GitHub dan ditautkan dari website.

## Berkas

| Berkas | Sistem | Ukuran | SHA-256 |
| --- | --- | --- | --- |
| `NxCode-IDE-Setup-1.0.0.exe` | Windows 10/11 (64-bit) | ± 54 MB | `BD46E4FE32F868B3975C678ABE9A23BE2903BF67B1BB8292BEFAD9E48CF2A6EA` |
| `NxCode-IDE-1.0.0-linux-x64.tar.gz` | Linux (x64) | ± 10 MB | `6060538C36560B64F05E2539DE66DD4E16428A8B946316EC93CCE0977C1154A4` |

> macOS belum tersedia — SDK NXC belum menyediakan aset untuk platform itu.

## Cara Pasang

### Windows

1. Unduh `NxCode-IDE-Setup-1.0.0.exe`.
2. Jalankan. Karena belum ditandatangani, Windows SmartScreen mungkin muncul —
   pilih **More info** lalu **Run anyway**.
3. Ikuti wizard: folder instal, shortcut Start Menu / Desktop, lalu selesai.

Installer bersifat per-user (tidak butuh admin) dan memperbarui instalasi lama
(sekarang AppId tetap). Runtime Visual C++ sudah ikut di dalam paket.

### Linux

```bash
tar -xzf NxCode-IDE-1.0.0-linux-x64.tar.gz
cd NxCode-IDE-1.0.0-linux-x64
./editor
```

Jenjang minimum: distribusi Linux 64-bit dengan **Qt 6** terpasang
(mis. `sudo apt install qt6-base-dev qt6-svg-dev` di Ubuntu/Debian), serta
`libnxc.so.0` dari **NXC SDK 0.3.5** (Linux) tersedia di `LD_LIBRARY_PATH`:

```bash
export LD_LIBRARY_PATH="$HOME/.nxc/sdk/nxc-sdk-0.3.5-qt6.8.3-linux/lib:$LD_LIBRARY_PATH"
./editor
```

Catatan: paket ini **belum self-contained** — Qt 6 dan `libnxc.so.0` diambil
dari sistem. Untuk mesin tanpa Qt, perlu bundel Qt (AppImage/linuxdeployqt).

## Kebutuhan Umum

- Windows 10 (1809+) / 11 64-bit, **atau** Linux 64-bit dengan Qt 6.
- Perangkat keras standar; tidak butuh GPU khusus.

## Verifikasi Integritas

```powershell
# Windows
Get-FileHash .\NxCode-IDE-Setup-1.0.0.exe -Algorithm SHA256
```

```bash
# Linux
sha256sum NxCode-IDE-1.0.0-linux-x64.tar.gz
```

Bandingkan hasilnya dengan tabel di atas.

## Dibangun Dari

- NXC SDK **0.3.5** (Qt 6.8.3).
- Windows: Visual Studio 2022 (MSVC), Inno Setup.
- Linux: GCC 15 + Qt 6, Ninja.

Sumber kode & lisensi ada di repo aplikasi. Nama produk: **NxCode IDE**
(Nusantara eXtreme Development Object Model).

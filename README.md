# Agenda Harian 
**Siti Aisyah Nor Fitriani - 2210010043 - UTS**

## Deskripsi Aplikasi
Aplikasi **Agenda Harian** adalah aplikasi desktop berbasis Java Swing yang membantu pengguna mengelola agenda harian mereka. Aplikasi ini mendukung fitur seperti login pengguna, pengisian agenda berdasarkan hari, penyimpanan ke database, serta ekspor dan impor data menggunakan file CSV.

---

## Fitur Utama

- **Login:**
  - Validasi username dan password menggunakan database.
  - Pesan notifikasi login berhasil atau gagal.

- **Tambah Agenda:**
  - Tambahkan agenda harian berdasarkan tanggal, pukul, hari, dan nama agenda.

- **Ubah Agenda:**
  - Edit data langsung di tabel sebelum disimpan ke database.

- **Hapus Agenda:**
  - Hapus baris tertentu dari tabel dengan konfirmasi.

- **Simpan ke Database:**
  - Menyimpan semua data di tabel ke database MySQL.

- **Muat Data dari Database:**
  - Memuat semua data agenda yang tersimpan di database ke dalam tabel.

- **simpan ke file  :**
  - Simpan semua data di tabel ke dalam file CSV.

- **Impor dari CSV:**
  - Memuat data dari file CSV ke database dengan validasi format file.

- **Reset Tabel:**
  - Menghapus semua data di tabel tanpa memengaruhi data yang sudah tersimpan di database.

---

## Cara Menggunakan Aplikasi

### 1. Login
- Masukkan **username** dan **password**.
- Klik tombol **MASUK** untuk login.
- Jika login berhasil, pengguna akan diarahkan ke form utama untuk mengelola agenda.

### 2. Tambah Agenda
- Pilih **hari** menggunakan combobox.
- Masukkan **tanggal** dengan memilih dari kalender.
- Masukkan **pukul** dan **nama agenda**.
- Klik tombol **Masukkan Ke Daftar Agenda** untuk menambahkan ke tabel.

### 3. Ubah Agenda
- Pilih baris di tabel yang ingin diubah.
- Data dari baris yang dipilih akan otomatis terisi ke input form.
- Lakukan perubahan pada input form.
- Klik tombol **UBAH** untuk menyimpan perubahan ke tabel.

### 4. Hapus Agenda
- Pilih baris di tabel yang ingin dihapus.
- Klik tombol **HAPUS**.
- Konfirmasi penghapusan akan muncul sebelum baris dihapus.

### 5. Simpan ke Database
- Klik tombol **Simpan ke Database** untuk menyimpan semua data di tabel ke database.

### 6. Muat Data
- Klik tombol **Muat Data** untuk memuat data dari database ke tabel.

### 7. simpan ke CSV
- Klik tombol **Simpan ke File** untuk mengekspor data tabel ke file CSV.

### 8. Impor dari CSV
- Klik tombol **Impor** untuk memuat data dari file CSV ke database.

### 9. Reset Tabel
- Klik tombol **Reset** untuk mengosongkan tabel dan membersihkan semua input form.

### 10. Keluar
- Klik tombol **KELUAR** untuk menutup aplikasi.
- Akan muncul dialog konfirmasi sebelum aplikasi ditutup.

---

## Struktur Database

### Tabel `users`
| Kolom          | Tipe Data     | Keterangan               |
|----------------|---------------|--------------------------|
| `id`           | INT           | Primary key, auto increment |
| `username`     | VARCHAR(50)   | Username pengguna        |
| `nama_lengkap` | VARCHAR(100)  | Nama lengkap pengguna    |
| `email`        | VARCHAR(100)  | Email pengguna           |
| `no_hp`        | VARCHAR(20)   | Nomor HP pengguna        |
| `password`     | VARCHAR(100)  | Password pengguna        |

### Tabel `agenda`
| Kolom   | Tipe Data | Keterangan                |
|---------|-----------|-------------------------  |
| `tanggal` | DATE      | Tanggal agenda          |
| `pukul`   | VARCHAR(20) | Waktu pelaksanaan     |
| `senin`   | TEXT      | Agenda hari Senin       |
| `selasa`  | TEXT      | Agenda hari Selasa      |
| `rabu`    | TEXT      | Agenda hari Rabu        |
| `kamis`   | TEXT      | Agenda hari Kamis       |
| `jumat`   | TEXT      | Agenda hari Jumat       |
| `sabtu`   | TEXT      | Agenda hari Sabtu       |
| `minggu`  | TEXT      | Agenda hari Minggu      |

---
### DEMO
![Demo Aplikasi](img/UTS.gif)

---
## Catatan
1. Pastikan input tanggal, pukul, dan nama agenda tidak kosong saat menambahkan atau mengubah agenda.

---

## Pembuat Aplikasi
**Nama:** Siti Aisyah Nor Fitriani  
**NPM:** 2210010043  
**UTS** 

---



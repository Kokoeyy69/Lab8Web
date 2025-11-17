# 📘 Praktikum 8 – PHP dan MySQL

---

# 1. Tujuan Praktikum
Praktikum ini bertujuan untuk memahami cara:
- Menghubungkan PHP dengan MySQL.
- Membuat aplikasi CRUD (Create, Read, Update, Delete).
- Mengelola data menggunakan query SQL.
- Mengupload file (gambar) ke server.
- Menampilkan data dari database dalam format tabel.

---

# 2. Membuat Database dan Tabel

### Database yang digunakan:
latihan1

### Struktur tabel:
data_barang
```
id_barang INT AUTO_INCREMENT
kategori VARCHAR(100)
nama VARCHAR(200)
gambar VARCHAR(200)
harga_beli INT
harga_jual INT
stok INT
```
<img width="1366" height="740" alt="image" src="https://github.com/user-attachments/assets/e27e1a03-004e-4335-ba82-c33a5e62e213" />

---

# 3. Koneksi Database (koneksi.php)

```php
<?php
$host = "localhost";
$user = "root";
$pass = "";
$db = "latihan1";

$conn = mysqli_connect($host, $user, $pass, $db);

if (!$conn) {
    die("Koneksi gagal: " . mysqli_connect_error());
}
?>
```

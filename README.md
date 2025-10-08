# 🧾 InfoCekBantuan

**Frontend:** HTML, CSS, JavaScript
**Backend:** Supabase
**Tema:** Transparansi dan Akuntabilitas Program Sosial Pemerintah

---

## 📌 Deskripsi Proyek

**InfoCekBantuan** adalah sebuah platform digital berbasis web yang dirancang untuk meningkatkan **transparansi** dan **akuntabilitas program bantuan sosial pemerintah**.
Melalui aplikasi ini, masyarakat dapat secara langsung melakukan pengecekan status penerimaan bantuan sosial berdasarkan **NIK** yang mereka masukkan, mengetahui apakah mereka terdaftar dalam **DTKS (Data Terpadu Kesejahteraan Sosial)**, serta melihat daftar bantuan yang diterima.

Platform ini tidak hanya memberikan akses informasi yang terbuka, tetapi juga menyediakan jalur pelaporan langsung apabila ditemukan **kasus salah sasaran atau ketidaksesuaian data**.

---

## 🎯 Tujuan Utama

* **Meningkatkan transparansi**: Masyarakat dapat mengetahui secara mandiri status bantuan sosial yang diterima.
* **Meningkatkan akuntabilitas**: Masyarakat dan pemerintah desa dapat melaporkan serta menindaklanjuti data yang tidak valid atau salah sasaran.
* **Mempermudah akses informasi**: Memberikan berita, panduan, dan update terbaru mengenai program bantuan sosial secara lengkap dan ringkas.

---

## 🧩 Fitur Utama

### 1. 🔍 **Cek Bantuan Sosial**

* Pengguna dapat memasukkan **NIK** untuk memeriksa:

  * Status terdaftar/tidak di **DTKS**.
  * Jenis bantuan sosial yang sedang diterima.
* Data diambil dari **Supabase** sebagai backend database.

### 2. 📣 **Pelaporan ke Desa dan Dinas Sosial**

* Jika warga merasa **tidak menerima bantuan padahal terdaftar di DTKS**, mereka dapat:

  * Menghubungi **pihak desa** yang tercantum di web.
  * Atau melalui **form pelaporan online** yang diinputkan langsung oleh perangkat desa.
* Laporan tersebut akan diteruskan secara otomatis ke **Dinas Sosial atau instansi terkait** melalui sistem berbasis Supabase.

### 3. 🏠 **Dashboard Desa**

* Login khusus perangkat desa (contoh: *Desa Dukuh Waluh*).
* Dapat melihat laporan warga dan mengirim data verifikasi ke dinas sosial.

### 4. 📰 **Berita dan Informasi Bantuan Sosial**

* Menyediakan update terkini seputar kebijakan bantuan sosial, perubahan regulasi, dan tips verifikasi data.
* Didesain agar informatif, ringkas, dan mudah dipahami masyarakat.

---

## ⚙️ Arsitektur Sistem

```
[User/Masyarakat] --> [Frontend: HTML, CSS, JS]
       ↓
   Input NIK
       ↓
 [Supabase Database]
       ↓
  [DTKS Data + Data Bantuan]
       ↓
   Output hasil cek

[Desa/Kelurahan] --> [Login Panel] --> [Form Laporan]
       ↓
   [Supabase Backend]
       ↓
 [Dinas Sosial menerima data pelaporan]
```

---

## 🧠 Teknologi yang Digunakan

| Komponen     | Teknologi                                                                       |
| ------------ | ------------------------------------------------------------------------------- |
| **Frontend** | HTML5, CSS3 (modern responsive design), JavaScript (Vanilla JS)                 |
| **Backend**  | Supabase (Authentication, Database, API)                                        |
| **UI Theme** | Merah–Biru dengan gaya minimalis dan modern                                     |
| **Keamanan** | Validasi input, autentikasi desa, dan pengelolaan data laporan secara real-time |

---


 🧾 Alur Penggunaan Sistem

1. **Masyarakat membuka web InfoCekBantuan.**
   Mereka memasukkan NIK → Sistem menampilkan hasil pencarian (terdaftar DTKS/tidak, jenis bantuan yang diterima).

2. **Jika ada ketidaksesuaian**, masyarakat dapat **menghubungi pihak desa** melalui kontak yang tersedia atau secara langsung datang ke kantor desa.

3. **Perangkat Desa melakukan login** di sistem (contoh: Desa Dukuh Waluh).
   Setelah login, perangkat desa dapat mengisi **form laporan** dan mengirimkannya ke **Dinas Sosial**.

4. **Dinas Sosial** menerima laporan, melakukan validasi, dan memperbarui data di Supabase bila diperlukan.

5. **Masyarakat juga dapat membaca berita terbaru** mengenai bantuan sosial langsung dari halaman utama InfoCekBantuan.

---

## 🌍 Manfaat untuk Masyarakat dan Pemerintah

| Pihak                | Manfaat                                                                |
| -------------------- | ---------------------------------------------------------------------- |
| **Masyarakat**       | Akses informasi yang jelas, terbuka, dan cepat terkait bantuan sosial. |
| **Pemerintah Desa**  | Alat pelaporan digital yang efisien dan transparan.                    |
| **Dinas Sosial**     | Data pelaporan yang lebih akurat dan mudah diverifikasi.               |
| **Pemerintah Pusat** | Meningkatkan kepercayaan publik terhadap program bantuan sosial.       |

---

 💡 Kesimpulan

**InfoCekBantuan** hadir sebagai solusi konkret untuk mewujudkan **transparansi dan akuntabilitas program sosial pemerintah**.
Dengan sistem berbasis web yang mudah diakses, masyarakat tidak lagi kesulitan mengetahui hak mereka terhadap bantuan sosial.
Sementara itu, perangkat desa dan dinas sosial memperoleh jalur pelaporan yang efisien, akurat, dan terintegrasi.

Aplikasi ini sekaligus menjadi **jembatan digital antara pemerintah dan masyarakat**, memastikan bahwa setiap bantuan sosial benar-benar **tepat sasaran dan transparan bagi semua.

---


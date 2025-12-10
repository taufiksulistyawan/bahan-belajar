Kalau **Microsoft Excel 2013 sering force close (keluar sendiri)**, itu bisa disebabkan oleh beberapa hal: add-ins yang bermasalah, file corrupt, instalasi rusak, atau masalah kompatibilitas. Berikut langkah-langkah perbaikan **paling efektif dan berurutan** 👇

---

### 🧩 1. Jalankan Excel dalam **Safe Mode**

Untuk mengecek apakah masalahnya berasal dari Add-ins atau ekstensi.

**Langkah:**

1. Tekan `Windows + R`
2. Ketik:

   ```
   excel /safe
   ```
3. Tekan **Enter**

Jika Excel bisa terbuka normal dan tidak force close, berarti penyebabnya **add-ins**.

---

### ⚙️ 2. Nonaktifkan Semua Add-ins

**Langkah:**

1. Buka Excel (kalau bisa lewat Safe Mode).
2. Masuk ke menu:

   ```
   File > Options > Add-ins
   ```
3. Di bawah jendela, ubah **Manage: COM Add-ins**, lalu klik **Go**.
4. Hilangkan semua centang, klik **OK**.
5. Tutup dan buka Excel lagi.

> ✅ Jika sudah normal, aktifkan add-ins satu per satu untuk menemukan penyebabnya.

---

### 🧰 3. Lakukan **Repair Office**

Kadang instalasi Office rusak sebagian.

**Langkah:**

1. Tekan `Windows + R`, ketik:

   ```
   appwiz.cpl
   ```
2. Tekan **Enter** → buka daftar program.
3. Cari **Microsoft Office 2013**
4. Klik kanan → **Change** → pilih **Repair**

   * Pilih **Quick Repair** dulu.
   * Jika belum berhasil, ulangi dengan **Online Repair** (butuh koneksi internet).

---

### 🧼 4. Hapus Cache & Temporary File

Cache Office bisa menyebabkan crash.

**Langkah:**

1. Tekan `Windows + R`
2. Ketik:

   ```
   %temp%
   ```
3. Hapus semua file di folder tersebut (lewati yang tidak bisa dihapus).

---

### 💾 5. Nonaktifkan Hardware Acceleration

**Langkah:**

1. Buka Excel.
2. Masuk ke:

   ```
   File > Options > Advanced
   ```
3. Scroll ke bawah ke bagian **Display**.
4. Centang **Disable hardware graphics acceleration**.
5. Klik **OK**, lalu restart Excel.

---

### 🧱 6. Update Office dan Windows

Buka **Windows Update** dan pastikan semua pembaruan terpasang, termasuk Office update (bisa juga lewat Control Panel → Windows Update → Check for updates).

---

### 📂 7. Cek File Excel yang Bermasalah

Jika Excel hanya crash saat membuka file tertentu:

* Coba buka file tersebut di **komputer lain**.
* Coba buka dari Excel Safe Mode.
* Jika tetap crash, file mungkin corrupt — coba buka lewat:

  ```
  File > Open > Browse > pilih file > panah bawah di tombol Open > Open and Repair
  ```

---

### 💡 8. (Opsional) Reset Setting Excel

Jika semua langkah gagal, reset registry Excel:

**Langkah:**

1. Tekan `Windows + R`, ketik `regedit`
2. Arahkan ke:

   ```
   HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Excel
   ```
3. Klik kanan folder **Excel** → pilih **Export** (untuk backup)
4. Setelah itu, klik kanan lagi → **Delete**
5. Tutup Registry Editor, lalu buka Excel lagi.

> Excel akan membuat ulang pengaturan default otomatis.

---

Kalau kamu mau, kirimkan:

* Pesan error (kalau muncul sebelum force close)
* Kapan biasanya terjadi (saat buka file, edit, atau simpan)

Nanti saya bantu diagnosa lebih spesifik. Mau saya bantu urutkan langkah **paling aman dan cepat untuk dicoba dulu**?

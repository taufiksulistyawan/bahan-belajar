Oke 👍 saya susun **roadmap belajar Ubuntu Server selama 6 minggu**. Ini fleksibel ya, bisa lebih cepat atau lebih lama tergantung waktu kamu.

---

# 🗂 Roadmap Belajar Ubuntu Server (6 Minggu)

## 📌 Minggu 1 – Dasar Linux & Instalasi

* Install Ubuntu Server (di **VirtualBox**, **Proxmox**, atau **VPS murah**).
* Belajar command dasar:

  * Navigasi file (`ls`, `cd`, `pwd`)
  * Kelola file/folder (`cp`, `mv`, `rm`, `mkdir`)
  * Permission (`chmod`, `chown`)
* Kenali struktur folder Linux (`/etc`, `/var`, `/home`, `/srv`).
* Update & upgrade sistem:

  ```bash
  sudo apt update && sudo apt upgrade -y
  ```

---

## 📌 Minggu 2 – Networking & SSH

* Konfigurasi IP statis dengan **Netplan**.
* Cek koneksi internet (`ping`, `curl`, `wget`).
* Install & konfigurasi SSH:

  ```bash
  sudo apt install openssh-server -y
  ```
* Belajar remote SSH dari komputer lain.
* Kenali **UFW firewall** (allow port 22, 80, 443).

---

## 📌 Minggu 3 – Service Dasar & Manajemen User

* Belajar **systemctl** (start, stop, restart service).
* Buat user baru & beri akses sudo:

  ```bash
  adduser namauser
  usermod -aG sudo namauser
  ```
* Latihan dengan `cron` (jadwal otomatis).
* Pasang tool monitoring:

  ```bash
  sudo apt install htop glances -y
  ```

---

## 📌 Minggu 4 – Web Server & Database

* Install **Nginx**:

  ```bash
  sudo apt install nginx -y
  ```
* Buat virtual host sederhana.
* Install **MariaDB** / **PostgreSQL**.
* Latihan buat database + user.
* Coba deploy **WordPress** atau aplikasi PHP sederhana.

---

## 📌 Minggu 5 – File Sharing & Docker

* Install **Samba** untuk file sharing dengan Windows.
* Uji akses lewat Windows Explorer (`\\ip-server`).
* Install **Docker & Docker Compose**.
* Jalankan container (contoh: Portainer, Nextcloud, atau MySQL).

---

## 📌 Minggu 6 – Security, Backup, & Proyek Nyata

* Setting **SSH Key Authentication** (tanpa password login).
* Pelajari **Fail2Ban** untuk keamanan.
* Buat **backup otomatis** dengan `cron + rsync/tar`.
* Proyek mini:

  * Website pribadi (pakai Nginx + SSL Let’s Encrypt).
  * Nextcloud (cloud storage pribadi).
  * Git server kecil untuk latihan DevOps.

---

🎯 Setelah 6 minggu, kamu sudah pegang dasar server dan bisa berkembang ke:

* **DevOps** (CI/CD, Kubernetes, Ansible)
* **Cloud** (AWS, GCP, Azure)
* **Network & Security** lebih lanjut

---

Mau saya bikinkan juga **checklist mingguan** (berisi tugas-tugas kecil yang bisa kamu centang setiap selesai), biar belajarnya lebih rapi kayak roadmap to-do list?

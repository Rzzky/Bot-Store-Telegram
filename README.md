# 🤖 Bot-Store-Telegram 🛒

Bot Telegram untuk Pesanan Otomatis (Auto Order).

> **Pemberitahuan:** BOT MASIH DALAM TAHAP PENGEMBANGAN, BELUM RILIS SEPENUHNYA. AKAN DIUPDATE SECARA BERKALA (JIKA ADA WAKTU & MOOD).

Jika Anda memiliki kritik & saran, silakan hubungi saya di Telegram [@govtrashit](https://t.me/govtrashit).

---

## ✨ Fitur

### 👤 Fitur Pengguna
* **📋 List Produk:** Melihat daftar produk yang tersedia beserta harganya.
* **📦 Cek Stok:** Memeriksa jumlah stok terkini untuk semua produk.
* **🛒 Pesan Produk:** Memilih produk dan jumlah yang ingin dibeli.
* **💰 Sistem Saldo:** Setiap pengguna memiliki saldo pribadi yang dapat digunakan untuk pembelian dan dapat melakukan deposit.
* **📖 Riwayat Pembelian:** Bot mencatat semua riwayat transaksi pengguna (deposit dan pembelian).
* **🚚 Pengiriman Otomatis:** Detail akun yang dibeli akan dikirimkan secara otomatis kepada pengguna dalam bentuk file `.txt` setelah pembelian berhasil.

### 🛠️ Fitur Admin
* **👑 Panel Admin:** Panel khusus untuk pemilik bot guna mengelola semua aktivitas.
* **📊 Lihat Data Pengguna:** Admin dapat melihat informasi saldo semua pengguna.
* **✅ Konfirmasi Deposit:** Admin dapat melihat dan mengonfirmasi permintaan deposit yang tertunda. Saldo pengguna akan diperbarui secara otomatis setelah konfirmasi.
* **📈 Statistik Transaksi:** Bot melacak jumlah transaksi dan total nominal belanja untuk setiap pengguna.

---

## ⚙️ Cara Kerja

1.  **▶️ Mulai:** Pengguna memulai bot dan akan disambut dengan menu utama yang menampilkan saldo dan riwayat transaksi mereka.
2.  **👀 Lihat Produk:** Pengguna dapat melihat daftar produk atau memeriksa ketersediaan stok.
3.  **💸 Pembelian:** Untuk membeli, pengguna memilih produk. Jika saldo mencukupi, transaksi akan diproses.
4.  **💳 Transaksi:** Biaya produk akan dipotong dari saldo pengguna, stok produk diperbarui, dan transaksi dicatat.
5.  **📦 Pengiriman:** Detail akun yang telah dibeli dikirimkan kepada pengguna dalam bentuk file teks.
6.  **➕ Deposit:** Jika saldo tidak mencukupi, pengguna dapat melakukan deposit. Setelah mentransfer dana, pengguna mengirimkan bukti pembayaran ke bot, dan admin akan menerima notifikasi untuk konfirmasi.

---

## 📂 Struktur File

Repositori ini menggunakan beberapa file `.json` untuk menyimpan data:

* `produk.json`: Berisi daftar produk, termasuk nama, stok, harga, dan detail akun yang tersedia.
* `saldo.json`: Menyimpan informasi saldo terkini untuk setiap ID pengguna.
* `pending_deposit.json`: Menyimpan data deposit yang sedang menunggu konfirmasi dari admin.
* `riwayat.json`: Catatan riwayat semua transaksi (deposit dan pembelian) untuk setiap pengguna.
* `statistik.json`: Berisi statistik jumlah transaksi dan total pengeluaran untuk setiap pengguna.

---

## 🚀 Pengaturan

1.  **Clone repositori ini:**
    ```bash
    git clone https://github.com/rzzky/Bot-Store-Telegram
    ```
2.  **Instal dependensi yang diperlukan:**
    ```bash
    pip install python-telegram-bot
    ```
3.  **Konfigurasi bot:**
    * Buka file `main.py`.
    * Ganti `"CHANGE_THIS_TO_YOUR_TOKEN"` dengan Token Bot Telegram Anda.
    * Atur ID pengguna Anda sebagai `OWNER_ID` untuk mendapatkan akses ke panel admin.
4.  **Jalankan bot:**
    ```bash
    python main.py
    ```

---

## 👨‍💻 Penulis

* **RzkyO**
    * **Telegram:** [@govtrashit](https://t.me/govtrashit)
    * **GitHub:** [@rzzky](https://github.com/rzzky)
    * **Instagram:** [@rizzkyo](https://instagram.com/rizzkyo)

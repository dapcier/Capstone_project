# Capstone_project
Berikut draf teks lengkap untuk file **`README.md`** yang berisi penjelasan alur kerja (*workflow*) kolaborasi dan panduan perintah-perintah dasar Git.
Teks ini dirancang agar kamu dan temanmu memiliki acuan yang sama saat bekerja dalam satu repositori.

### Teks Salin-Tempel untuk `README.md`
```markdown
# 🚀 Capstone Project - Collaboration & Git Guide
Dokumen ini berisi panduan alur kerja kolaborasi dan referensi perintah dasar Git untuk pengembangan proyek **Capstone_project** (Frontend React & Backend Node.js).
---
## 🔄 Alur Kerja Harian (Daily Workflow)
Untuk menghindari bentrokan kode (*merge conflict*), selalu ikuti alur kerja berikut setiap kali mulai dan selesai koding:
### 1. Sebelum Mulai Koding
Selalu ambil pembaruan kode terbaru dari repositori GitHub agar komputermu tidak tertinggal:
```bash
git pull origin main
```
### 2. Setelah Selesai Koding / Menambah Fitur
Kirimkan perubahan yang sudah kamu buat ke GitHub:
```bash
# Cek status file yang diubah
git status
# Tambahkan seluruh file yang diubah ke staging area
git add .
# Simpan perubahan dengan pesan commit yang jelas
git commit -m "feat: menambah fitur login backend"
# Push kode ke branch utama GitHub
git push origin main
```
---
## 🛠️ Cheat Sheet Perintah Git
### 📥 1. Mengambil Kode (Pull & Clone)
* **Clone repositori pertama kali ke komputer:**
```bash
git clone [https://github.com/dapcier/Capstone_project.git](https://github.com/dapcier/Capstone_project.git) .

```

* **Mengambil perubahan terbaru dari GitHub:**
```bash
git pull origin main

```



---

### 📤 2. Menandai & Mengirim Perubahan (Add, Commit, Push)

* **Mengecek status perubahan file:**
```bash
git status

```


* **Menandai semua file yang diubah:**
```bash
git add .

```


* **Menandai file tertentu saja:**
```bash
git add path/ke/file.js

```


* **Membuat commit (catatan perubahan):**
```bash
git commit -m "Deskripsi ringkas perubahan kamu"

```


* **Mengunggah commit ke GitHub:**
```bash
git push origin main

```



---

### ⏪ 3. Pembatalan Perubahan (Undo)

* **Membatalkan `git add` (membatalkan staging file):**
```bash
git restore --staged nama_file.js

```


* **Mengembalikan file lokal ke kondisi commit terakhir (menghapus perubahan lokal):**
```bash
git restore nama_file.js

```


* **Membatalkan commit terakhir (file editan tetap tersimpan di lokal):**
```bash
git reset --soft HEAD~1

```


* **Membatalkan commit terakhir secara total (menghapus commit & perubahan file):**
```bash
git reset --hard HEAD~1

```



---

### 🗑️ 4. Menghapus File dari Tracking Git

* **Menghapus file dari komputer dan sistem Git:**
```bash
git rm nama_file.js
git commit -m "Remove nama_file.js"
git push origin main

```


* **Menghapus file dari GitHub saja (file tetap ada di komputer lokal):**
```bash
git rm --cached nama_file.js
git commit -m "Remove nama_file.js from repository"
git push origin main

```



---

## ⚠️ Aturan Penting Kredensial (.env)

* **DILARANG PUSH FILE `.env**`: File `.env` berisi kunci rahasia (database URI, JWT secret, API key) dan **tidak boleh** ter-upload ke GitHub.


* Gunakan file **`.env.example`** di folder `frontend` dan `backend` sebagai templat variabel tanpa menyertakan kredensial asli.

```

---

### Cara Mengubah File `README.md` di Komputer Kamu:

1. Buka folder `C:\Capstone_project` di laptopmu (bisa lewat VS Code atau Notepad)[cite: 10].
2. Buka file **`README.md`**, hapus teks lama, lalu salin dan tempel teks di atas[cite: 5].
3. Simpan file.
4. Jalankan perintah ini di Command Prompt / Git Bash folder proyekmu[cite: 10]:
   ```bash
   git add README.md
   git commit -m "docs: update README dengan panduan perintah Git"
   git push origin main

```

## **Melakukan Remote Operations**

1. **Membuat Repository GitHub**
2. **Membuat Folder di Local**
3. **Buka Git Bash**
4. **Masuk ke Folder Local yang Dibuat**
   ```bash
   $ cd <lokasi-folder>
   ```
5. **Membuat repositori Git lokal**
   ```bash
   $ git init
   ```
6. **Menambahkan File atau Folder ke Staging Area**
   ```bash
   $ git add <"nama-file" atau "nama-folder" jika ingin add semua file dan folder gunakan tanda titik "."> git add -A
   ```
7. **Melihat Status File**
   ```bash
   $ git status
   ```
8. **Melakukan Commit**
   ```bash
   $ git commit -m "komentar"
   ```
9. **Melihat Branch yang Ada**
   ```bash
   $ git branch
   ```
10. **Menambahkan Remote Repository**
   ```bash
   $ git remote add <nama: sering menggunakan "origin"> <urlnamarepo>
   ```
11. **Menampilkan Informasi Tentang Remote Repository**
    ```bash
    $ git remote
    ```
    **Atau**
    ```bash
    $ git remote -v
    ```
12. **Melihat URL Remote yang Terhubung**
    ```bash
    $ git remote get-url origin
    ```
13. **Melakukan Push ke Remote Repository**
    ```bash
    $ git push origin main
    ```
14. **Jika Sudah Melakukan Commit dan Ingin Menambahkan Perubahan Lagi, Ulangi Langkah 5 hingga 12:**
    - Tambahkan file lagi dengan
       ```bash
       $ git add <"nama-file" atau "nama-folder" jika ingin add semua file dan folder gunakan tanda titik "."> git add -A
       ```
    - Commit dengan
       ```bash
       $ git status
       ```
    - Push dengan
       ```bash
       $ git push origin main
       ```
15. **Jika Perubahan Pada Repository Remote Dilakukan dan Anda Ingin Menariknya ke Local, Lakukan Git Pull**
    ```bash
    $ git pull origin main
    ```
16. **Menghapus Remote dari Repository Lokal, Lakukan git remove/re **
    ```bash
    $ git remote re <nama-remote>
    ```

---

## **Melakukan Clone**

1. **Melakukan Clone Repository**
   ```bash
   $ git clone <urlnamarepo>
   ```
   Jika ingin folder di local memiliki nama berbeda dengan nama repository:
   ```bash
   $ git clone <urlnamarepo> <namafolder>
   ```
2. **Menambahkan File atau Folder ke Staging Area Setelah Clone**
   ```bash
   $ git add <"nama-file" atau "nama-folder" jika ingin add semua file dan folder gunakan tanda titik "."> git add -A
   ```
3. **Melakukan Commit**
   ```bash
   $ git commit -m "komentar"
   ```
4. **Melakukan Push ke Remote Repository**
   ```bash
   $ git push origin main
   ```
5. **Jika Ada Perubahan pada Repository Remote dan Anda Ingin Mengikuti Perubahan Tersebut pada Local Clone:**
   - Melakukan fetch untuk menarik perubahan:
     ```bash
     $ git fetch origin
     ```
   - Melakukan reset untuk menyelaraskan local dengan remote:
     ```bash
     $ git reset --hard origin/main
     ```

---

## **Pentingnya Urutan**

- Pada *remote operations*, Anda akan melakukan perubahan dan push ke repository remote.
- Pada *clone operations*, Anda akan melakukan clone dari repository remote dan dapat melakukan pull, fetch, atau reset sesuai kebutuhan untuk mengupdate local repository agar sesuai dengan perubahan remote.

Urutan ini memastikan Anda bisa mengikuti proses git dengan baik dan tidak mengalami konflik atau kebingungannya.

---

Dengan format ini, instruksi menjadi lebih mudah dipahami dan terstruktur seperti panduan yang jelas, menggabungkan langkah-langkah praktis untuk setiap operasi yang diperlukan di Git.

Pasted markdown(1).md
File
belajar github. aku sudah sampai dengan membuat branch. trus aku harus apa lagi

Bagus. Setelah membuat branch tambah-catatan-sqli, tahap berikutnya adalah membuat file catatan SQL Injection di branch tersebut.

Jangan melakukan commit dulu. Kita selesaikan satu tahap ini dahulu.

Langkah 2 — Membuat file di branch
Di PowerShell, pastikan branch aktif:
git branch

Hasil yang benar:

  main
* tambah-catatan-sqli

Tanda * menunjukkan branch yang sedang aktif.

Buka repository di VS Code:
code .
Di panel kiri VS Code:
Klik ikon New Folder
Beri nama:
notes
Klik folder notes, lalu klik New File.

Beri nama:

sql-injection.md
Isi file tersebut dengan:
# SQL Injection

SQL injection terjadi ketika input pengguna dimasukkan ke query SQL secara tidak aman.

## Konsep yang Dipelajari

- Query SQL
- Boolean condition
- UNION
- Error-based SQL injection
- Blind SQL injection

## Catatan Keamanan

Latihan hanya dilakukan pada lab yang memberikan izin, seperti PortSwigger Academy.
Simpan dengan menekan:
Ctrl + S

Struktur foldernya seharusnya menjadi:

cybersecurity-learning-log
├── notes
│   └── sql-injection.md
└── README.md

Setelah berhasil, balas saja “sudah”. Setelah itu kita lanjut ke git status, lalu git add—satu per satu.

Setelah dijalankan, kirim hasil PowerShell-nya. Kita belum membuat pull request dahulu.

Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 20 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 558 bytes | 558.00 KiB/s, done.
Total 4 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'belajar-github' on GitHub by visiting:
remote:      
https://github.com/ajimulyo/Belajar_GitHub/pull/new/belajar-github
remote:
To 
ajimulyo/Belajar_GitHub.git
 * [new branch]      belajar-github -> belajar-github
branch 'belajar-github' set up to track 'origin/belajar-github'.

Push berhasil sempurna. ✅

Artinya:

Branch belajar-github sudah dikirim ke GitHub.
Commit 6976afb sudah tersimpan di GitHub.
Branch lokal sudah terhubung dengan origin/belajar-github.
Tautan yang ditampilkan GitHub adalah opsi untuk membuat Pull Request—belum perlu dibuka sekarang.

Sekarang cek kondisi repository lokal:

git status

Hasil yang diharapkan:

On branch belajar-github
Your branch is up to date with 'origin/belajar-github'.

nothing to commit, working tree clean

Jalankan perintah tersebut lalu kirimkan hasilnya. Setelah itu, kita lanjut melihat branch baru di website GitHub sebelum belajar membuat Pull Request.

On branch belajar-github
Your branch is up to date with 'origin/belajar-github'.

nothing to commit, working tree clean

Semuanya sudah benar dan tersinkron. ✅

Branch aktif: belajar-github
Branch lokal sama dengan branch di GitHub
Semua perubahan sudah di-commit
Tidak ada file yang belum disimpan oleh Git
Langkah berikutnya — Cek branch di GitHub

Buka repository ini di browser:

github.com/ajimulyo/Belajar_GitHub

Klik tombol pilihan branch yang biasanya bertuliskan main.
Pilih branch:
belajar-github
Buka folder:
notes
Pastikan file ini terlihat:
tambah_file_d_branch.md

Untuk saat ini jangan klik Compare & pull request dahulu. Setelah file tersebut ditemukan di GitHub, balas “sudah terlihat”.

Ya. Dengan posisi awal 2/100, target realistis dalam 14 hari adalah:

Memahami perbedaan Git dan GitHub.
Membuat repository sendiri.
Melakukan clone, add, commit, push, dan pull.
Menggunakan branch dan pull request.
Melihat riwayat serta membatalkan perubahan.
Membaca repository orang lain.
Mengambil repository n8n dan menjalankan n8n dengan Docker.

Kita akan memakai proyek sederhana:

Cybersecurity Learning Log — kumpulan catatan belajar SQL injection dan cybersecurity dalam file Markdown.

Tidak perlu bisa coding terlebih dahulu.

Pola belajar harian

Durasi ideal: 60–90 menit per hari.

Setiap sesi:

15 menit memahami konsep.
40–60 menit praktik.
10 menit mencatat perintah dan error.
Jangan lanjut jika hasil hari itu belum berhasil.
Minggu 1 — Git dan GitHub dasar
Hari 1 — Pemeriksaan alat
Target

Memastikan Git dan VS Code siap.

Praktik

Buka PowerShell:



git --version

Lalu:



code --version

Jika code tidak dikenali, VS Code tetap bisa dibuka manual.

Periksa identitas Git:



git config --global user.name
git config --global user.email

Jika masih kosong, isi:



git config --global user.name "Nama Anda"


git config --global user.email "email-yang-dipakai-di-github@example.com"

Atur nama branch utama:



git config --global init.defaultBranch main

Periksa hasilnya:



git config --global --list
Lulus jika
git --version menampilkan versi.
Nama dan email muncul.
Anda mempunyai akun GitHub.
Hari 2 — Mengenal GitHub tanpa terminal
Target

Memahami repository, branch, commit, dan pull request.

Praktik resmi

Buka:

GitHub Skills: Introduction to GitHub

Klik Start course atau Use this template, lalu ikuti instruksi GitHub.

Latihan ini akan mengajarkan:

Membuat branch.
Membuat atau mengubah file.
Melakukan commit.
Membuka pull request.
Melakukan merge.

Latihan resminya memang dirancang untuk pemula dan dapat diselesaikan kurang dari satu jam. Anda juga bisa membaca GitHub Hello World.

Lulus jika

Anda pernah membuat dan melakukan merge satu pull request.

Hari 3 — Membuat repository sendiri
Target

Membuat tempat penyimpanan catatan cybersecurity.

Praktik

Di GitHub:

Klik tanda + di kanan atas.
Pilih New repository.
Repository name:


cybersecurity-learning-log
Description:


Catatan perjalanan belajar cybersecurity dan web security.
Pilih Public.
Aktifkan Add a README file.
Klik Create repository.

Buka README.md, klik ikon pensil, lalu isi:



# Cybersecurity Learning Log

Repository ini berisi catatan perjalanan belajar cybersecurity saya.

## Materi

- Git dan GitHub
- Dasar SQL
- SQL injection
- PortSwigger Web Security Academy

## Tujuan

Mendokumentasikan latihan dan perkembangan belajar secara konsisten.

Klik Commit changes.

Lulus jika

Repository dapat dibuka melalui:



https://github.com/USERNAME-ANDA/cybersecurity-learning-log
Hari 4 — Memahami terminal dan folder
Target

Bisa berpindah folder menggunakan PowerShell.

Praktik

Buat folder khusus proyek:



cd C:\


mkdir GitHub


cd GitHub

Periksa posisi:



pwd

Lihat isinya:



dir

Buka folder melalui File Explorer:



explorer .

Tanda titik . berarti “folder saat ini”.

Lulus jika

Anda memiliki folder:



C:\GitHub
Hari 5 — Clone repository
Target

Menyalin repository GitHub ke komputer.

Di halaman repository Anda:

Klik tombol Code.
Pilih HTTPS.
Salin URL repository.

Contohnya:



https://github.com/USERNAME-ANDA/cybersecurity-learning-log.git

Di PowerShell:



cd C:\GitHub

Kemudian:



git clone https://github.com/USERNAME-ANDA/cybersecurity-learning-log.git

Masuk ke repository:



cd cybersecurity-learning-log

Periksa:



git status

Buka di VS Code:



code .
Maknanya


GitHub → git clone → salinan di komputer

Menurut dokumentasi GitHub, cloning membuat salinan lokal repository beserta data Git-nya. GitHub Docs: Cloning a repository.

Lulus jika

git status menampilkan kurang lebih:



On branch main
Your branch is up to date with 'origin/main'.
nothing to commit, working tree clean
Hari 6 — Perubahan dan commit pertama
Target

Mengubah file dan menyimpan snapshot perubahan.

Di VS Code, tambahkan pada README.md:



## Progress

- [x] Membuat akun GitHub
- [x] Membuat repository
- [x] Clone repository
- [ ] Mempelajari branch

Simpan dengan Ctrl + S.

Kembali ke PowerShell:



git status

Lihat perubahannya:



git diff

Masukkan file ke staging area:



git add README.md

Buat commit:



git commit -m "docs: tambahkan progress belajar"

Kirim ke GitHub:



git push
Alurnya


Ubah file → git add → git commit → git push → GitHub
Lulus jika

Perubahan muncul pada README.md di GitHub.

Hari 7 — Review Minggu 1

Tanpa melihat catatan, coba jalankan:



cd C:\GitHub\cybersecurity-learning-log
git status
git log --oneline
git remote -v

Pahami hasilnya:

PerintahFungsi	

git status	Melihat kondisi repository
git log --oneline	Melihat riwayat commit
git remote -v	Melihat hubungan dengan GitHub
git diff	Melihat perubahan file
git push	Mengirim commit ke GitHub
Tantangan

Tambahkan satu baris baru ke README, lalu lakukan sendiri:



git add README.md
git commit -m "docs: perbarui catatan minggu pertama"
git push
Minggu 2 — Workflow GitHub dan praktik n8n
Hari 8 — Membuat branch
Target

Melakukan perubahan tanpa langsung mengganggu main.

Periksa branch:



git branch

Buat branch baru:



git switch -c tambah-catatan-sqli

Periksa lagi:



git branch

Branch aktif ditandai dengan *:



  main
* tambah-catatan-sqli

Di VS Code, buat folder:



notes

Di dalamnya buat file:



sql-injection.md

Isi sederhana:



# SQL Injection

SQL injection terjadi ketika input pengguna dimasukkan ke query SQL secara tidak aman.

## Konsep yang Dipelajari

- Query SQL
- Boolean condition
- UNION
- Error-based SQL injection
- Blind SQL injection

## Catatan Keamanan

Latihan hanya dilakukan pada lab yang memberikan izin, seperti PortSwigger Academy.

Commit:



git add notes/sql-injection.md
git commit -m "docs: tambahkan catatan dasar SQL injection"
git push -u origin tambah-catatan-sqli
Lulus jika

Branch tambah-catatan-sqli muncul di GitHub.

Hari 9 — Pull request dan merge
Target

Memindahkan perubahan branch ke main melalui pull request.

Di GitHub:

Buka repository.
Klik Compare & pull request.
Pastikan:


base: main
compare: tambah-catatan-sqli
Judul:


Tambahkan catatan dasar SQL injection
Deskripsi:


Menambahkan ringkasan materi SQL injection dan batasan penggunaan untuk latihan legal.
Klik Create pull request.
Periksa tab Files changed.
Klik Merge pull request.
Klik Confirm merge.
Klik Delete branch.

Pull request adalah usulan untuk menggabungkan perubahan dari satu branch ke branch lain. GitHub Docs: Pull requests.

Lulus jika

File notes/sql-injection.md muncul di branch main.

Hari 10 — Menyinkronkan komputer

Setelah merge dilakukan di GitHub, komputer Anda belum otomatis mengetahuinya.

Kembali ke branch utama:



git switch main

Ambil perubahan terbaru:



git pull

Hapus branch lokal yang sudah selesai:



git branch -d tambah-catatan-sqli

Periksa:



git branch
git status
Lulus jika

Hanya branch main yang tersisa dan file SQL injection ada di komputer.

Hari 11 — Membatalkan kesalahan
Target

Tidak panik ketika salah mengubah file.

Ubah README.md, tetapi jangan commit. Tambahkan:



INI ADALAH KESALAHAN

Periksa:



git status
git diff

Batalkan perubahan:



git restore README.md

Periksa lagi:



git status

Hasilnya seharusnya:



nothing to commit, working tree clean
Konsep penting
KondisiPerintah	

Perubahan belum di-add	git restore nama-file
Sudah di-add, belum commit	git restore --staged nama-file
Melihat riwayat	git log --oneline

Untuk sekarang, jangan menggunakan git reset --hard.

Hari 12 — .gitignore dan keamanan
Target

Memahami file yang tidak boleh dikirim ke GitHub.

Buat file:



.gitignore

Isi:



.env
*.log
node_modules/
.vscode/

Buat juga .env.example:



API_KEY=masukkan_api_key_di_sini
DATABASE_URL=masukkan_database_url_di_sini

Commit:



git add .gitignore .env.example
git commit -m "chore: tambahkan aturan file yang diabaikan"
git push

Aturan utama:

Jangan pernah memasukkan password, API key, token GitHub, credential Wablas, atau credential Google ke repository.

.env.example hanya berisi nama variabel dan contoh kosong, bukan credential asli.

Hari 13 — Membaca repository n8n
Target

Menggunakan kemampuan Git pada proyek nyata.

Masuk ke folder utama:



cd C:\GitHub

Karena repository n8n sangat besar, gunakan clone dangkal:



git clone --depth 1 https://github.com/n8n-io/n8n.git

Masuk:



cd n8n

Periksa:



git status
git branch
git remote -v
git log -5 --oneline

Buka di VS Code:



code .

Pelajari file berikut tanpa mengubahnya:

README.md
CONTRIBUTING.md
LICENSE.md
package.json
Folder packages
Folder docker
Lulus jika

Anda mampu menjawab:

Siapa pemilik repository? n8n-io
Apa nama repository? n8n
Apa remote-nya? origin
Apa fungsi README?
Apa arti --depth 1? Mengambil versi terbaru tanpa seluruh riwayat lama.
Hari 14 — Menjalankan n8n
Target

Menjalankan aplikasi yang ditemukan melalui repository GitHub.

Pastikan Docker Desktop berstatus Engine running.

Buat penyimpanan:



docker volume create n8n_data

Jalankan n8n di background:



docker run -d --name n8n -p 5678:5678 -v n8n_data:/home/node/.n8n docker.n8n.io/n8nio/n8n

Periksa:



docker ps

Lihat log:



docker logs n8n

Buka browser:



http://localhost:5678

Untuk menghentikan:



docker stop n8n

Untuk menjalankannya kembali:



docker start n8n

Data tetap tersimpan dalam volume n8n_data.

Checklist kelulusan 14 hari

Setelah 14 hari, Anda harus dapat menjelaskan dan mempraktikkan:

Membuat repository.
Membuat dan mengedit Markdown.
git clone
git status
git diff
git add
git commit
git push
git pull
Membuat branch.
Membuat pull request.
Merge pull request.
Membatalkan perubahan dengan git restore.
Menggunakan .gitignore.
Membaca repository n8n.
Menjalankan n8n menggunakan Docker.

Catatan penting: pada akhir dua minggu, Anda sudah bisa menggunakan repository dan menjalankan n8n, tetapi belum ditargetkan mampu memodifikasi source code inti n8n. Itu tahap lanjutan karena n8n menggunakan TypeScript, Node.js, Vue, pnpm, dan struktur monorepo.

Sekarang kita mulai dari Hari 1 saja. Jalankan dan kirim hasil tiga perintah ini:



git --version
git config --global user.name
git config --global user.email

Jangan kirim password atau token apa pun.

Jika membantu, saya juga bisa menyiapkan “Latihan GitHub setiap hari” agar setiap sesi 14 hari ini tidak terlewat.

Close
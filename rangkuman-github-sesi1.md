Github
RANGKUMAN BELAJAR GITHUB SESI 1 — MINGGU 28 JUNI 2026 — DASAR GIT & GITHUB
[1] SETUP AWAL — CONFIG IDENTITAS

---

git config --global user.name "Yudistira"
git config --global user.email "emailkamu@gmail.com"

## -- Cukup dilakukan sekali aja di awal!

## [2] BIKIN REPOSITORY LOKAL

mkdir C:\belajar-github -- bikin folder baru
cd C:\belajar-github -- masuk ke folder
git init -- jadiin folder ini repo Git

-- Output: Initialized empty Git repository in C:/belajar-github/.git/
-- .git/ = folder tersembunyi, jangan dihapus!

---

## [3] BIKIN FILE DARI TERMINAL

echo "# Belajar GitHub" > README.md -- bikin file baru
echo "teks tambahan" >> README.md -- tambah isi file

-- > = tulis ke file (timpa isi lama)
-- >> = tambah ke file (isi lama tetap ada)

---

## [4] WORKFLOW DASAR — ADD, COMMIT, PUSH

git status -- cek kondisi file
git add README.md -- daftarin file ke Git
git commit -m "pesan perubahan" -- simpan checkpoint
git push -- upload ke GitHub

## -- Urutan ini SELALU sama setiap kali ada perubahan!

## [5] CEK HISTORY COMMIT

## git log --oneline -- lihat semua history commit

## [6] HAPUS FILE & PUSH

del README.md -- hapus file
git status -- cek status (merah)
git add README.md -- add perubahan
git commit -m "hapus README" -- commit
gitu push -- push ke GitHub

---

## [7] TIPS NULIS PESAN COMMIT

❌ Yang jelek:
git commit -m "update"
git commit -m "fix"
git commit -m "asd"

✅ Yang bagus:
git commit -m "tambah fitur login user"
git commit -m "fix bug di halaman dashboard"
git commit -m "update README - tambah dokumentasi"

## -- Pesan commit = catatan perubahan, makin jelas makin bagus!

## [8] PERBEDAAN PENTING

Hapus FILE = file ilang, history commit TETAP ADA
Hapus REPOSITORY = semua ilang, file + seluruh history commit

-- Git = time machine buat kode!
-- Selama repo ada, bisa balik ke versi manapun!

---

## [9] STATUS WARNA DI GIT STATUS

MERAH = Untracked / belum di add
HIJAU = Sudah di add, siap di commit

=======================
SESI 2 GITHUB (MINGGU DEPAN): Branch, Pull, Clone, Merge, .gitignore
=======================

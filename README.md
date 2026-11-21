# 🍎 Apple's Little World

Website persona punya Apple (Honey Fried Apple). Isinya buku, lagu, warna, karakter, cosplay, inspo, dan tulisan.

## Isi folder ini

| File | Gunanya |
|---|---|
| `index.html` | Tampilan dan semua fitur website. Jarang perlu diubah. |
| `content.json` | **Semua isi website**: lagu, buku, karakter, tulisan, dll. Ini yang berubah kalau kamu ngedit. |
| `images/` | Tempat foto-foto yang kamu upload lewat panel admin. |
| `README.md` | Panduan ini. |

---

## Langkah 0 — (Disarankan) Bikin akun GitHub khusus persona

Link GitHub Pages bentuknya `https://USERNAME.github.io`, dan halaman repo-nya nunjukin siapa pemiliknya. Kalau kamu pengen persona Apple nggak nyambung ke nama asli, bikin akun GitHub baru khusus buat Apple (misalnya `honeyfriedapple`), pakai email lain.

Nanti kalau udah punya domain sendiri, link-nya bisa diganti jadi domain itu.

## Langkah 1 — Bikin repository

1. Login ke GitHub, klik **+** di pojok kanan atas, lalu pilih **New repository**.
2. Isi **Repository name** dengan: `USERNAME.github.io`. Ganti USERNAME pakai username akun itu, persis sama.
3. Pilih **Public**.
4. Klik **Create repository**.

## Langkah 2 — Upload file

1. Di halaman repo yang baru, klik **uploading an existing file**. Bisa juga lewat **Add file**, lalu **Upload files**.
2. Drag & drop **semua isi folder ini**: `index.html`, `content.json`, `README.md`, dan folder `images`.
3. Klik **Commit changes** di bawah.

## Langkah 3 — Nyalain GitHub Pages

1. Di repo, buka tab **Settings**, lalu menu **Pages** di sebelah kiri.
2. Di bagian **Build and deployment**, isi **Source** dengan **Deploy from a branch**.
3. Pilih branch **main** dan folder **/ (root)**, lalu klik **Save**.
4. Tunggu 1–2 menit, terus refresh halaman itu. Link website kamu bakal muncul di atas 🎉

## Langkah 4 — Bikin "kunci" buat panel admin (token)

Token ini yang bikin tombol **Simpan** bisa langsung ngubah website kamu.

1. Klik foto profil di kanan atas, lalu pilih **Settings**.
2. Scroll ke paling bawah, klik **Developer settings**, terus **Personal access tokens**, terus **Fine-grained tokens**.
3. Klik **Generate new token**, lalu isi:
   - **Token name**: `apple-admin`
   - **Expiration**: terserah, misalnya 1 tahun. Kalau udah kadaluarsa, tinggal bikin lagi.
   - **Repository access**: pilih **Only select repositories**, terus pilih repo `USERNAME.github.io`.
   - **Permissions**: buka **Repository permissions**, cari **Contents**, ubah jadi **Read and write**.
4. Klik **Generate token**, terus **copy** token-nya. Token cuma ditampilin sekali.

> ⚠️ Token itu kayak password. **Jangan kirim ke siapa pun**, termasuk ke chat. Cukup kamu tempel sendiri di panel admin (langkah 5).

## Langkah 5 — Hubungkan panel admin

1. Buka website kamu dengan tambahan `#admin` di ujung link, contohnya `https://USERNAME.github.io/#admin`.
2. Klik **✏️ Edit** di kanan bawah, terus klik **🔑 Koneksi GitHub**.
3. Isi **Repo** dengan `USERNAME/USERNAME.github.io`, **Branch** dengan `main`, dan **Token** dengan token dari langkah 4.
4. Klik **Simpan & tes koneksi**. Kalau muncul ✅ berarti udah siap.

Ini cukup sekali di tiap laptop atau HP yang kamu pakai. Setelah itu tombol ✏️ Edit selalu muncul di browser itu. Pengunjung lain nggak bakal lihat tombol itu, dan kalaupun mereka buka `#admin`, mereka tetap nggak bisa nyimpen apa-apa tanpa token kamu.

## Cara update website (sehari-hari)

1. Buka website kamu, lalu klik **✏️ Edit**.
2. Ubah apa aja: tambah lagu, buku, karakter, tulisan, upload foto, ganti warna, sembunyiin bagian, dan lain-lain.
3. Klik **💾 Simpan**.
4. Tunggu ±1–2 menit, refresh, dan semua orang udah lihat versi baru ✨

**Bonus:** GitHub nyimpen semua versi lama. Kalau ada yang salah, kamu bisa balikin dari tab **Commits** di repo.

## Nanti: pakai domain sendiri

1. Beli domain, misalnya `.my.id` atau `.com`, di penyedia domain.
2. Di GitHub, buka **Settings**, lalu **Pages**, terus isi **Custom domain** dan klik **Save**.
3. Di penyedia domain, tambahin DNS record sesuai petunjuk GitHub.

Bagian ini nanti kita kerjain bareng ya 🍎

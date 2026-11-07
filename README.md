# Untukmu

Halaman satu file (`index.html`), siap di-deploy ke Vercel tanpa build.

## Isi folder

- `index.html` : halaman Untukmu (file asli Anda, tidak diubah)
- `vercel.json` : pengaturan Vercel
- `.gitignore` : file yang tidak ikut di-upload

## Upload ke GitHub

1. Buat repository baru di https://github.com/new (jangan centang "Add a README").
2. Di terminal, dari dalam folder ini:

```bash
git init
git add .
git commit -m "Commit pertama"
git branch -M main
git remote add origin https://github.com/USERNAME/NAMA-REPO.git
git push -u origin main
```

Tanpa terminal: di halaman repository klik **Add file > Upload files**, lalu seret semua isi folder ini.

## Deploy ke Vercel

1. Masuk ke https://vercel.com dengan akun GitHub.
2. **Add New > Project**, pilih repository tadi, klik **Import**.
3. Framework Preset: **Other**. Biarkan sisanya kosong.
4. Klik **Deploy**. Alamatnya akan berbentuk `nama-repo.vercel.app`.

Jika ingin mengubah isi, edit `index.html` lalu `git push`; Vercel memperbarui situs otomatis.

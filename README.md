# MyPortfolio

Website portofolio personal sederhana menggunakan HTML, CSS, dan JavaScript.

## Cara edit data

Ubah teks placeholder di `index.html`:

- `Nama Kamu`
- `NK`
- `Frontend Developer`
- `emailkamu@example.com`
- `https://github.com/username`
- `https://www.linkedin.com/in/username`
- Judul dan deskripsi proyek di bagian `projects`

## Cara melihat di komputer

Buka file `index.html` langsung di browser, atau jalankan server lokal:

```bash
node -e "const http=require('http'),fs=require('fs'),path=require('path');http.createServer((req,res)=>{const file=path.join(process.cwd(),req.url==='/'?'index.html':req.url);fs.readFile(file,(err,data)=>{if(err){res.writeHead(404);return res.end('Not found')}res.end(data)})}).listen(5500)"
```

Lalu buka:

```text
http://localhost:5500
```

## Cara upload ke GitHub

1. Buat repository baru di GitHub, misalnya `myportfolio`.
2. Jalankan perintah berikut dari folder project:

```bash
git init
git add .
git commit -m "Initial portfolio website"
git branch -M main
git remote add origin https://github.com/username/myportfolio.git
git push -u origin main
```

3. Buka repository di GitHub.
4. Masuk ke `Settings` > `Pages`.
5. Pada `Build and deployment`, pilih `Deploy from a branch`.
6. Pilih branch `main` dan folder `/root`, lalu klik `Save`.

Setelah aktif, website biasanya tersedia di:

```text
https://username.github.io/myportfolio/
```

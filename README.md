# Panduan Meningkatkan Literasi AI (LaTeX)

Repo ini menyimpan sumber naskah LaTeX untuk ebook/panduan literasi AI.

## Kenapa `main.pdf` tidak kena warning biner di PR?
`main.pdf` disimpan menggunakan **Git LFS** agar PR tetap ringan dan tidak memunculkan warning diff biner biasa.

## Cara kompilasi PDF

Sebelum pull, pastikan Git LFS aktif:

```bash
git lfs install
```

Jalankan perintah berikut di root repo:

```bash
pdflatex -interaction=nonstopmode main.tex
pdflatex -interaction=nonstopmode main.tex
```

Output akan terbentuk sebagai:

- `main.pdf`

## File sementara yang diabaikan
Artefak build LaTeX sementara (seperti `.aux`, `.log`, `.out`, `.toc`) diabaikan oleh `.gitignore`. File `main.pdf` tetap disimpan, tetapi melalui Git LFS.

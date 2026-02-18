# Panduan Meningkatkan Literasi AI (LaTeX)

Repo ini menyimpan sumber naskah LaTeX untuk ebook/panduan literasi AI.

## Kenapa `main.pdf` tidak disimpan di Git?
GitHub PR sering memberi peringatan untuk file biner (seperti PDF) karena tidak bisa ditinjau inline seperti teks. Agar review PR tetap rapi, repo ini hanya menyimpan sumber teks (`main.tex`).

## Cara kompilasi PDF
Jalankan perintah berikut di root repo:

```bash
pdflatex -interaction=nonstopmode main.tex
pdflatex -interaction=nonstopmode main.tex
```

Output akan terbentuk sebagai:

- `main.pdf`

## File sementara yang diabaikan
Artefak build LaTeX (seperti `.aux`, `.log`, `.out`, `.toc`) serta `main.pdf` diabaikan oleh `.gitignore`.

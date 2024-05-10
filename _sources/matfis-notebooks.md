---
jupytext:
  formats: md:myst
  text_representation:
    extension: .md
    format_name: myst
    format_version: 0.13
    jupytext_version: 1.11.5
kernelspec:
  display_name: Python 3
  language: python
  name: python3
---

# Matfis-Notebooks (_MyST Markdown_)

Jupyter Book juga memungkinkan kita untuk menyusun sebuah notebook yang berbasis teks dengan memanfaatkan _MyST Markdown_.
Lihat [Dokumentasi Notebook dengan _MyST Markdown_](https://jupyterbook.org/file-types/myst-notebooks.html) untuk intruksi yang lebih terperinci.

Berikut ini menunjukkan halaman yang ditulis dengan memanfaatkan _MyST Markdown_.

## Sebuah Sel Contoh

Dengan _MyST Markdown_, kita dapat mendefinisikan "code cells" sebagai berikut:

```{code-cell}
print(2 + 2)
```
Ketika buku kita dibangun (melalui perintah "_jb build <nama buku kita>_")
konten yang mengandung blok `{code-cell}` akan dieksekusi dengan  "_Jupyter Kernel_", dan  outputnya akan ditayangkan bersama-sama dengan konten lainnya.


```{seealso}
Jupyter Book menggunakan [Jupytext](https://jupytext.readthedocs.io/en/latest/) untuk mengkonversi file yang berbasis teks menjadi notebook, dan dapat mendukung [banyak notebook berbasis teks](https://jupyterbook.org/file-types/jupytext.html).
```

## Membuat Notebook dengan _MyST Markdown_

Notebook _MyST Markdown_ didefinisikan melalui dua hal:

1. Metadata YAML yang diperlukan untuk memahami/ bagaimana file teks dikonversi menjadi notebook (termasuk informasi tentang kernel yang diperlukan).
   Lihat YAML di atas sebagai contoh.
2. Keberadaan direktif  `{code-cell}` yang akan dieksekusi dengan buku Anda.

Itulah yang semua kita perlukan untuk memulai!

## Menambah _Metadata YAML_ untuk  _Notebook MyST_

Jika Anda mempunyai file markdown dan kita menginginkan secara cepat menambahkan metadata YAML pada file tersebut, sehingga Jupyter Book memberlakukannya sebagai sebuah Notebook MyST Markdown, jalankan perintah berikut:

```
jupyter-book myst init path/to/markdownfile.md
```

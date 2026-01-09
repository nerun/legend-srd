# Procedures and Tools

> DEPRECATED: All this work was done. Working on revision now.

On Linux:

1. Extract chapter or pages:

``` console
$ pdftk infile.pdf cat 12-15 output outfile.pdf
```

2. Convert to TXT or directly to MD:

```console
$ pdftotext outfile.pdf outfile.txt
```

&nbsp;&nbsp;&nbsp;&nbsp;A good python alternative with better results:

```console
$ pdf2txt.py outfile.pdf > outfile.txt
```

&nbsp;&nbsp;&nbsp;&nbsp;Convert PDF directly to MD: [PDF to Markdown Converter](https://pdf2md.morethan.io) (source in [GitHub](https://github.com/jzillmann/pdf-to-markdown)). Very good, recommended.

3. In both cases, fix broken paragraphs: [paragrapher](https://gist.github.com/nerun/8318924aa35f3f27231f86468804cc8c).

4. Copy txt inside the right chapter:

```console
echo "" >> chapter.md
cat outfile.txt >> chapter.md
```

5. Edit with [Ghostwriter](https://ghostwriter.kde.org) or other editor.

## Docs and Guides

- CONE, Matt. [Basic Syntax](https://www.markdownguide.org/basic-syntax). *Makdown Guide*.
- GitHub Docs. [Writing on GitHub](https://docs.github.com/en/get-started/writing-on-github). _GitHub.com_.
- PRITCHARD, Adam. [Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet). _GitHub: markdown-here_.

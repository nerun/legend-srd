# Procedures and Tools

> DEPRECATED: All this work was done. Working on revision now.

On Linux:

1. Extract chapter or pages:

		pdftk infile.pdf cat 12-15 output outfile.pdf

2. Convert to TXT or directly to MD:

		pdftotext outfile.pdf outfile.txt

	A good python alternative with better results:

		pdf2txt.py outfile.pdf > outfile.txt

	Convert PDF directly to MD: [PDF to Markdown Converter](https://pdf2md.morethan.io) (source in [GitHub](https://github.com/jzillmann/pdf-to-markdown)). Very good, recommended.

3. In both cases, fix broken paragraphs: [paragrapher](https://gist.github.com/nerun/8318924aa35f3f27231f86468804cc8c).

4. Copy txt inside the right chapter:

		echo "" >> chapter.md
		cat outfile.txt >> chapter.md

5. Edit with [Ghostwriter](https://ghostwriter.kde.org) or other editor.
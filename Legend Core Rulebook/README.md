# Legend Core Rulebook

This project aims to convert to markdown the PDF version of [Legend Core Rulebook](https://www.mongoosepublishing.com/products/legend-core-rulebook?variant=42088757854455) published by _Mongoose Publishing_ in 2011. Here you can follow the progress of this work.

## Convertion to markdown progress

| Chapter                         | Pgs. | Conv.|    %  |
|---------------------------------|:----:|:----:|------:|
| ~~1 Welcome to Legend~~         |   2  |   2  | 100.0 |
|   2 Adventurer Creation         |  33  |   0  |     0 |
|   3 Skills                      |  28  |   0  |     0 |
|   4 Game System                 |  28  |   0  |     0 |
|   5 Equipment                   |  27  |   0  |     0 |
|   6 Combat                      |  32  |   0  |     0 |
| ~~7 Magic~~                     |   3  |   3  | 100.0 |
|   8 Common Magic                |  15  |   0  |     0 |
|   9 Divine Magic                |  19  |   0  |     0 |
|  10 Sorcery                     |  19  |   0  |     0 |
|~~11 Guilds, Factions and Cults~~|   9  |   9  | 100.0 |
|~~12 Heroic Ablities~~           |   7  |   7  | 100.0 |
|  13 Gamemastering Legend        |  14  |   0  |     0 |
|~~14 License~~                   |   2  |   2  | 100.0 |
|                         TOTAL   | 238  |  23  |   9.7 |

## Procedures and Tools

On Linux:

1. Extract chapter or pages:

		pdftk infile.pdf cat 12-15 output outfile_p12-15.pdf

2. Convert to text:

		pdftotext outfile_p12-15.pdf outfile_p12-15.txt
		
	A good alternative:
		
		pdf2txt.py outfile_p12-15.pdf

3. Copy txt inside the right chapter:

		echo >> num\ chapter.md
		cat outfile_p12-15.txt >> num\ chapter.md

4. Edit with Ghostwriter.

Better alternative: [PDF to Markdown Converter](https://pdf2md.morethan.io) (source in [GitHub](https://github.com/jzillmann/pdf-to-markdown)).

To fix broken paragraphs: [paragrapher](https://gist.github.com/nerun/8318924aa35f3f27231f86468804cc8c).
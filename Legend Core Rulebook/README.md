# Legend Core Rulebook

This project aims to convert to markdown the PDF version of [Legend Core Rulebook](https://www.mongoosepublishing.com/products/legend-core-rulebook?variant=42088757854455) published by _Mongoose Publishing_ in 2011. Here you can follow the progress of this work.

## Convertion to markdown progress

| #   Chapter                    | Pgs. | Conv.|    %  |
|--------------------------------|:----:|:----:|------:|
| ~~1 Welcome to Legend~~        |   2  |   2  | 100.0 |
|   2 Adventurer Creation        |  33  |   0  |     0 |
|   3 Skills                     |  28  |   0  |     0 |
|   4 Game System                |  28  |   0  |     0 |
|   5 Equipment                  |  27  |   0  |     0 |
|   6 Combat                     |  32  |   0  |     0 |
| ~~7 Magic~~                    |   3  |   3  | 100.0 |
|   8 Common Magic               |  15  |   0  |     0 |
|   9 Divine Magic               |  19  |   0  |     0 |
|  10 Sorcery                    |  19  |   0  |     0 |
|  11 Guilds, Factions and Cults |   9  |   0  |     0 |
|~~12 Heroic Ablities~~          |   7  |   7  | 100.0 |
|  13 Gamemastering Legend       |  14  |   0  |     0 |
|~~14 License~~                  |   2  |   2  | 100.0 |
|     TOTAL                      | 238  |  14  |   5.9 |

## Procedure

On Linux:

1. Extract chapter or pages:

		pdftk infile.pdf cat 12-15 output outfile_p12-15.pdf

2. Use the command:

		pdftotext outfile_p12-15.pdf outfile_p12-15.txt

3. Rename file to "outfile_p12-15.md" and edit it in Ghostwriter, for example.
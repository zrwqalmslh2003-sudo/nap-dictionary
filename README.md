# nap-dictionary

Word dictionary for the Arabic game "اسم حيوان نبات جماد بلاد".

Each CSV file contains words starting with one Arabic letter.
Format: `word,category` where category ∈ {name, animal, plant, object, country}.

## Files

28 files, one per Arabic letter:

| # | File | Letter |
|---|------|--------|
| 01 | 01-alef.csv | ا |
| 02 | 02-beh.csv | ب |
| 03 | 03-teh.csv | ت |
| 04 | 04-theh.csv | ث |
| 05 | 05-jeem.csv | ج |
| 06 | 06-hah.csv | ح |
| 07 | 07-khah.csv | خ |
| 08 | 08-dal.csv | د |
| 09 | 09-dhal.csv | ذ |
| 10 | 10-reh.csv | ر |
| 11 | 11-zain.csv | ز |
| 12 | 12-seen.csv | س |
| 13 | 13-sheen.csv | ش |
| 14 | 14-sad.csv | ص |
| 15 | 15-dad.csv | ض |
| 16 | 16-tah.csv | ط |
| 17 | 17-zah.csv | ظ |
| 18 | 18-ain.csv | ع |
| 19 | 19-ghain.csv | غ |
| 20 | 20-feh.csv | ف |
| 21 | 21-qaf.csv | ق |
| 22 | 22-kaf.csv | ك |
| 23 | 23-lam.csv | ل |
| 24 | 24-meem.csv | م |
| 25 | 25-noon.csv | ن |
| 26 | 26-heh.csv | ه |
| 27 | 27-waw.csv | و |
| 28 | 28-yeh.csv | ي |

## CSV format

Two columns, no header, UTF-8:

```csv
سمك,animal
سيارة,object
سوريا,country
سامي,name
سمسم,plant
```

Categories (exact strings): `name`, `animal`, `plant`, `object`, `country`.

## Notes

- Words are normalized before matching (hamza forms → ا, ة → ه, ى → ي, diacritics removed).
- Files can be empty during the initial phase; the game handles empty files by falling back to first-letter validation.

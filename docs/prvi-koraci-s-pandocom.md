# Prvi koraci s Pandocom

Citatelj ce nauciti koristiti Pandoc za pretvorbu filetypea. Ucenje traje do 30 minuta.

Provjereno s Pandocom 3.13 na Windows 11 Pro, i GNU bash, version 5.3.15.

## Prije početka

Citatelju je potrebno:
- VSCode
- GitBash
- korisnicki racun i repozitorij na GitHubu
- README.md datoteka.

## 1. Instalirajte Pandoc

### Windows

[Posjetite link za skidanje Pandoca.](https://github.com/jgm/pandoc/releases/latest) Nakon sto ste preuzeli Pandoc, instalirajte ga na Vase racunalo. Nakon instalacije, ponovno pokrenite VSCode. 

### macOS

[Koraci za macOS. Ako nemate Mac, ostavite odjeljak za kolegu iz dijela D.]

## 2. Provjerite instalaciju

Unesite slijedecu naredbu kako biste provjerili status instalacije.

```bash
pandoc --version
```

**Očekivani rezultat:** Ukoliko je instalacija bila uspjesna, trebali biste vidjeti blok teksta koji pocinje sa "pandoc 3.13" u prvoj liniji.

## 3. Pretvorite Markdown u Word

Da pretvorite odredjenu .md datoteku u .docx datoteku za rad u Wordu, unesite slijedecu komandu u shell:
```
pandoc odredjena-datoteka.md -o odredjena.datoteka.docx
```

## 4. Pretvorite Markdown u web-stranicu

Da pretvorite odredjenu .md datoteku u ..html datoteku, unesite slijedecu komandu:
```
pandoc odredjena-datoteka.md -s -o odredjena.datoteka.html
```
Argument -s sluzi da bi kreirao .html kao standalone datoteka sa svim metapodatcima.


## Ako ne radi

| Poruka | Što znači | Što učiniti |
|---|---|---|
| `command not found` | Pandoc nije instaliran | Ponovno odraditi instalaciju Pandoca |

## Što ste napravili

Sada ste upuceni u proces skidanja i instalacije programa Pandoc. Pandoc sluzi pretvorbi raznih tekstualnih podataka u druge formate od pocetnog. Proces pretvorbe je opisan u ovom tutorialu. Sada imate potrebne informacije za neke od pretvorbi.
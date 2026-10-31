# Prvi koraci u terminalu

<!-- Ovo je početna verzija (v0) za projekt P1.
     Sve što je u [uglatim zagradama] zamijenite svojim tekstom.
     Očekivane rezultate prepišite sa SVOJEG zaslona, ne izmišljajte ih.
     Kad završite, ovaj komentar izbrišite. -->

[Jedna ili dvije rečenice: što će čitatelj naučiti u ovom tutorialu i koliko otprilike traje.]

## Prije početka

- Rad se izvodi na sustavu Windows 11 Pro, i GNU bash, version 5.3.15.
- Visual Studio Code je pokrenut, a u njemu je otvorena mapa /atp-prirucnik.

## 1. Otvorite terminal

U izborniku **Terminal** odaberite **New Terminal**.

**Očekivani rezultat:**   
$ 
## 2. Provjerite gdje se nalazite

```bash
pwd
```

**Očekivani rezultat:**   
/c/Users/Korisnik/Documents/zagrijavanje/atp-prirucnik

## 3. Napravite mapu i uđite u nju

```bash
mkdir proba-terminala
cd proba-terminala
pwd
```

**Očekivani rezultat:**   
/c/Users/Korisnik/Documents/zagrijavanje/atp-prirucnik/proba-terminala

## 4. Napravite datoteku i upišite u nju tekst

```bash
echo "# Moje biljeske" > biljeske.md
cat biljeske.md
```

**Očekivani rezultat:**   
\# Moje biljeske

## 5. Dodajte još jedan redak

```bash
echo "- Naredba pwd ispisuje gdje se nalazim." >> biljeske.md
cat biljeske.md
```

**Očekivani rezultat:**   
\# Moje biljeske  
\- Naredba pwd ispisuje gdje se nalazim.

Koristenje jednog znaka '>' brise sve postojece unose i ostavlja samo unos u komandi, a koristenje dva znaka, odnosno '>>', dodaje unos u novi redak na kraju teksta.

## 6. Kopirajte, preimenujte i izbrišite datoteku

```bash
cp biljeske.md kopija.md
mv kopija.md stara.md
rm stara.md
ls
```

**Očekivani rezultat:**  
biljeske.md

Prije koristenja naredbe 'rm' korisnik mora biti potpuno siguran u namjeru, jer tako obrisana datoteka ne moze biti povracena.

## Ako ne radi

| Poruka | Što znači | Što učiniti |
|---|---|---|
| `No such file or directory` | Objekt komande ne postoji u radnoj mapi | Kreirati objekt sa komandama mkdir ili touch |
| File exists | Istoimena datoteka ili mapa postoji | Promijeniti zeljeno ime nove mape ili datoteke, ili preimenovati postojecu |

## Što dalje

Za vise komandi i detaljnije upute, referirati se na priručnik Srca *Uvod u Linux*, poglavlja 2 i 3.

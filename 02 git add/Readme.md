# Cvičení git add

> Pracujte se svým veřejným repozitářem.

## Cvičení 1

1. Vytvořte nový soubor Merkur.txt v projektu.
2. Použijte příkaz git add na přidání souboru do stage area.
3. Ověřte pomocí příkazu git status, že se soubor úspěšně přidal.

### Řešení 1

```bash
(vytvoreni souboru v projektu)
git status
git add "02 git add/Merkur.txt"
git status
```

## Cvičení 2

1. Vytvořte 3 nové soubory Venuše.txt, Země.txt, Mars.txt v projektu.
2. Přidejte změny provedené ve všech souborech do indexu naráz.

### Řešení 2

```bash
(vytvoreni novych souboru v projektu)
git status
git add --all "02 git add/"	
git status
```

## Cvičení 3

1. Vytvořte 2 nové soubory Jupiter.txt, Saturn.txt v projektu.
2. Přidejte změny provedené pouze v souboru Jupiter.txt do indexu.
3. Smažte soubor Saturn.txt a podívejte se, co na to git.

### Řešení 3

```bash
(vytvoreni souboru v projektu)
git add "02 git add/Jupiter.txt"
git status
(po smazani nezaindexovaneho souboru Saturn.txt git tento soubor vůbec nedetekuje)
```

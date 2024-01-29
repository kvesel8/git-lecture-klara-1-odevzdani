# git pull

Pracujte se repozitářem ze cvičení `git merge`.

## Cvičení 1

1. Stáhněte si nejnovější verzi projektu ze vzdáleného repozitáře.

### Řešení 1

```bash
 git pull upstream main
```

## Cvičení 2

1. Vytvořte si nový prázdný adresář s názvem „Klient 2“.
2. Do tohoto adresáře si naklonujte svůj vzdálený repozitář, který jste použili v cvičení `git merge`.
3. V hlavní větvi přidejte nový soubor Ganymed.txt.
4. Komitněte změny.
5. Dostaňte tyto změny do vzdáleného repozitáře.
6. Vraťte se do původního adresáře, který jste používali během cvičení `git merge`
7. Stáhněte si změny ze vzdáleného repozitáře.
8. Zkontrolujte si, zda jsou změny ze složky „Klient 2“ přítomny i v původním adresáři.

### Řešení 2

```bash
 (vytvoreni noveho adresare s nazvem Klient 2)
 git clone https://github.com/kvesel8/git-lecture-klara-1-odevzdani
 (vytvoreni souboru Ganymed.txt na hlavni větvi)
 git add "07 git pull/Ganymed.txt"
 git commit -m "pridani souboru Ganymed.txt"
 git push
 git pull upstream main
 (v původním adresáři jsou přítomny změny ze složky Klient 2) 
```

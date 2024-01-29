# Cvičení git push

## Cvičení 1

1. Nahrajte své změny z cvičení git branch & git checkout do vzdáleného repozitáře na GitHubu.
2. Zkontrolujte, že na webu vidíte všechny větve.

### Řešení 1

```bash
 git config --global --add safe.directory "C:\Users\User\GITkurz\git-lecture-klara-1"
 git remote add upstream https://github.com/kvesel8/git-lecture-klara-1-odevzdani
 git push upstream main
 git push upstream test-branch
 git push upstream feature/europa-file
 git push upstream feature/test-branch
 git push upstream feature/bug-fix
```

## Cvičení 2

1. Přepněte se na hlavní větev.
2. Vytvořte novou větev s názvem „feature/bug-fix“.
3. Upravte soubor Jupiter.txt a připište do něj řádek „Bug fix Jupiter file“.
4. Dostaňte tuto změnu do vzdáleného repozitáře na GitHubu.

### Řešení 2

```bash
  git branch feature/bug-fix 
  (pridani textu „Bug fix Jupiter file“ do Jupiter.txt)
  git add "02 git add/Jupiter.txt"
  git commit -m "Bug fix Jupiter file"
  git push upstream main 
```

## Cvičení 3

1. Na hlavní větvi změňte skrze webové rozhraní GitHubu soubor Země.txt. Připište nový řádek „Update Earth file“.
2. Proveďte komit změny.
3. Na hlavní větvi v lokálním repozitáři, upravte soubor Uran.txt a připište do něj nový řádek „Update Uran file“.
4. Proveďte komit této změny.
5. Nyní tuto změnu dostaňte na vzdálený repozitář na GitHubu.

### Řešení 3

```bash
  (uprava souboru Zeme.txt na githubu)
  (komit)
  (uprava souboru Uran.txt v lokalnim repository)
  git add "03 git commit/Uran.txt"
  git commit "03 git commit/Uran.txt"
  git push upstream main
  (zobrazeni zpravy  'git pull' before pushing again.)
  git pull upstream main
  git push upstream main 
```

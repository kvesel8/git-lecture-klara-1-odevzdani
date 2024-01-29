# Cvičení git merge

## Cvičení 1

1. Vypište všechny větve.
2. Postupně všechny větve slučte do hlavní větve.
3. Dostaňte tyto změny do vzdáleného repositáře.
4. Na GitHubu si zobrazte komity v hlavní větvi. Všimněte si, jak vypadá historie hlavní větve.
5. Smažte všechny sloučené větve.

### Řešení 1

```bash
 git branch
 git checkout main
 git merge test-branch
 git merge feature/test-branch
 git merge feature/europa-file
 git merge feature/bug-fix
 git push upstream main
 (smazani sloučených větví)
 
```

## Cvičení 2

1. Vytvořte novou větev „feature/new-moon-files“ z hlavní větve a přepněte se do ní.
2. Postupně vytvořte nový soubor s názvem Charon.txt, komitněte tuto změnu, nový soubor Měsíc.txt a komitněte.
3. Připište nový řádek „New Pluto moon“ do souboru Charon.txt a komitněte změnu.
4. Připište nový řádek „New Earth moon“ do souboru Měsíc.txt a komitněte změnu.
5. Slučte tyto změny do hlavní větve tak, aby vznik pouze jeden jediný komit v hlavní větvi.
6. Smažte větev „feature/new-moon-files“.

### Řešení 2

```bash
 git branch feature/new-moon-files
 git checkout feature/new-moon-files
 (vytvoreni souboru Charon.txt a Mesic.txt)
 git add --all "06 git merge"
 git commit -m "pridani souboru Mesic a Charon"
 git add "06 git merge/Charon.txt"
 git commit -m "pridani textu do Charon.txt"
 git add "06 git merge/Mesic.txt"
 git commit -m "pridani textu do Mesic.txt"
 git checkout main
 git merge --squash feature/new-moon-files
 git commit -m "slouceni vsech zmen do jednoho komitu z vetve feature/new-moon-files"
 git branch -D feature/new-moon-files
```

# Cvičení git nastaveni

## Cvičení 1

1. Nastavte si své jméno a e-mail pro komitování.
2. Zobrazte nastavení pro váš lokální repozitář.
3. Nastavte si své nové jméno (prohoďte třeba pořadí jména a příjmení) a email pro komitování pouze pro jeden konkrétní repozitář.
4. Vytvořte si novou větev „new-collaborator“.
5. Přidejte nový soubor Titan.txt
6. Komitněte změny.
7. Zobrazte historii komitů a zkontrolujte si, že komit je podepsaný opravdu novým jménem.

### Řešení 1

```bash
git config --global user.name "klara vesela"
git config --global user.email "k.vesel8@seznam.cz"
git config --list
git config --local user.name "Klara"
git config --local user.email "Klara856@seznam.cz"
git checkout -b new-collaborator
git status
git add Titan.txt
git status
git commit -m "pridani textoveho souboru"
git log
```

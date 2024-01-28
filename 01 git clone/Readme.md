# Cvičení git clone

## Cvičení 1

1. Vytvořte nový adresář u sebe na počítači.
2. Naklonujte do něj repozitář s projektem z GitHubu, např. https://github.com/KUTlime/Git-cheatsheet.git

### Řešení 1

```bash
git clone https://github.com/KUTlime/Git-cheatsheet
```

## Cvičení 2

1. Naklonujte veřejný projekt ze svého účtu na GitHubu na svůj počítač pomocí příkazu git clone.
2. Upravte nějaký soubor ve svém lokálním repozitáři.
3. S pomocí git příkazu, ověřte, že změny se neuložily na server a že na serveru je stále původní verze.

### Řešení 2

```bash
git clone https://github.com/kvesel8/test-repository-GIT-kurz
(pridani textu do readme.md)
git fetch
git diff origin
```

## Cvičení 3

1. Zkuste naklonovat projekt z jiné větve pomocí příkazu git clone.
2. S pomocí git příkazu, ověřte, že jste úspěšně naklonovali projekt z požadované větve.

### Řešení 3

```bash
git clone -b clone-exercises https://github.com/kvesel8/test-repository-GIT-kurz/tree/clone-exercises
git remote show origin
```

## Cvičení 4

Uveďte všechny příkazy, které musíte zadat do příkazové řádky. Citlivé údaje pozměňte, aby nebyly zneužitelné (_tj. nekopírujte celé klíče_).

1. Naklonujte repozitář s projektem na vzdáleném serveru pomocí SSH.

### Řešení 4

```bash
ssh-keygen
(vygenerování public/private key a uložení do souborů - rsa, rsa.pub)
ssh -T git@github.com

```

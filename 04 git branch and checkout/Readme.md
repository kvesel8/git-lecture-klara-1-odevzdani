# Cvičení git branch & git checkout

## Cvičení 1

1. Vytvořte novou větev s názvem "test-branch"
2. Přepněte se na tuto větev pomocí příkazu git checkout.
3. Vytvořte nový soubor Neptun.txt.
4. Komitněte tyto změny na této nové větvi.
5. Vraťte se zpět na hlavní větev a ověřte, že změny **nejsou** viditelné.

### Řešení 1

```bash
git branch test-branch
git checkout test-branch
(vytvoreni Neptun.txt)
git add Neptun.txt
git commit -m "pridani Neptun souboru"
git checkout master
git status
git log
```

## Cvičení 2

1. Na jeden příkaz, vytvořte novou větev „feature/test-branch“ a přepněte se do ní.
2. Všimněte si, že větev se jmenuje stejně jako v předchozím příkladu. Popřemýšlejte proč.
3. Vytvořte nový soubor Pluto.txt
4. Udělejte komit.

### Řešení 2

```bash
git checkout -b feature/test-branch
git add Pluto.txt
git commit -m "novy soubor pluto"
```

## Cvičení 3

1. Na hlavní větvi vytvořte soubor Europa.txt.
2. Přesuňte ho do stage area.
3. Vytvořte a přepněte se do nové větve „feature/europa-file“.
4. Proveďte komit. Všimněte si, v jaké větvi soubor skončil. Pokud to není zřejmé, přepněte se mezi větvemi „feature/europa-file“ a hlavní větví.

### Řešení 3

```bash
git checkout master
git add Europa.txt
git checkout -b feature/europa-file
git commit  
soubor skončil ve větvi feature/europa-file
```

## Cvičení 4

1. Přepněte se do větve „feature/europa-file“.
2. Zkuste vytvořit novou větev s názvem „test-branch“. Všimněte si, jak bude git reagovat.

### Řešení 4

```bash
git checkout feature/europa-file
git branch test-branch
(fatal: a branch named 'test-branch' already exists)
```

## Cvičení 5

1. Vypište všechny větve ve vašem repozitáři. Povšimněte si, jak dává Git najevo, která větev je aktivní.

### Řešení 5

```bash
git branch
(aktivní větev je napsaná barevně a tučně a má u sebe hvězdičku)
```

## Cvičení 6

1. Vytvořte novou větev „test-feature“.
2. Nyní tuto větev smažte.

### Řešení 6

```bash
git branch test-feature
git branch
git branch --delete test-feature
git branch
```

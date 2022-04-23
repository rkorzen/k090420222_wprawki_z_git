# Wprawki z git


git add .
git commit -m "init"


git log

git show

git show @^^

## conflict

```
    <<<<<<< HEAD

    ## conflict


    =======
    ## konflikt 2
    >>>>>>> 5566029aa93db9f6d9acc47d3b78a4d06b7e00c0
```

## Jak uzywac git stash

    rkorzen@MacBook-Pro-Rafa-2 wprawki_z_git % git stash
    Zapisano katalog roboczy i stan indeksu WIP on master: 1cbe52e Merge with origin master
    rkorzen@MacBook-Pro-Rafa-2 wprawki_z_git % git stash pop
    Na gałęzi master
    Zmiany nie przygotowane do złożenia:
      (użyj „git add <plik>...”, żeby zmienić, co zostanie złożone)
      (użyj „git restore <plik>...”, aby odrzucić zmiany w katalogu roboczym)
        zmieniono:       README.md

    brak zmian dodanych do zapisu (użyj „git add” i/lub „git commit -a”)
    Porzucono refs/stash@{0} (4ae9f78495164fe6a1b1c4ad7cd07432a9a2987c)
    rkorzen@MacBook-Pro-Rafa-2 wprawki_z_git % git pull origin master
    remote: Enumerating objects: 5, done.
    remote: Counting objects: 100% (5/5), done.
    remote: Compressing objects: 100% (3/3), done.
    remote: Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
    Rozpakowywanie obiektów: 100% (3/3), 698 bajtów | 232.00 KiB/s, gotowe.
    Z https://github.com/rkorzen/k090420222_wprawki_z_git
     * branch            master     -> FETCH_HEAD
       1cbe52e..f381db8  master     -> origin/master
    Aktualizowanie 1cbe52e..f381db8
    error: Scalenie nadpisałoby zmiany w następujących plikach:
        README.md
    Złóż swoje zmiany lub dodaj do schowka zanim je scalisz.
    Przerywanie
    rkorzen@MacBook-Pro-Rafa-2 wprawki_z_git % git stash
    Zapisano katalog roboczy i stan indeksu WIP on master: 1cbe52e Merge with origin master
    rkorzen@MacBook-Pro-Rafa-2 wprawki_z_git % git pull origin master
    Z https://github.com/rkorzen/k090420222_wprawki_z_git
     * branch            master     -> FETCH_HEAD
    Aktualizowanie 1cbe52e..f381db8
    Fast-forward
     README.md | 1 +
     1 file changed, 1 insertion(+)
    rkorzen@MacBook-Pro-Rafa-2 wprawki_z_git % git stash pop
    Auto-scalanie README.md
    KONFLIKT (zawartość): Konflikt scalania w README.md
    Wpis pozostaje w schowku w razie, gdyby miał być znów potrzebny.


## niepewna zmiana


## konflikt 2 zdalnie



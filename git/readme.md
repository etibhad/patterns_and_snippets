# git

# git programs (from CLI)

```
git gui &
gitk &
gitk --all &
```

# git commands

```
# megmutatja az aktuális branchet és hogy mely fájlok vannak létrehozva
git status

# ezzel adjuk hozzá a staging area-hoz a fájlokat
git add <FILE_NAME>

# a stagingben lévő fájlokból egy commit készítése commit üzenettel
git commit -m "<COMMIT_MESSAGE>"

# megmutatja a fát/historty-t
git log
git log --oneline

# felteszed a távoli szerverre(remote) az ott nem létező commitokat
git push

# a remotra felküldi a master égon lévő commitokat, amik még ott nem léteznek
git push origin master
```

# git commands TODO

* git reset
* git reset --hard HEAD~1
* git clean
* git stash
* git stash drop

# git modify existing commits

```
# a stagingben lévő fájlokat(zöld színűek) fűzi hozzá ahhoz a commithoz módosít, amire a HEAD mutat (sárga pötty), módosul a commit és a commithoz tartozó hash is
git commit --amend

# ha már beküldésre került az eredeti commit a régi hashel, akkor ezzel lehet kikényszeríteni az új beküldést
git push -f
git push -f origin master
```

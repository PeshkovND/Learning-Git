# Branches

## 1.Создать файл LearningGit.md

```
touch Learning.md
git add Learning.md
git commit -m "add LearningGit.md"
git push origin master
```

## 2.Создать ветку main на основе master

```
git checkout -b main
```

## 3.Создать ветку dev на основе main

```
git checkout -b dev
```

## 4.Удалить ветку master

```
git branch -d master
git push origin --delete master
```

## 5. Перенести изменения в remote репозиторий

```
git push origin --all
```

## 6.Переименовать dev в develop

```
git branch -m develop
```

## 7. Обновить remote репозиторий

```
git push origin --delete dev
git push origin develop
```

## 8. Сделать ветку experiment/git-merge

```
git checkout -b experiment/git-merge
```

## 9. Изменить удалить первую строчку README.md

## 10. Закомитить

```
git add README.md
git commit -m "change first string"
```

## 11. Добавить новую строчку в конец файла // контент произвольный
 
## 12. Закоммитить

```
git add README.md
git commit -m "add new string at the end"
```

## 13. Запушить

```
git push origin experiment/git-merge
```

## 14. Переключиться на ветку develop

```
git checkout develop
```

## 15. Изменить первую строчку README.md

## 16. Добавить новую строку в в конец файла README.md// контент произвольный

## 17. Закоммитить и запушить

```
git add README.md
git commit -m "change readme"
git push origin develop
```

## 18. Сделать Pull Request(Merge Request) из ветки experiment/git-merge в develop

## 19. Локально смержить ветку develop в experiment/git-merge и разрешить конфликты

```
git merge experiment/git-merge
git add README.md
```

## 20. Закоммитить и запушить

```
git merge --continue
git push origin develop
```

## 21. Убедиться, что нет конфликтов

## 22. Смержить Merge Request

# Rebase

## 1. Создать ветку experiment/git-rebase

```
git checkout -b 'experiment/git-rebase'
```

## 2. Сделать 3 коммита // произвольные изменения

## 3. Закоммитить и запушить

## 4. Использую команду rebase в интерактивном режиме объединить 3 последних коммита в один

## 5. Запушить

## 6. Должна возникнуть ошибка, что локальная и удаленная история git отличаются
 
## 7. Сделать force push для ветку experiment/git-rebase

## 8. Сделать еще один коммит

## 9. Обновить описание последнего коммита использую commit c флагом amend

## 10. Запушить

## 11. Добавить несколько файлов

## 12. Закоммитить и запушить

## 13. Разделить предыдущий коммит на два по файлам используя soft reset.

## 14. Запушить

## 15. Сделать произвольные изменения и добавить в индекс (staged or indexed состояние)

## 16. Переключиться на develop ветку без переноса измененных файлов

## 17. Применить изменения сделанные в ветке experiment/git-rebase

## 18. Удалить изменения из индекса

## 19. Отменить изменения на ветке develop

## 20. Снова применить спрятанные (stashed) изменения

## 21. Снова отменить используя hard reset

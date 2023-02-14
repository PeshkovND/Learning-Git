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

## 11. Добавить новую строчку в конец файла // контент произвольный

## 12. Закоммитить

## 13. Запушить

## 14. Переключиться на ветку develop

## 15. Изменить первую строчку README.md

## 16. Добавить новую строку в в конец файла README.md// контент произвольный

## 17. Закоммитить и запушить

## 18. Сделать Pull Request(Merge Request) из ветки experiment/git-merge в develop

## 19. Локально смержить ветку develop в experiment/git-merge и разрешить конфликты

## 20. Закоммитить и запушить

## 21. Убедиться, что нет конфликтов

## 22. Смержить Merge Request

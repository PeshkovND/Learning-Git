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

```
git add LearningGit.md
git commit -m "add Rebase layout to LearningGit.md"
git add README.md
git commit -m "add ! to hello"
git add README.md
git commit -m "add ! to Learning Git"
```
## 3. Закоммитить и запушить

```
git push origin experiment/git-rebase
```
## 4. Использую команду rebase в интерактивном режиме объединить 3 последних коммита в один

```
git rebase -i HEAD~3
```

В текстовом редакторе:

```
pick 714b535 add Rebase layout to LearningGit.md
squash 54f7fa1 add ! to hello
squash c6f8355 add ! to Learning Git

rebase 3 commits
```

## 5. Запушить

```
git push origin experiment/git-rebase
```

## 6. Должна возникнуть ошибка, что локальная и удаленная история git отличаются
 
## 7. Сделать force push для ветку experiment/git-rebase

```
git push -f origin experiment/git-rebase
```

## 8. Сделать еще один коммит

```
git commit -m "add 7 steps in LearningGit.md"
```

## 9. Обновить описание последнего коммита использую commit c флагом amend

```
git commit --amend -m "update LerningGit.md"
```

## 10. Запушить

```
git push origin experiment/git-rebase
```

## 11. Добавить несколько файлов

```
git add file1.txt
git add file2.txt
```

## 12. Закоммитить и запушить

```
git commit -m "add 2 files"
git push origin experiment/git-rebase
```

## 13. Разделить предыдущий коммит на два по файлам используя soft reset.

```
git reset --soft HEAD~1
git add file1.txt
git commit -m "add first file"
git add file2.txt
git commit -m "add second file"
```

## 14. Запушить

```
git push -f origin experiment/git-rebase
```

## 15. Сделать произвольные изменения и добавить в индекс (staged or indexed состояние)

```
git add .
```

## 16. Переключиться на develop ветку без переноса измененных файлов

```
git stash
git checkout develop
```

## 17. Применить изменения сделанные в ветке experiment/git-rebase

```
git stash apply
```

## 18. Удалить изменения из индекса

```
git reset
```

## 19. Отменить изменения на ветке develop

```
git clean -fd
```

## 20. Снова применить спрятанные (stashed) изменения

```
git stah apply
```

## 21. Снова отменить используя hard reset

```
git reset --hard
```

# Tagging

## 1. Поставить lightweight тег любой коммит

```
git tag experiment HEAD
```

## 2. Запушить тег в ремоут

```
git push origin experiment
```

## 3. Убедиться, что тег появился в ремоут репозитории

## 4. Добавить еще один тег на тот же коммит

```
git tag experiment2 HEAD
```

## 5. Удалить предыдущий тег локально и в ремоут

```
git tag -d experiment
git push origin --delete experiment
```

## 6. Убедиться что старый тег удален и новый добавлен в ремоут репе

## 7. Переключить на состояние 3 или 4 коммита назад

```
git checkout HEAD~3
```

## 8. Вернуться в состояние последнего коммита, используя commit hash

```
git checkout ea12e05c6e55c9f6bcd3f3fe4492a822a7374042
```

## 9. Переключить на состояние 3 или 4 коммита назад

```
git checkout HEAD~3
```

## 10. Вернуться в состояние последнего коммита, используя добавленный tag

```
git checkout experiment2
```

# Misc

## 1. Проверить ссылку на текущий ремоут git remote -v

```
git remote -v
```

## 2. Удалить ссылку на текущий ремоут

```
git remote rm origin
```

## 3. Убедиться, что ссылка удалена

```
git remote -v
```

## 4. Сделать новый коммит

## 5. Попытаться запушить

## 6. Добавить ссылку на ремоут используя протокол ssh

## 7. Запушить изменения

## 8. Настроить вызов кастомного редактора в гит конфиге 

## 9. Убедиться, что вызывается установленный редактор

    1. Сделать произвольные измения

    2. Сделать коммит используя git commit. Должен появиться редактор для добавления сообщения коммита

## 10. *Установить приложение SourceTree [https://www.sourcetreeapp.com/](https://www.sourcetreeapp.com/), поиграться с интерфейсом для выполнения разных операций, которые были использованы выше

## 11. *Установить приложение gitup: [https://gitup.co/](https://gitup.co/) поиграться с интерфейсом для выполнения разных операций, которые были использованы выше
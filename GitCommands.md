GIT COMMANDS

1. Создать внешний репозиторий c названием JSON.
2. Клонировать репозиторий JSON на локальный компьютер.
```
git clone https (или ssh git@github.com:IrinaDKuz/TXT.git)
```
3. Внутри локального JSON создать файл “new.json”.
```
touch new.json
```
7. Добавить файл под гит.
```
git add new.json (или .)
```
8. Закоммитить файл.
```
git commit -m "new.json add"
```
9. Отправить файл на внешний GitHub репозиторий.
```
git push
```
10. Отредактировать содержание файла “new.json” - написать информацию о себе (ФИО, возраст, количество домашних животных, будущая желаемая зарплата). Всё написать в формате JSON.
``` 
cat >> preferences.json
```
или
```
vim preferences.json
i
esc
:wq
```
11. Отправить изменения на внешний репозиторий.
```
git commit -am "added new info in new.json"
git push
```
12. Создать файл preferences.json
```
touch preferences.json
```
13. В файл preferences.json добавить информацию о своих предпочтениях (Любимый фильм, любимый сериал, любимая еда, любимое время года, сторона которую хотели бы посетить) в формате JSON.
```
vim preferences.json
```
14. Создать файл sklls.json добавить информацию о скиллах которые будут изучены на курсе в формате JSON
```
touch skils.json
vim skils.json
```
15. Отправить сразу 2 файла на внешний репозиторий.
```
git add .
git commit -m "added two new json files"
git push
```
или в одну строку:
```
git add . && git commit -m "added two new json files"
git push
```
16. На веб интерфейсе создать файл bug_report.json.
17. Сделать Commit changes (сохранить) изменения на веб интерфейсе.
18. На веб интерфейсе модифицировать файл bug_report.json, добавить баг репорт в формате JSON.
19. Сделать Commit changes (сохранить) изменения на веб интерфейсе.
20. Синхронизировать внешний и локальный репозиторий JSON
```
git pull
```
21. Информация о статусе
```
git status
```

GitHub. HW_2

1. На локальном репозитории сделать ветки для:
- Postman
- Jmeter
- CheckLists
- Bag_Reports
- SQL
- Charles
- Mobile_Testing
Создать ветку:
```
git branch Postman
```
или
```
git checkout -b Postman
```

Проверить какие сетки созданы:
```
git branch
```

2. Запушить все ветки на внешний репозиторий
```
git push --all origin 
```

3. В ветке Bag_Reports сделать текстовый документ со структурой баг репорта
```
git checkout Bag_Reports
touch bugReport.txt
vim bugReport.txt
```

4. Запушить структуру багрепорта на внешний репозиторий
```
git add .
git commit -m "bug report was added"
git push -u origin Bag_Reports
```
5. Вмержить ветку Bag Reports в Main
```
git checkout main
git merge Bag_Reports
```
6. Запушить main на внешний репозиторий.
```
git add .
git commit -m "Bag_Report merge"
git push
```
7. В ветке CheckLists набросать структуру чек листа.
```
git checkout CheckLists
touch checkList.txt
vim checkList.txt
```
8. Запушить структуру на внешний репозиторий
```
git add .   
git commit -m "CheckList was added"
git push -u origin CheckLists
```
9. На внешнем репозитории сделать Pull Request ветки CheckLists в main

10. Синхронизировать Внешнюю и Локальную ветки Main
```
git checkout main
git pull
```
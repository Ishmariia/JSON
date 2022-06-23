 4. Создать внешний репозиторий c названием JSON.
В GitHub нажать справа кнопку New > в названии Repository написать название JSON >
вибрать пункт Public > поставить галочку рядом с Добавить файл README. Внизу нажать кнопку Создать репозиторий

5. Клонировать репозиторий JSON на локальный компьютер. (В репозитории в правом верхнем углу нажать кнопку "Code" скопировать ссылку HTTPS>в рабочей папке открыть GitBash Here и вставит в терминал>нажать "Enter")  
git clone https://github.com/Ishmariia/JSON.git

 6. Внутри локального JSON создать файл “new.json”.
touch new.json
 7. Добавить файл под гит.

git add new.json

8. Закоммитить файл.
git commit -m "add new.json file"

9. Отправить файл на внешний GitHub репозиторий.
git push

10. Отредактировать содержание файла “new.json” - написать информацию о себе (ФИО, возраст, количество домашних животных, будущая желаемая зарплата). Всё написать в формате JSON.
 vim new.json
{
"FuLL Name":"Ishchenko Mariia Viktorovna",
"Age":28,
"Animals":"none",
"Desired salary":[700$, 800$, 900$, 1000$]
}

11. Отправить изменения на внешний репозиторий.
git commit -m "change json" 
 git push
 
 12. Создать файл preferences.json
touch preferences.json
 
 13. В файл preferences.json добавить информацию о своих предпочтениях (Любимый фильм, любимый сериал, любимая еда, любимое время года, сторона которую хотели бы посетить) в формате JSON.
 vim preferences.json
{
"Favorite movie": "1 + 1",
"Favorite TV series": "Friends",
"Favorite food": "pasta",
"Favorite time of year": "spring",
"Country": "Spain"
}

14. Создать файл sklls.json добавить информацию о скиллах которые будут изучены на курсе в формате JSON
cat >> sklls.json
{
"Git bash": "true",
"Android studio": "true",
"GitHub": "true",
"Postman": "true",
"text data transfer formats": ["Json","CSV","XML"]
}

15. Отправить сразу 2 файла на внешний репозиторий.
git add . 
git commit -m "new file preferences & skill" 
git push

16. На веб интерфейсе создать файл bug_report.json.
В репозитории GitHub нажать на кнопку "add file"> выбрать create new file > создать bug_report.json

 17. Сделать Commit changes (сохранить) изменения на веб интерфейсе.
Сохранить в github

 18. На веб интерфейсе модифицировать файл bug_report.json, добавить баг репорт в формате JSON.
{
    "ID": 696,
    "Title": "Parameters of the Send e-mail button, do not send data to e-mail when the data is entered correctly",

    "Severity": "Major",
    "Priority": "Medium",
    "Environment": "Xiaomi mi 9 Lite, Android 10",


    "Precondition": "Installed app on the device",
    "STR": "1.Open the APP. 2.Tap Send Email button",
    

    "AR": "App return different links not related to sending email",
    "ER": "App return links related to sending emai"
}

 19. Сделать Commit changes (сохранить) изменения на веб интерфейсе.
В гите анизу нажать кнопку commit changes
 
 20. Синхронизировать внешний и локальный репозиторий JSON
git pull

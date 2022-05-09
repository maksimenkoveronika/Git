GitHub.HW_2

    git init HW_Git
    touch readme.md
    git status 
    git add .
    git commit -m "add readme.md"

1. На локальном репозитории сделать ветки для:
- Postman // git branch Postman
- Jmeter  // git branch Jmeter
- CheckLists  // git branch CheckLists
- Bag Reports   // git branch BagReports
- SQL   // git branch SQL
- Charles  // git branch Charles
- Mobile testing  // git branch MobileTesting

2.Запушить все ветки на внешний репозиторий
    
    git remote add origin https://github.com/maksimenkoveronika/HW_Git.git
    git push --set-upstream origin main

    git push origin Postman
    git push origin Jmeter
    git push origin CheckLists
    git push origin BagReports
    git push origin SQL
    git push origin Charles
    git push origin MobileTesting

3.В ветке Bag Reports сделать текстовый документ со структурой баг репорта

    git checkout BagReports //Перейти из ветки main в ветку BagReports 
    touch BagReports.txt
    vim BagReports.txt

        Основные поля баг
          Короткое описание
          Проект 
          Компонент приложения
          Номер версии 
          Серьезность 
          Приоритет 
          Статус 
          Автор
          Шаги воспроизведения
          Фактический 
          Результат 
          Ожидаемый результат 
          Прикрепленный файл

4.Запушить структуру багрепорта на внешний репозиторий

    git add .
    git commit -m "add new.txt"
    git push --set-upstream origin BagReports
    git push

5.Вмержить ветку Bag Reports в Main

    git checkout main
    git merge BagReports

6.Запушить main на внешний репозиторий
    
    git push

7.В ветке CheckLists набросать структуру чек листа

    git checkout CheckLists
    touch CheckLists.txt
    vim CheckLists.txt

      Структура чек листа:
          Описанная задача
          Статус

8.Запушить структуру на внешний репозиторий

    git add .
    git commit -m "add nex file"
    git status
    git push --set-upstream origin CheckLists
    git push

9.На внешнем репозитории сделать Pull Request ветки CheckLists в main

-----> New pull request //CheckLists в main

10.Синхронизировать Внешнюю и Локальную ветки Main

    git checkout main
    git pull

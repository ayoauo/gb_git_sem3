# **Инструкция по работе с Git**

![Эмбема гит](github-logo.png)

## Инициализация репозитория

Для инициализации (создания) репозитория используется команда:

    git init

## Проверка состояния репозитория

Чтобы проверить текущее состояние репозитория используется команда:

    git status

## Добавление в индекс
Для добавления файла проекта в репозиторий используется команда:

    git add <имя_файла> 

## Фиксация изменений

Для фиксации изменений в файле используется команда:

    git commit -m "<комментарий>"

## Просмотр истории коммитов

Для просмотра истории коммитов используется команда:

    git log

Для просмотра краткой истории коммитов используется команда:

    git log --oneline

## Переход к ранее сохраненным коммитам 

Для перехода к ранее сохраненному коммиту используется команда:

    git checkout <id_комита>

Для возвращения в последнее состояние файла используется команда:

    git checkout master

## Просмотр конкретных изменений в файле 

Для просмотра изменений в файле используется команда:

    git diff

Зеленым цветом показывает что было добавлено

Красным цветом указана удаленная информация 

Для просмотра разницы между двумя коммитами используется команда:

    git diff <id_комита1> <id_комита2>

Важен порядок создания коммитов!    

## Ветвление

Общая информация о ветвлении:

Ветвление означает, отклонение от основной линии разработки и продолжение работы, без вмешательства в основную линию.

### Слияние веток

Информация о слиянии веток

Это перенос кода из одной ветки в другую. Например, когда закончена работа над веткой, был сделан новый функционал или исправлен баг, она заливается в мастер-ветку. В мастер-ветке код проверяется еще раз и выкладывается на рабочий сервер.

#### Создание новой ветки

Для создания новой ветки, используется команда:

    git branch <branch_name>  

#### Просмотр всех веток

Для просмотра всех веток, используется команда:

    git branch

Зеленое выделение со звездочкой (*) указывает в какой ветке мы сейчас находимся 

#### Переход на другую ветку

Для перехода на другую ветку, используется команда:

    git checkout <branch_name>

#### Команда слияния 

Для того, чтобы влить ветку в текущую нужно использовать команду:

    git merge <branch_name>

Важно! Нужно находиться в той ветке в которую вливаем и указываем имя ветки из которой происходит влитие.    

#### Удаление ветки

После того как работа с веткой закончена, ее необходимо удалить для поддержания порядка в репозитории.

Для этого используется команда:

    git branch -d <branch_name>

## Удаленные репозитории    

Удаленные репозитории нужны для совместной работы.

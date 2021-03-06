# Инструкция по работе с git

 ![error](Fedya.jpg)
 
## Начало работы с репозиторием
> git init

* Cоздает в директории пустой репозиторий в виде директории .git, где и будет в дальнейшем храниться вся информация об истории коммитов, тегах — о ходе разработки проекта

Если при регистрации не бало задано имя пользователя то:

> git config --global user.name "Slava"

> git config --global user.emeil "antonevich@mail.ru"

## Добавление файлов в репозиторий


> git add file_name

Добавляет файл file_name для отслеживания, которые затем войдут в коммит.


>git commit -m "some message"

Фиксирует все файлы, которые были добавлены для отслеживания

## Отслеживание состояния репозитория

> git status

Команду git status, пожалуй, можно считать самой часто используемой наряду с
командами коммита и индексации. Она выводит информацию обо всех изменениях,
внесенных в дерево директорий проекта по сравнению с последним коммитом рабочей
ветки;

Показывает измененные файлы и файлы готовые для commit

> git log

для визуализации веток добовляйте тег:
>git log --graph

Короткая справка по всем коммитам, коснувшимся активной в настоящий момент ветки.

> git diff

Показывает разницу между текущей версией и сохраненной

## Переход между коммитами
> git checkout commit_code

Переходит к коммиту с кодом commit_code  (его можно посмотреть по git log) 

> git checkout master

 Вернуться к актуальному состоянию




## Ветки в git

Чтобы посмотреть все ветки: 

> git branch
Для создания ветки brsnch_neme:

> git branch branch_neme

Переместиться к ветке branch_neme

> git checkout branch_neme

 ## Удаление веток

Удалить ветку с именем branch_neme можно командой:

 > git branch -d branch_neme

Для удаления ветки игнорируя все ошибки:

>git branch -D branch_neme

## Слияние веток и решение конфликтов

Команда для выкачивания информации из ветки branch_neme в текущую ветку:

> git merg branch_neme

## Слияние веток и решение конфликтов

Команда для выкачивания информации из ветки branch_neme в текущую ветку:

>git merge branch_neme

**Для того, чтобы решить конфликт, нужно убрать лишние строки и отредактировать текст:**

## Cправка
Чтобы вызвать справку для какой-то команды, нужно добавить:

>--help

Примеры:

>git add --help

>git commit --help

>branch --help




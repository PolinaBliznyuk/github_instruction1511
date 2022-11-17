# Инструкция для работы с Git и удалёнными репозиториями # 

**Что такое Git?**

Git - это одна из реализаций распределённых систем контроля версий, имеющая как и локальные, так и удалённые репозитории. Является самой популярной реализацией систем контроля версий в мире.

**Подготовка репозитория**

Для создание репозитория необходимо выполнить команду *git init* в папке с репозиторием и у Вас создаться репозиторий (появится скрытая папка *.git)*

**Создание коммитов**

__Git add__

Для добавления измений в коммит используется команда *git add.* Чтобы использовать команду *git add* напишите *git add* <имя файла>

**Создание коммитов**

Для того, чтобы создать коммит(сохранение) необходимо выполнить команду *git commit.* Выполняется она так: *git commit -m* "<сообщение к коммиту>. Все файлы для коммита должны быть ДОБАВЛЕНЫ и сообщение к коммиту писать *__ОБЯЗАТЕЛЬНО__*.

**Перемещение между сохранениями**

Для того, чтобы перемещаться между коммитами, используется команда *git checkout*. Используется она в папке с пепозиторием следующим образом: *git checkout <номер коммита>*

**Журнал изменений**

Для того, чтобы посмтреть все сделанные изменения в репозитории, используется команда *git log*. Для этого достаточно выполнить команду *git log* в папке с репозиторием

** Ветки в *Git* **

**Создание ветки**

Для того, чтобы создать ветку, используется команда *git branch.* Делается это следующим образом в папке с репозиторием: *git branch <название новой ветки>*

**Слияние веток**

Для того чтобы дабавить ветку в текущую ветку используется команда *git merge*

**Удаление веток**

Для удаления ветки ввести команду *"git branch -d 'name branch'"*

**Создание картинов**

![pictures](https://thumb.tildacdn.com/tild6336-6565-4834-b433-616638643930/-/resize/960x/-/format/webp/2_git_fetch_pull_pus.png)

!\[text]\(name.gif)

**Ветки**

Ветки нужны, чтобы несколько программистов могли вести работу над одним и тем же проектом или даже файлом одновременно, при этом не мешая друг другу.

Кроме того, ветки используются для тестирования экспериментальных функций: чтобы не повредить основному проекту, создается новая ветка специально для экспериментов. Если эксперимент удался, изменения с экспериментальной ветки переносятся на основную, если нет – новая ветка попросту удаляется, а проект остается нетронутым.

Больше информации [тут](https://smartiqa.ru/courses/git/lesson-3).

**Просмотр старых коммитов и перемещение указателя HEAD**

Итак, пришло время разобраться, каким образом можно перемещать HEAD (и другие указатели тоже) и что это дает. Для начала нужно прояснить несколько важных аспектов, которые мы уже упоминали, но не обращали ваше внимание на них:

1. Весь репозиторий – это древовидный граф, ноды которого – наши коммиты, а ребра – родительские отношения между коммитами.
2. *HEAD* – это указатель (то есть ссылка на один из коммитов), главное назначение которого - определять, в каком состоянии находится рабочая копия. На какой коммит указывает *HEAD* – в таком состоянии файлы и находятся в рабочей области.
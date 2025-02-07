# Инструкция для работы с Git и удалёнными репозиториями
## Что такое Git?
Git - это одна из реализаций распределённых систем контроля версий, имеющая как и локальные, так и удалённые репозитории. Является самой популярной реализацией систем контроля версий в мире.

## Подготовка репозитория
Для создание репозитория необходимо выполнить команду *git init* в папке с репозиторием и у Вас создаться репозиторий (появится скрытая папка .git)

## Создание коммитов
### Git add
Для добавления измений в коммит используется команда *git add*. Чтобы использовать команду *git add* напишите *git add <имя файла>*

### Просмотр состояния репозитория
Для того, чтобы посмотреть состояние репозитория используется команда *git status*. Для этого необходимо в папке с репозиторием написать *git status*, и Вы увидите были ли измения в файлах, или их не было.

### Создание коммитов
Для того, чтобы создать коммит(сохранение) необходимо выполнить команду *git commit*. Выполняется она так: *git commit -m "<сообщение к коммиту>*. Все файлы для коммита должны быть **ДОБАВЛЕНЫ** и сообщение к коммиту писать **ОБЯЗАТЕЛЬНО**.

## Перемещение между сохранениями
Для того, чтобы перемещаться между коммитами, используется команда *git checkout*. Используется она в папке с пепозиторием следующим образом: *git checkout <номер коммита>*

## Журнал изменений
Для того, чтобы посмтреть все сделанные изменения в репозитории, используется команда *git log*. Для этого достаточно выполнить команду *git log* в папке с репозиторием

## Ветки в Git
### Создание ветки
Для того, чтобы создать ветку, используется команда *git branch*. Делается это следующим образом в папке с репозиторием: *git branch <название новой ветки>*

## Слияние веток
Для того чтобы дабавить ветку в текущую ветку используется команда *git merge*

## Удаление веток
Для удаления ветки ввести команду "git branch -d 'name branch'"

## Копирование внешнего репозитория  на свой компьютер
***git clone*** -  Команда git clone иногда выступает в роли оболочки для других команд. 
Она создает новую папку, переходит в нее и запускает команду **git init** для создания пустого Git-репозитория. 
Затем она добавляет удаленный репозиторий **(git remote add)** по URL-адресу, который вы ей передали (по умолчанию он получает имя **origin**), выполняет из этого репозитория команду **git fetch**, а затем выгружает самый последний коммит в рабочую папку командой **git checkout**.

## Отправление своей версии репозитория во внешний репозиторий
***git push*** Команда **git push** используется для взаимодействия с другим репозиторием, 
вычисления данных, которые есть в вашей локальной базе, но отсутствуют там, 
и передачи этих данных в упомянутый репозиторий. Так как в данном случае 
требуется право на запись в чужой репозиторий, команда прибегает к процедуре 
аутентификации.

## Скачивание всего из текущего репозитория и автоматическое *merge* с нашей версией
***git pull*** - Команда **git pull**, по сути, представляет собой комбинацию Git-команд **fetch** и 
**git merge**. То есть система Git сначала извлекает информацию из указанного вами 
удаленного репозитория, а затем пытается вставить ее в текущую ветку.



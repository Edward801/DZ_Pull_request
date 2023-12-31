# Инструкция для работы с Git и удаленными репозиториями

## Что такое Git?
Git - это одна из реализаций распределенных систем контроля версий, имеющая как и локальные, так и удаленные репозитории. Является самой популярной реализацией систем контроля версий в мире.
## Подготовка репозитория
```sh
git init
```

Для создания репозитория необходимо выполнить команду *git init* в папке с репозиторием и у Вас создастся репозиторий (появиться папка .git)

## Создание коммитов

### Git add
```sh
git add
```

Для добавления изменений в коммит используется команда *git add* напишите *git add <имя файла>*

### Просмотр состояния репозитория
Для того, чтобы посмотреть состояние репозитория используется команда *git status*. Для этого необходимо в папке с репозиторием написать *git status* и Вы увидите были ли изменения в файлах, или их не было.

### Создание коммитов
```sh
git commit
```

Для того, чтобы создать коммит(сохранение) необходимо выполнить команду *git commit*. Выполняется она так *git commit -m "Message text"*

### Просмотр истории коммитов
```sh
git log
```

Для того чтобы просмотреть историю последовательности действий используется команда *git log*

### Просмотр истории коммитов в компактном виде
```sh
git log --oneline
```
Для того, чтобы просмотреть историю коммитов в компактном виде используется команда *git log --oneline*

### Переключение между состояниями структуры (ветки)
```sh
git checkout <имя_ветки>
```
Для того, чтобы переключаться между состояниями структуры в разный момент времени создания используется команда *git checkout<Хеш коммита>*

Отображение всех веток
```sh
git branch
```
Создание новой ветки
```sh
git branch <имя_ветки>
```
Добавили команду удаления ветки -d<имя ветки>
```sh
git branch -d <имя_ветки>
```
Для наглядного изображения изменения структуры изпользуется команда *graph*
```sh
git log --graph
```
### Работа с удаленными репозиториями
```sh
git clone <адрес удаленного репозитория>
```
Для копирования удаленного репозитория изпользуется команда clone

Создание файла README.md в папке My_first_repoz
```sh
echo "# my_first_repoz" >> README.md
```

Команда отправления всех изменений на удаленный сервер в ветку main
```sh
git push -u origin main
```
Команда запроса изменений из удаленного сервера
```sh
git pull
```

Команда добавления новой ветки на удаленный сервер
```sh
git push --set-upstream origin newbranch1
```
Команда удаления удаленной ветки через консоль
```sh
git push origin --delete <имя ветки>
```

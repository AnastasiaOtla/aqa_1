# git fetch VS git pull

## Загрузить содержимое из удаленного репозитория можно с помощью двух команд: **git pull** и **git fetch**.

### *git fetch* можно считать «безопасным» вариантом. Она загружает удаленное содержимое, но не обновляет рабочее состояние локального репозитория, оставляя текущую работу нетронутой.

### Команда *git pull* действует более агрессивно: она загружает удаленное содержимое для активной локальной ветки и сразу выполняет команду *git merge*, создавая коммит слияния для нового удаленного содержимого. Если у вас есть ожидающие изменения, то возникнут конфликты, и будет запущен процесс разрешения конфликтов слияния.

Команда **git commit --amend** — это удобный способ изменить последний коммит. Она позволяет объединить проиндексированные изменения с предыдущим коммитом без создания нового коммита. Ее можно использовать для редактирования комментария к предыдущему коммиту без изменения состояния кода в нем. Но такое изменение не только редактирует последний коммит, но и полностью его заменяет. То есть измененный коммит станет новой сущностью с отдельной ссылкой.

# Git: всё, что нужно знать

---

Git - это распределённая система управления версиями, которая позволяет эффективно отслеживать изменения в коде и с легкостью сотрудничать с другими разработчиками.

### Основные команды Git

1. `git init` - создает новый репозиторий Git в текущей директории.
2. `git clone <URL>` - клонирует удаленный репозиторий на локальную машину.
3. `git add <файл>` - добавляет файлы в индекс для будущего коммита.
4. `git commit -m "<сообщение>"` - создает коммит с заданным сообщением, сохраняя изменения.
5. `git status` - показывает статус изменений в рабочей директории.
6. `git log` - выводит историю коммитов с информацией о каждом из них.
7. `git push` - отправляет коммиты в удаленный репозиторий.
8. `git pull` - получает и объединяет изменения из удаленного репозитория в локальной копии.
9. `git branch` - показывает список веток в репозитории.
10. `git checkout <ветка>` - переключается на указанную ветку.
11. `git merge <ветка>` - объединяет изменения из указанной ветки в текущую ветку.
12. `git reset <commit>` - возвращает репозиторий к указанному коммиту.
13. `git stash` - сохраняет текущие изменения во временном хранилище.
14. `git cherry-pick <commit>` - применяет изменения из указанного коммита в текущую ветку.

### Ключевые понятия

- **Репозиторий** - это хранилище для всех файлов и истории изменений в проекте.
- **Индекс** - это набор изменений, которые будут включены в следующий коммит.
- **Ветка** - это разветвление разработки, позволяющее работать на разных ветках изменений.
- **Коммит** - это точка в истории репозитория, содержащая информацию об изменениях и ссылку на предыдущий коммит.
- **Родительский коммит** - это предыдущий коммит, на основе которого создан новый коммит.
- **Удаленный репозиторий** - это копия репозитория, которая хранится на удаленном сервере, обычно на платформе совместной разработки, такой как GitHub.
- **Хеш (Hash)** - это уникальный идентификатор коммита в Git.
- **HEAD** - указывает на текущий коммит или ветку в проекте.
- **Статус файлов** - показывает, изменены ли файлы и находятся ли они в индексе.
- **Сообщение к коммиту** - это описание изменений, записываемое при создании коммита, чтобы легче понимать, что было сделано.

### Статусы файлов в Git

1. **Ненаблюдаемые (Untracked)**: Файлы, которые Git не отслеживает. Они не включены в индекс и не будут участвовать в коммитах.
2. **Неизмененные (Unmodified)**: Файлы, которые Git отслеживает и которые не были изменены с момента последнего коммита.
3. **Измененные (Modified)**: Файлы, в которых были внесены изменения после последнего коммита. Эти изменения не были включены в индекс и не будут включены в следующий коммит, пока файлы не будут добавлены в индекс с помощью команды `git add`.
4. **Готовые к коммиту (Staged)**: Файлы, которые были добавлены в индекс с помощью команды `git add`. Они готовы к включению в следующий коммит.
5. **Закоммиченные (Committed)**: Файлы, которые были включены в коммит и сохранены в репозитории Git.


### Инициализация проекта

Для начала работы с Git в проекте необходимо выполнить следующие шаги:

1. Открыть командную строку или терминал в корневой директории проекта.
2. Инициализировать Git репозиторий с помощью команды `git init`.
3. Добавить файлы в индекс с помощью команды `git add <файл>` или `git add .` для добавления всех файлов.
4. Создать первый коммит с помощью команды `git commit -m "<сообщение>"`.
5. Установить удаленный репозиторий с помощью команды `git remote add origin <URL>`.

Теперь вы можете начать работу с Git и эффективно управлять версиями вашего проекта.
# LR6
## Лабораторная работа №6

**Цель работы:** изучение базовых возможностей системы управления версиями, опыт работы с Git Api, опыт работы с локальным и удаленным репозиторием.

**Ход работы**

1. Создан аккаунт на сайте GitHub
![рис.1](screenshots_git/photo_2023-11-13_16-17-24.jpg)

2. Создана копия исходного репозитория в личное хранилище
![рис.2](screenshots_git/photo_2023-11-14_13-53-56.jpg)

3. Установлен Git
![рис.3](screenshots_git/photo_2023-11-13_17-42-29.jpg)

4. Настроен клиент Git (введено имя пользователя и email) с помощью команд `git config --global user.name <имя>` и `git config --global user.email <почта>`
![рис.4](screenshots_git/photo_2023-11-13_19-38-42.jpg)

5. Клонирован личный удалённый репозиторий на компьютер с помощью `git clone`
![рис.5](screenshots_git/photo_2023-11-14_14-00-09.jpg)

6. Добавлен файл через интерфейс GitHub
![рис.6](screenshots_git/photo_2023-11-14_14-02-07.jpg)

Изменения подтянуты в локальный репозиторий (переход в локальный репозиторий - `cd LR6 `,  "подтягивание" - `git pull`)
![рис.7](screenshots_git/photo_2023-11-14_14-06-57.jpg)

> Далее работа продолжена локально

7. Получена история операций веток с помощью `git log`

Для **master**
![рис.8](screenshots_git/photo_2023-11-14_14-15-50.jpg)

Для **branch1**
![рис.9](screenshots_git/photo_2023-11-14_14-25-42.jpg)

8. Просмотрены последние изменения ветки master с помощью `git log --all --graph --oneline`
![рис.10](screenshots_git/photo_2023-11-14_14-38-09.jpg)

9. Выполнено слияние веток с помощью `git merge branch1`, просматрено состояние проекта, используя `git status` и разрешен конфликт по данной ситуации с помощью `git add <file>`
![рис.11](screenshots_git/photo_2023-11-14_14-56-03.jpg)

10. Удаление побочной ветки после слияния с помощью `git branch -d <ветка>`
![рис.12](screenshots_git/photo_2023-11-14_22-51-48.jpg)

11. Проведены и зафиксированы изменения, используемые команды:
- `echo текст_изменения > файл_для_сохранения`
- `git add <файл>`
- `git commit -m "изменение n"`

Первое изменение
![рис.13](screenshots_git/photo_2023-11-14_22-54-57.jpg)

Второе изменение
![рис.14](screenshots_git/photo_2023-11-14_22-56-56.jpg)

Просмотр историй операций с помощью `git log -2`
![рис.14](screenshots_git/photo_2023-11-14_22-57-58.jpg)

12. Сделан откат коммита с помощью `git reset HEAD~1` и проверка истории изменений с помощью `git log -2`
![рис.15](screenshots_git/photo_2023-11-14_22-59-48.jpg)

13. Создана ветка для отчёта branch2 с помощью `git branch branch2`
![рис.16](screenshots_git/photo_2023-11-14_23-03-06.jpg)

14. Оформлен отчет в редакторе Notepad
![рис.17](screenshots_git/photo_2023-11-15_01-22-00.jpg)

15. Получена история операций в форматированном виде
![рис.17](screenshots_git/photo_2023-11-15_01-32-43.jpg)

16. Лог всех команд
git config - настройки  
git clone - клонирование репозитория  
git pull - извлечение и загрузка содержимого из удаленного репозитория  
git log --all --graph --oneline - вывод компактного графа истории коммитов  
git checkout - переключениt между ветками  
git log -p -2 - просмотр историй коммитов с показом изменений, внесенных в каждом коммите  
git merge - объединение изменений из одной ветки в другую  
git status - показывает состояния файлов в рабочем каталоге  
git add - добавление изменений в индекс  
git commit -m "Text" - делает для проекта снимок текущего состояния изменений, добавленных в раздел проиндексированных файлов  
git branch -d - удаление ветки  
git log --date=format:'%D' --pretty=format:"%h - %cd, %cn : %s" - вывод истории коммитов с форматированными данными  

**Вывод:** в ходе лабораторной работы были изучены базовые возможности системы управления версиями, также был получен опыт работы с Git Api и опыт работы с локальным и удаленным репозиторием.

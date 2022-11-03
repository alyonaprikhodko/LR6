#LR6
##**Лабораторная работа №6**
##Ход работы
Создаётся аккаунт в github.com. Далее при помощи Fork создаётся копия в личное хранилище из https://github.com/Kurtyanik/LR6. С помощью команды git --version в консоли скачивается git. Клиент git настраивается при помощи команды git config. Вводится Фамилия. И. О. и электронная почта пользователя (Рис. 1).<br>
![Рис. 1 - Настройка клиента](./git screens/imya i pochta.png)<br>
*Рис. 1 - Настройка клиента*<br>
Далее личный удаленный репозиторий клонируется на компьютер с помощью команды git clone (Рис. 2).<br>
![Рис. 2 - Клонирование личного удалённого репозитория](./git screens/git clone 1.png)<br>
*Рис. 2 - Клонирование личного удалённого репозитория*<br>
Посредством интерфейса GitHub создаётся новый файл file_1.txt. С помощью команды git pull продтягиваются изменения в локальный репозиторий (Рис. 3).<br>
![Рис. 3 - Подтягивание изменений в локальный репозиторий](./git screens/git pull (iz interneta d komp).png)<br>
*Рис. 3 - Подтягивание изменений в локальный репозиторий*<br>
История операций для каждой из веток просматривается при помощи команды git log (Рис. 4, 6). Смена ветки же осуществляется с помощью команды git checkout (Рис. 5).<br>
![Рис. 4 - История операций для ветки master](./git screens/git log master.png)<br>
*Рис. 4 - История операций для ветки master*<br>
![Рис. 5 - Смена ветки](./git screens/smena vetki.png)<br>
*Рис. 5 - Смена ветки*<br>
![Рис. 6 - История операций для ветки branch1](./git screens/git log branch1.png)<br>
*Рис. 6 - История операций для ветки branch1*<br>
Просмотр последних изменений для веток осуществляется посредством команды git show (Рис. 7, 8).<br>
![Рис. 7 - Просмотр последних изменений для ветки master](./git screens/git show master.png)<br>
*Рис. 7 - Просмотр последних изменений для ветки master*<br>
![Рис. 8 - Просмотр последних изменений для ветки branch1](./git screens/git show branch 1.png)<br>
*Рис. 8 - Просмотр последних изменений для ветки branch1*<br>
Слияние веток производится с помощью команды git merge, но при её выполнении происходит конфликт (Рис. 9). Просмотреть, в каком файле произошёл конфликт, можно, применив команду git status(Рис. 10). <br>
![Рис. 9 - Конфликт при применении git merge](./git screens/1st try of merge error.png)<br>
*Рис. 9 - Конфликт при применении git merge*<br>
![Рис. 10 - Файл с конфликтом](./git screens/git status (merge).png)<br>
*Рис. 10 - Файл с конфликтом*<br>
Для разрешения конфликта часть даных файла удаляется (Рис. 11, 12). <br>
![Рис. 11 - Окно файла с конфликтом](./git screens/text file.png)<br>
*Рис. 11 - Окно файла с конфликтом*<br>
![Рис. 12 - Отредактированный файл](./git screens/file without conflicts.png)<br>
*Рис. 12 - Отредактированный файл*<br>
Далее для добавления файлов в индекс применяется команда git add, и для дополнительной проверки спорного файла ещё раз выполняется git status (Рис. 13). Для сохранения данных используется команда git commit(рис.14).<br>
![Рис. 13 - Сохранение файлов в индекс; статус спорного файла после разрешения конфликта](./git screens/add+status.png)<br>
*Рис. 13 - Сохранение файлов в индекс; статус спорного файла после разрешения конфликта*<br>
![Рис. 14 - Сохранение изменений](./git screens/commit for merge.png)<br>
*Рис. 14 - Сохранение изменений*<br>
При следующей попытке выполнить команду git merge бесконфликтно происходит слияние в ветку master.<br>
![Рис. 15 - Слияние в ветку master](./git screens/merge.png)<br>
*Рис. 15 - Слияние в ветку master*<br>

Далее вызывается команда git log --graph --all, чтобы увидеть визуализацию слияния в ветку master (Рис. 16).<br>
![Рис. 16 - Визуализация слияния](./git screens/graph.png)<br>
*Рис. 16 - Визуализация слияния*<br>
После успешного слияния производится удаление побочной ветки (Рис. 17).<br>
![Рис. 17 - Удаление побочной ветки](./git screens/deleted branch1.png)<br>
*Рис. 17 - Удаление побочной ветки*<br> 

Внесение изменений происходит вручную в окне файла (Рис. 18, 19), а их фиксация - с помощью команд git add и git commit (Рис. 20, 21).<br>
![Рис. 18 - Изменения в окне файла file_1](./git screens/file_1 modifyed.png)<br>
*Рис. 18 - Изменения в окне файла file_1*<br>
![Рис. 19 - Изменения в окне файла mergefile.txt](./git screens/mergefile modified.png)<br>
*Рис. 19 - Изменения в окне файла mergefile.txt*<br>
![Рис. 20 - Первый коммит](./git screens/add+1commit.png)<br>
*Рис. 20 - Первый коммит*<br>
![Рис. 21 - Второй коммит](./git screens/add+2commit.png)<br>
*Рис. 21 - Второй коммит*<br>
Откат коммита совершается с помощью команды git reset (Рис. 22).<br>
![Рис. 22 - Откат последнего коммита](./git screens/откат коммита.png)<br>
*Рис. 22 - Откат последнего коммита*<br>
Новая ветка для отчёта так же, как и удаление побочной ветки (Рис. 17), создаётся с помощью команды git branch (Рис. 23).<br>
![Рис. 23 - Создание ветки для отчёта](./git screens/creation of branch2.png)<br>
*Рис. 23 - Создание ветки для отчёта*<br>
Скриншоты, используемые в отчёте, размещены в папке "git screens", размещённой в папке "LR6". Добавление папки так же происходит при помощи команд git add и git commit (Рис. 24).<br>
![Рис. 24 - Добавление папки](./git screens/screens added.png)<br>
*Рис. 24 - Добавление папки*<br>
По мере написания отчета создавались коммиты изменений(рис.25).<br>

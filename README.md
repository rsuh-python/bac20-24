# bac20-24

Материалы по курсу программирования в лингвистике для бакалавриата ФиПЛ набора 2020 года. 

[Таблица оценок](https://docs.google.com/spreadsheets/d/1LNxOkYlk3gi9aZqv2SniCgFOZ90BjOhXoIkVglPYKhU/edit?usp=sharing)

Краткая инструкция по Github для тех, кому она нужна:

1. Установите [git](https://git-scm.com/downloads) - можно оставить дефолтные настройки
2. Чтобы склонировать репозиторий (впервые скачать к себе на компьютер):
  - откройте командную строку от имени администратора (пуск - cmd) или терминал 
  - перейдите в папку, в которую вы хотите скачать репозиторий, с помощью команды cd (для Windows cd /d path, если другая буква диска в пути)
  - откройте страницу репозитория, нажмите зеленую кнопку Code - там будет опция скопировать адрес репозитория
  - в командной строке напишите git clone и вставьте скопированный адрес
3. Чтобы обновить уже склонированный репозиторий (будьте осторожны - если меняете какие-то файлы в этом репозитории, гит откажется его так просто обновлять, возможно, понадобится использовать команду stash:
  - откройте командную строку в папке репозитория
  - (опционально) git stash
  - git pull
  - (опционально) git stash pop
4. Чтобы создать свой собственный репозиторий в своем аккаунте:
  - заведите аккаунт как на любом другом сайте
  - можно просто заводить репозитории и заливать файлы через Upload
  - или делать это через командную строку!
  - зайдите в Settings - Developer Settings - Personal access tokens (classic), сгенерируйте токен, обязательно скопируйте его и сохраните себе, а то потом больше он вам его не покажет
  - можно создать репозиторий просто через сайт, а потом склонировать его
  - либо можно установить себе GithubCLI (gh) и заводить репозиторий с помощью консольной команды gh repo create (ввести ее в командной строке из папки с репозиторием, а дальше отвечать на вопросики)
5. Чтобы обновлять свой собственный репозиторий через командную строку:
  - зайти в папку с репозиторием через командную строку
  - git add -A
  - git commit -m "ваш комментарий к коммиту"
  - git push
  - (все три команды можно объединить в одну строку через &&)
  - вот на push гитхаб спросит ваш access token (можно в настройках в менеджере сохранить, чтобы не спрашивал)

Для совсем продвинутых ребят:

Можно сдавать мне домашние задания через Github. Для этого:

- заведите свой репозиторий для будущих домашек
- зайдите в Settings репозитория и во вкладке Collaborators добавьте меня (fortvivlan)
- создайте новую ветку (в командной строке: git checkout -b Имя_Ветки)
- делайте домашку!
- запушите в удаленный репозиторий: git add -A && git commit -m "add hw01" && git push --set-upstream origin Имя_Ветки
- создайте Pull Request (на сайте), в процессе создания выберите опцию Request reviewers и добавьте туда меня (я появлюсь там среди возможных, как только приму приглашение в коллабораторы)
- мне придет письмо с уведомлением, я напишу ревью и могу оставить комментарии. Если понадобится дорабатывать какие-то задачки, можно делать новые пуши обычным git push (set-upstream нужен только в первый раз) и новые PR
- если я сделала approve, можно мержить пулл реквест. 

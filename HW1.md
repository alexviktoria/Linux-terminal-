# Terminal HW_1
### Linux terminal (GitBash) commands

### ЗАДАНИЕ 1

__1. Посмотреть где я__

`pwd`

__2. Создать папку__

`mkdir HW1`

__3. Зайти в папку__

`cd HW1`

__4. Создать 3 паки__

`mkdir x1 x2 x3`

__5. Зайти в любую папку__

`cd x1`

__6. Создать 5 файлов (3 txt, 2 json)__

`touch f1.txt f2.txt f3.txt f4.json f5.json`

__7. Создать 3 папки__

`mkdir file_1 file_2 file_3`

__8. Вывести список содержимого папки__

`ls -la`

__9. Открыть любой txt файл__

`vim f1.txt`

__10. Написать туда что-нибудь, любой текст__

`Beautiful is better than ugly.`

`Explicit is better than implicit.`

 `Simple is better than complex.`

 `Complex is better than complicated.`

 `Flat is better than nested.`

 `Sparse is better than dense...`

__11. Сохранить и выйти__

`esc + :wq + enter`

__12. Выйти из папки на уровень выше__

`cd ..`

__13. Переместить любые 2 файла, которые создали, в любую другую папку__

`mv f1.txt f2.txt ../file_1`

__14. Переместить любые 2 файла, которые создали, в любую другую папку__

`cp f3.txt f4.json f5.json ../file_1`

__15. Найти файл по имени__

`find -name file_1`

__16. Просмотреть содержимое в реальном времени__

`tail -f f1.txt`

__17. Вывести несколько первых строк из текстового файла__

`head -3 f1.txt`

__18. Вывести несколько последних строк из текстового файла__

`tail -n2 f1.txt`

__19. Просмотреть содержимое длинного файла__

`less f1.txt`  Выход: `q`

__20. Вывести дату и время__

`date`

### ЗАДАНИЕ 2

__Отправить http запрос на сервер__

`curl http://162.55.220.72:5005/terminal-hw-request`

__приходит ответ с запросом имени и возраста отправляем:__

`curl http://162.55.220.72:5005/get_method?name="Viktoria"\&age=42`

### ЗАДАНИЕ 3

__Написать скрипт, который выполнитавтоматически пункты 3, 4, 5, 6, 7, 8, 13__

__- создаем файл__

`touch task.sh`

__- заходим в этот файл__

`vim task.sh`

__- нажимаем "i"__

__- набираем:__

`#!/bin/bash`

`cd HW1`

`mkdir x1 x2 x3`

`cd x1`

`touch f1.txt f2.txt f3.txt f4.json f5.json`

`mkdir file_1 file_2 file_3`

`ls -la`

`mv f1.txt f2.txt ../file_1`

__выйти и сохранить: нажимаем__ 

`esc :wq + enter`

__- запускаем__

`sh task.sh`

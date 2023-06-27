> Первая часть первого  ДЗ     |
> Linux terminal (GitBash) commands

|ToDo|Commands|
|:---------------|:-----|
|1) Посмотреть где я| `pwd` |
|2) Создать папку|`mkdir` Terminal|
|2) Зайти в папку|`cd` Terminal|
|4) Создать 3 папки|`mkdir` folder_1 folder_2 folder_3|
|5) Зайти в любоую папку|`cd` folder_3|
|6) Создать 5 файлов (3 txt, 2 json)|`touch` file_1.txt file_2.txt file_3.txt file_4.json file_5.json
|7) Создать 3 папки|`mkdir` dir_1 dir_2 dir_3|
|8) Вывести список содержимого папки|`ls -l`|
|9) + Открыть любой txt файл|`vim` 2.txt|
|10) + Написать туда что-нибудь, любой текст, сохранить и выйти| `esq : w q enter`|
|11) + Выйти из папки на уровень выше|`cd` ..|
|Переместить любые 2 файла, которые вы создали, в любую другую папку|`mv` 2.txt /e/NASTYA/QA/GIT/HW_github_1/folder_1/F_2|
|Скопировать любые 2 файла, которые вы создали, в любую другую папку|`cp` 3.txt 1.json /e/NASTYA/QA/GIT/HW_github_1/folder_1/F_3|
|Найти файл по имени|`find ./ -name` 3.txt|
|Просмотреть содержимое в реальном времени|`tail -f` 3.txt|
|Вывести несколько первых строк из текстового файла|`head -n3` 3.txt|
|Вывести несколько последних строк из текстового файла|`tail -n3` 3.txt|
|Просмотреть содержимое длинного файла|`less` 3.txt|
|Вывести дату и время|`date`|
|Задание * 1) Отправить http запрос на сервер http://162.55.220.72:5005/terminal-hw-request|`curl` http://162.55.220.72:5005/terminal-hw-request|

> 2) Написать скрипт который выполнит автоматически пункты 3, 4, 5, 6, 7, 8, 13

    ./script.txt
    #!/bin/bash
    mkdir folder_1
    cd folder_1
    mkdir F_1 F_2 F_3
    cd F_1
    touch 1.txt 2.txt 3.txt 1.json 2.json
    ls -la
    mkdir dir_1 dir_2 dir_3
    mv 1.txt 1.json /e/NASTYA/QA/GIT/HW_github_1/folder_1/folder_1/F_2
    cp 2.txt dir_2
    ls -la

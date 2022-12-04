# Git_Bash_HW1
### **_Задание 1. Linux terminal (GitBash) commands_**
_____________________________________________
1. Посмотреть где я - `pwd`
2. Создать папку - `mkdir HW_1`
3. Зайти в папку - `cd HW_1/`
4. Создать 3 папки - `mkdir folder_1 folder_2 folder_3`
5. Зайти в любоую папку - `cd folder_1/`
6. Создать 5 файлов (3 txt, 2 json) - `touch file1.txt file2.txt file3.txt file4.json file5.json`
7. Создать 3 папки - `mkdir papka1 papka2 papka3`
8. Вывести список содержимого папки - `ls -la`
9. Открыть любой txt файл - `vim file1.txt`
10. Написать туда что-нибудь, любой текст - `нажать i и ввести текст: Я в своем познании настолько преисполнился, что я как будто бы уже сто триллионов миллиардов лет проживаю на триллионах и триллионах таких же планет, как эта Земля, мне этот мир абсолютно понятен, и я здесь ищу только одного - покоя, умиротворения и вот этой гармонии, от слияния с бесконечно вечным, от созерцания великого фрактального подобия и от вот этого замечательного всеединства существа, бесконечно вечного, куда ни посмотри, хоть вглубь - бесконечно малое, хоть ввысь - бесконечное большое, понимаешь?`
11. Сохранить и выйти - `Esc + :wq`
12. Выйти из папки на уровень выше - `cd ..`
13. Переместить любые 2 файла, которые вы создали, в любую другую папку - `mv D:/31groupGITBASH/gitrepo/TerminalLinux/HW_1/folder_1/file4.json D:/31groupGITBASH/gitrepo/TerminalLinux/HW_1/folder_1/file5.json D:/31groupGITBASH/gitrepo/TerminalLinux/HW_1/folder_2`
14. Cкопировать любые 2 файла, которые вы создали, в любую другую папку - `cp D:/31groupGITBASH/gitrepo/TerminalLinux/HW_1/folder_1/file1.txt D:/31groupGITBASH/gitrepo/TerminalLinux/HW_1/folder_1/file2.txt D:/31groupGITBASH/gitrepo/TerminalLinux/HW_1/folder_3`
15. Найти файл по имени - `find -name file1.txt`
16. Просмотреть содержимое в реальном времени (команда grep) изучите как она работает - `grep "бесконечно" D:/31groupGITBASH/gitrepo/TerminalLinux/HW_1/folder_3/file1.txt`
17. Вывести несколько первых строк из текстового файла - `head -2 D:/31groupGITBASH/gitrepo/TerminalLinux/HW_1/folder_3/file1.txt`
18. Вывести несколько последних строк из текстового файла - `tail -2 D:/31groupGITBASH/gitrepo/TerminalLinux/HW_1/folder_3/file1.txt`
19. Просмотреть содержимое длинного файла (команда less) изучите как она работает - `less D:/31groupGITBASH/gitrepo/TerminalLinux/HW_1/folder_3/file1.txt`
20. Вывести дату и время - `date`
_____________________________________________
### **_*Задание №2 - Отправить http запрос на сервер_**
______________________________________________
`curl 'http://162.55.220.72:5005/object_info_3?name=Evgeney&age=24&salary=1200'`
_____________________________________________
### **_Задание №3 - Написать скрипт, который выполнит автоматически пункты 3, 4, 5, 6, 7, 8, 13_**
_____________________________________________
Файл со скриптом - **[script.sh](https://github.com/EvgeneyKEO/TerminalLinux/blob/67c8599bc08e0a8a946a854269542a72809c083a/script.sh)**

Команда в терминале - `./script.sh`
```
#!/bin/bash
cd folder_2/
mkdir papochka_1 papochka_2 papochka_3
cd papochka_1/
touch file1.txt file2.txt file3.txt file4.json file5.json
mkdir papochka_4 papochka_5 papochka_6
ls -la
mv file3.txt file4.json papochka_4/
```

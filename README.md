# TerminalLinux #
_____________________________________________
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
__________________________________________________________________________________
## **_Задание по GIT_**
__________________________________________________________________________________
 1. Создайте текстовый файл как в первом ДЗ по Terminal
 2. Сценарий перенесите в этот файл.
 3. На против каждого действия - напишите команду в GitBash
 _________________________________________________________________________________
 ### GIT file JSON
 _________________________________________________________________________________
 4. Создать внешний репозиторий c названием JSON            - **[JSON](https://github.com/EvgeneyKEO/JSON.git)**

 5. Клонировать репозиторий JSON на локальный компьютер     - `git clone git@github.com:EvgeneyKEO/JSON.git`

 6. Внутри локального JSON создать файл “new.json”          - `touch new.json`

 7. Добавить файл под гит.                                  - `git add .`

 8. Закоммитить файл.                                       - `git commit -m "add new file"`

 9. Отправить файл на внешний GitHub репозиторий.           - `git push`

 10. Отредактировать содержание файла “new.json” - написать 
информацию о себе (ФИО, возраст, количество домашних
животных, будущая желаемая зарплата).
Всё написать в формате JSON.                                - ```vim new.json после нажать на i ввести информацию о себе в формате JSON
                                                               {"FIO":"Kandyba Evgeney Olegovich";"age":25;"pets":1;"salary":2000}
                                                               после окончания ввода нажать Esc ввести :wq
                                                              ```
                                                               

 11. Отправить изменения на внешний репозиторий.            - ```git add . 
                                                                 git commit -m "update new.json" 
                                                                 git push
                                                              ```
 
 12. Создать файл preferences.json                          - `touch preferences.json` [preferences.json](https://github.com/EvgeneyKEO/JSON/blob/cc2c6d91e579d92e0c575d1b85dd255531e6935c/bug_report.json)

 13. В файл preferences.json добавить информацию о своих 
предпочтениях (Любимый фильм, любимый сериал, любимая еда,
любимое время года, сторона которую хотели бы посетить) 
в формате JSON.                                             - ```vim preferences.json после нажать на i ввести информацию о себе в формате JSON                                                                                          {"film":"1+1";"serial":"Peaky_Blinders";"food":"salat";"season":"winter";"country":"USA"}
                                                                 после окончания ввода нажать Esc ввести :wq
                                                              ```

 14. Создать файл skills.json добавить информацию о скиллах
которые будут изучены на курсе в формате JSON               - ```vim skills.json после нажать на i ввести информацию о себе в формате JSON
                                                                {"instruments":"postman","SQL","Jmeter","Python","Terminal","Android
                                                                Studio","XCode","DevTools","Charles","Fiddler","GitBash"}
                                                                после окончания ввода нажать Esc ввести :wq
                                                              ```

 15. Отправить сразу 2 файла на внешний репозиторий.        - ```git add .
                                                                 git commit -m "add two new files: new preferences.json skills.json"
                                                                 git push
                                                              ```


 16. На веб интерфейсе создать файл bug_report.json.        - [bug_report.json](https://github.com/EvgeneyKEO/JSON/blob/62d356725170363a1826bcee6f123ea125e261fe/bug_report.json)


 17. Сделать Commit changes (сохранить) изменения на веб интерфейсе.


 18. На веб интерфейсе модифицировать файл bug_report.json, добавить баг репорт в формате JSON.


 19. Сделать Commit changes (сохранить) изменения на веб интерфейсе.


 20. Синхронизировать внешний и локальный репозиторий JSON   - `git pull`
 _________________________________________________________________________________
 ### GIT file XML
 _________________________________________________________________________________
 21. Создать внешний репозиторий c названием XML.            - [XML](https://github.com/EvgeneyKEO/XML.git)


 22. Клонировать репозиторий XML на локальный компьютер.     - `git clone https://github.com/EvgeneyKEO/XML.git`


 23. Внутри локального XML создать файл “new.xml”.           - `touch new.xml`


 24. Добавить файл под гит.                                  - `git add .`


 25. Закоммитить файл.                                       - `git commit -m "add new.xml"`


 26. Отправить файл на внешний GitHub репозиторий.           - `git push`


 27. Отредактировать содержание файла “new.xml” - написать 
информацию о себе (ФИО, возраст, количество
 домашних животных, будущая желаемая зарплата). 
Всё написать в формате XML.                                  - ```<info>
                                                                        <FIO>Kandyba Evgeney Olegovich</FIO>
                                                                        <age>24</age>
                                                                        <pets>1</pets>    
                                                                        <salary>2000</salary>
                                                                 </info>
                                                              ```

 28. Отправить изменения на внешний репозиторий.             - ```git commit -am "update new.xml"
                                                                  git push
                                                              ```

 29. Создать файл preferences.xml                            - `touch preferences.xml` 

 30. В файл preferences.xml добавить информацию о своих 
предпочтениях (Любимый фильм, любимый сериал, любимая еда,
 любимое время года, сторона которую хотели бы посетить)
 в формате XML.                                              - ```<info>
	                                                                 <favorite_movie>1+1</favorite_movie>
		                                                         <favorite_TV_series>Peaky Blinders</favorite_TV_series>
	                                                                 <favorite_food>salat</favorite_food>
		                                                         <favorite_time_of_the_year>winter</favorite_time_of_the_year> 
	                                                                 <the_country_you_would_like_to_visit>USA</the_country_you_would_like_to_visit>
	                                                          </info>
                                                              	```   

 31. Создать файл skills.xml добавить информацию о скиллах
 которые будут изучены на курсе в формате XML		      - `Choose bug_report.json --> Edit this file`

 32. Сделать коммит в одну строку.                            - `git add . && git commit -m "Add new files"`

 33. Отправить сразу 2 файла на внешний репозиторий.	      - `git push`

 34. На веб интерфейсе создать файл bug_report.xml.           - Add file --> Create new file [bug_report.xml](https://github.com/EvgeneyKEO/XML/blob/80e38f039f2898659ea6d7ffd6e2477226ddcb08/bug_report.xml)

 35. Сделать Commit changes (сохранить) изменения 
на веб интерфейсе.					      - `Commit new file`

 36. На веб интерфейсе модифицировать файл bug_report.xml, 
добавить баг репорт в формате XML. 		     	      - `Choose bug_report.json --> Edit this file`` 

 37. Сделать Commit changes (сохранить) 
изменения на веб интерфейсе.			      	      - `Commit changes`

 38. Синхронизировать внешний и локальный репозиторий XML.    - `git pull`
 _________________________________________________________________________________
 ### GIT file TXT
 _________________________________________________________________________________
 39. Создать внешний репозиторий c названием TXT.

 40. Создать внешний репозиторий c названием TXT.

 41. Внутри локального TXT создать файл “new.txt”.

 42. Добавить файл под гит.

 43. Закоммитить файл.

 44. Отправить файл на внешний GitHub репозиторий.

 45. Отредактировать содержание файла “new.txt” - написать информацию о себе (ФИО, возраст, количество домашних животных, будущая желаемая зарплата). Всё написать в формате TXT.

 46. Отправить изменения на внешний репозиторий.

 47. Создать файл preferences.txt

 48. В файл preferences.txt” добавить информацию о своих предпочтениях (Любимый фильм, любимый сериал, любимая еда, любимое время года, сторона которую хотели бы посетить) в формате TXT.

 49. Создать файл sklls.txt добавить информацию о скиллах которые будут изучены на курсе в формате TXT.

 50. Сделать коммит в одну строку.

 51. Отправить сразу 2 файла на внешний репозиторий.

 52. На веб интерфейсе создать файл bug_report.txt.

 53. Сделать Commit changes (сохранить) изменения на веб интерфейсе.

 54. На веб интерфейсе модифицировать файл bug_report.txt, добавить баг репорт в формате TXT.

 55. Сделать Commit changes (сохранить) изменения на веб интерфейсе.

 56. Синхронизировать внешний и локальный репозиторий TXT
 




## Git Bash

##### 1. Определить имя папки, в которой вы находитесь.

ADMIN@DESKTOP-CE3F84N MINGW64 ~  
$ pwd  
/c/Users/ADMIN

##### 2. Создать папку с именем lesson1.

ADMIN@DESKTOP-CE3F84N MINGW64 ~  
$ mkdir lesson1

##### 3. Перейти в папку lesson1.

ADMIN@DESKTOP-CE3F84N MINGW64 ~  
$ cd lesson1  

ADMIN@DESKTOP-CE3F84N MINGW64 ~/lesson1

##### 4. Создать file, file2 и file3 внутри каталога lesson1.

ADMIN@DESKTOP-CE3F84N MINGW64 ~/lesson1  
$ touch file1 file2 file3  

ADMIN@DESKTOP-CE3F84N MINGW64 ~/lesson1

##### 5. Проверить содержимое каталога lesson1.

ADMIN@DESKTOP-CE3F84N MINGW64 ~/lesson1  
$ ls  
file1  file2  file3

##### 6. Создать папку lesson2 внутри домашней директории.

ADMIN@DESKTOP-CE3F84N MINGW64 ~/lesson1  
$ cd ~

ADMIN@DESKTOP-CE3F84N MINGW64 ~
$ mkdir Lesson2

##### 7. Удалить папку lesson2.

ADMIN@DESKTOP-CE3F84N MINGW64 ~
$ rmdir lesson2

##### 8. Удалить file2.

ADMIN@DESKTOP-CE3F84N MINGW64 ~  
$ cd lesson1

ADMIN@DESKTOP-CE3F84N MINGW64 ~/lesson1  
$ rm file2

##### 9. Создать папку lesson3 внутри домашней директории и добавить в нее два файла.

ADMIN@DESKTOP-CE3F84N MINGW64 ~/lesson1  
$ cd ~

ADMIN@DESKTOP-CE3F84N MINGW64 ~  
$ mkdir lesson3

ADMIN@DESKTOP-CE3F84N MINGW64 ~  
$ cd lesson3

ADMIN@DESKTOP-CE3F84N MINGW64 ~/lesson3  
$ touch les3_file1 les3_file2

ADMIN@DESKTOP-CE3F84N MINGW64 ~/lesson3  
$ ls  
les3_file1  les3_file2

##### 10. Создать папку lesson4.

ADMIN@DESKTOP-CE3F84N MINGW64 ~  
$ mkdir lesson4

##### 11. Переместить file1 и file3 в папку lesson4.

ADMIN@DESKTOP-CE3F84N MINGW64 ~/lesson4  
$ cd ~  

ADMIN@DESKTOP-CE3F84N MINGW64 ~  
$ mv lesson1/file1 lesson4

ADMIN@DESKTOP-CE3F84N MINGW64 ~  
$ mv lesson1/file3 lesson4

ADMIN@DESKTOP-CE3F84N MINGW64 ~  
$ cd lesson4

ADMIN@DESKTOP-CE3F84N MINGW64 ~/lesson4  
$ ls  
file1  file3

##### 12. Добавить в file1 три строки со словами line.

ADMIN@DESKTOP-CE3F84N MINGW64 ~/lesson4  
$ echo line line line > file1

##### 13. Посмотреть содержимое file1.

ADMIN@DESKTOP-CE3F84N MINGW64 ~/lesson4  
$ cat file1  
line line line

##### 14. Добавьте в file3 три строки со словами line.

ADMIN@DESKTOP-CE3F84N MINGW64 ~/lesson4  
$ echo line line line > file3

##### 15. Просмотрите содержимое двух файлов (1 и 3) сразу.

ADMIN@DESKTOP-CE3F84N MINGW64 ~/lesson4  
$ cat file1 file3  
line line line  
line line line

##### 16. Используя один из редакторов замените все строки

ADMIN@DESKTOP-CE3F84N MINGW64 ~/lesson4  
$ nano file1 file3

ADMIN@DESKTOP-CE3F84N MINGW64 ~/lesson4  
$ cat file1 file3  
smile smile smile  
smile smile

##### 17. Добавить в папку lesson3 три file4, file5 и file6, в каждом из которых должно быть по 4 строки row1, row2, row3, row4.

ADMIN@DESKTOP-CE3F84N MINGW64 ~  
$ cd  ~/lesson3

ADMIN@DESKTOP-CE3F84N MINGW64 ~/lesson3  
$ touch file4 file5 file6

ADMIN@DESKTOP-CE3F84N MINGW64 ~/lesson3  
$ ls  
file4  file5  file6

ADMIN@DESKTOP-CE3F84N MINGW64 ~/lesson3  
$ echo row1 row2 row3 row4 > file4

ADMIN@DESKTOP-CE3F84N MINGW64 ~/lesson3  
$ echo row1 row2 row3 row4 > file5

ADMIN@DESKTOP-CE3F84N MINGW64 ~/lesson3  
$ echo row1 row2 row3 row4 > file6

##### 18. Найдите строку row2 в file5.

ADMIN@DESKTOP-CE3F84N MINGW64 ~/lesson3  
$ grep row2 file5  
row2

##### 19. Найдите строку row в папке lesson3.

ADMIN@DESKTOP-CE3F84N MINGW64 ~  
$ cd ~/Documents

ADMIN@DESKTOP-CE3F84N MINGW64 ~  
$ grep -R row* test3  
lesson3/file4:row1  
lesson3/file4:row2  
lesson3/file4:row3  
lesson3/file4:row4  
lesson3/file5:row1  
lesson3/file5:row2  
lesson3/file5:row3  
lesson3/file5:row4  
lesson3/file6:row1  
lesson3/file6:row2  
lesson3/file6:row3  
lesson3/file6:row4

##### 20. Посчитайте сколько строк с содержимым row в file6.

ADMIN@DESKTOP-CE3F84N MINGW64 ~  
$ cd  ~/Documents/lesson3

ADMIN@DESKTOP-CE3F84N MINGW64 ~/lesson3  
$ grep -c row* file6
4

##### 21. Найдите file5 внутри папки lesson3.

ADMIN@DESKTOP-CE3F84N MINGW64 ~/lesson3   
$ find . -name file5  
./file5

##### 22. Используя команду find, удалите file5.

ADMIN@DESKTOP-CE3F84N MINGW64 ~lesson3  
$ find . -name file5 -delete -print  
./file5

ADMIN@DESKTOP-CE3F84N MINGW64 ~/lesson3  
$ ls  
file4  file6

##### 23. Используя команду echo, добавьте слово test в file4.

ADMIN@DESKTOP-CE3F84N MINGW64 ~/lesson3  
$ echo test>file4

ADMIN@DESKTOP-CE3F84N MINGW64 ~/lesson3  
$ cat file4  
test

##### 24. Замените слово test в файле 4 на fail.

ADMIN@DESKTOP-CE3F84N MINGW64 ~/lesson3  
$ echo fail>file4

ADMIN@DESKTOP-CE3F84N MINGW64 ~/lesson3  
$ cat file4  
fail

##### 25. Добавьте в файл 4 слово test так, чтобы сохранилось содержимое.

ADMIN@DESKTOP-CE3F84N MINGW64 ~/lesson3  
$ echo test>>file4

ADMIN@DESKTOP-CE3F84N MINGW64 ~/lesson3  
$ cat file4  
fail  
test

##### 26. Просмотрите все процессы для юзеров не только в консоли, которые происходят в системе.

ADMIN@DESKTOP-CE3F84N MINGW64 ~/lesson3  
$ ps aux  
      PID    PPID    PGID     WINPID   TTY         UID    STIME COMMAND  
      419     102     419      11956  pty0      197609 17:38:55 /usr/bin/ps  
      101       1     101      11868  ?         197609 16:00:14 /usr/bin/mintty  
      102     101     102      11984  pty0      197609 16:00:14 /usr/bin/bash

##### 27. Убейте процесс 666 в консоли.

ADMIN@DESKTOP-CE3F84N MINGW64 ~/lesson3
$ kill 666
bash: kill: (666) - No such process

##### 27. Узнайте доступность ресурса artsiomrusau.com, используя ping.

ADMIN@DESKTOP-CE3F84N MINGW64 ~/lesson3  
$ ping artsiomrusau.com

Pinging artsiomrusau.com [15.197.142.173] with 32 bytes of data:  
Reply from 15.197.142.173: bytes=32 time=21ms TTL=243  
Reply from 15.197.142.173: bytes=32 time=42ms TTL=243  
Reply from 15.197.142.173: bytes=32 time=24ms TTL=243  
Reply from 15.197.142.173: bytes=32 time=21ms TTL=243  

Ping statistics for 15.197.142.173:  
    Packets: Sent = 4, Received = 4, Lost = 0 (0% loss),  
Approximate round trip times in milli-seconds:  
    Minimum = 21ms, Maximum = 42ms, Average = 27ms  

##### 28. Отправьте 5 пакетов на сайт artsiomrusau.com.

ADMIN@DESKTOP-CE3F84N MINGW64 ~/lesson3  
$ ping -n 5 artsiomrusau.com

Pinging artsiomrusau.com [15.197.142.173] with 32 bytes of data:  
Reply from 15.197.142.173: bytes=32 time=46ms TTL=243  
Reply from 15.197.142.173: bytes=32 time=31ms TTL=243  
Reply from 15.197.142.173: bytes=32 time=23ms TTL=243  
Reply from 15.197.142.173: bytes=32 time=22ms TTL=243  
Reply from 15.197.142.173: bytes=32 time=45ms TTL=243  

Ping statistics for 15.197.142.173:  
    Packets: Sent = 5, Received = 5, Lost = 0 (0% loss),  
Approximate round trip times in milli-seconds:  
    Minimum = 22ms, Maximum = 46ms, Average = 33ms

##### 29. Очистить терминал.

ADMIN@DESKTOP-CE3F84N MINGW64 ~/lesson3  
$ clear

##### 30. Просмотреть историю команд в терминале. 

ADMIN@DESKTOP-CE3F84N MINGW64 ~/lesson3  
$ history  
 1  pwd  
 2  mkdir lesson1  
 3  cd lesson1  
 4  ls  
 5  touch file1 file2 file3  
 ...  
 179  kill 666  
 180  ping artsiomrusau.com  
 181  ping -n 5 artsiomrusau.com  
 182  clear  
 183  history








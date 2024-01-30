## Git Bash

##### 1. Определить имя папки, в которой вы находитесь.

ADMIN@DESKTOP-CE3F84N MINGW64 ~  
$ pwd  
/c/Users/ADMIN

##### 2. Создать папку с именем lesson1.

ADMIN@DESKTOP-CE3F84N MINGW64 ~  
$ mkdir lesson1

##### 3. Перейти в папку test1.

ADMIN@DESKTOP-CE3F84N MINGW64 ~  
$ cd lesson1  

ADMIN@DESKTOP-CE3F84N MINGW64 ~/lesson1  
$ ^C

##### 4. Создать файл 1,2 и 3 внутри каталога test1.

ADMIN@DESKTOP-CE3F84N MINGW64 ~/lesson1  
$ touch file1 file2 file3  

ADMIN@DESKTOP-CE3F84N MINGW64 ~/lesson1  
$ ^C

##### 5. Проверить содержимое каталога test1.

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

##### 8. Удалить файл 2.

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

##### 11. Переместить файлы 1 и 3 в папку lesson4.

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

##### 12. Добавить в файл 1 три строки со словами line.

ADMIN@DESKTOP-CE3F84N MINGW64 ~/lesson4  
$ echo line line line > file1

##### 13. Посмотреть содержимое файла 1.

ADMIN@DESKTOP-CE3F84N MINGW64 ~/lesson4  
$ cat file1  
line line line

##### 14. Добавьте в файл 3 три строки со словами line.

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

# Цель работы

Получение практических навыков работы в консоли с расширенными атрибутами файлов

# Выполнение работы

1. От имени пользователя guest определите расширенные атрибуты файла
/home/guest/dir1/file1 командой
lsattr /home/guest/dir1/file1
2. Установите командой
chmod 600 file1
на файл file1 права, разрешающие чтение и запись для владельца файла.
![Пункт1-2](https://github.com/dmitryabushek/study_2023_2024__infosec/blob/main/lab4/src/lab4_1.png)
3. Попробуйте установить на файл /home/guest/dir1/file1 расширенный атрибут a от имени пользователя guest:
chattr +a /home/guest/dir1/file1
В ответ вы должны получить отказ от выполнения операции. (Я не получил, но пытался)
![Пункт4-5](https://github.com/dmitryabushek/study_2023_2024__infosec/blob/main/lab4/src/lab4_2.png)
4. Зайдите на третью консоль с правами администратора либо повысьте
свои права с помощью команды su. Попробуйте установить расширенный атрибут a на файл /home/guest/dir1/file1 от имени суперпользователя:
chattr +a /home/guest/dir1/file1
5. От пользователя guest проверьте правильность установления атрибута:
lsattr /home/guest/dir1/file1
![Пункт5](https://github.com/dmitryabushek/study_2023_2024__infosec/blob/main/lab4/src/lab4_3.png)
6. Выполните дозапись в файл file1 слова «test» командой
echo "test" /home/guest/dir1/file1
После этого выполните чтение файла file1 командой
cat /home/guest/dir1/file1 
![Пункт6](https://github.com/dmitryabushek/study_2023_2024__infosec/blob/main/lab4/src/lab4_4.png)
8. Попробуйте с помощью команды
chmod 000 file1
установить на файл file1 права, например, запрещающие чтение и запись для владельца файла.(рис. @fig:002)
9. Снимите расширенный атрибут a с файла /home/guest/dirl/file1 от
имени суперпользователя командой
chattr -a /home/guest/dir1/file1
Повторите операции, которые вам ранее не удавалось выполнить. 
![Пункт9](https://github.com/dmitryabushek/study_2023_2024__infosec/blob/main/lab4/src/lab4_5.png)
10. Повторите ваши действия по шагам, заменив атрибут «a» атрибутом «i». (рис. @fig:004)
![Пункт10](https://github.com/dmitryabushek/study_2023_2024__infosec/blob/main/lab4/src/lab4_6.png)
    
# Выводы
Я получил углубленные навыки работы с linux.
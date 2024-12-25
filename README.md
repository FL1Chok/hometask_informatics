# Лабораторная работа по теме: команда grep
## Предварительные требования:

1. Основы работы с Git.
2. Установленный Git на локальной машине

### Общее описание команды grep

Команда grep (Global Regular Expression Print) используется для поиска текста в файлах. Она позволяет находить строки, соответствующие заданному шаблону. Давайте рассмотрим простой пример использования grep, разобранный по шагам.
## Введение
1. Убедитесь, что у вас есть текстовый файл для работы. Или создайте текстовый файл с именем example.txt и добавьте в него несколько строк текста. Например:
```
Hello, world!
This is a test file.
Grep is a powerful tool.
Let's find some text.
Goodbye, world!
```
<br>2.   Использование команды grep. Теперь мы можем использовать команду grep для поиска строк, содержащих определенное слово. Например, чтобы найти все строки, содержащие слово "world", выполните следующую команду:
```
grep "world" example.txt
```
После выполнения команды вы должны увидеть следующие строки:
```
Hello, world!
Goodbye, world!
```
<br>3. Использование дополнительных опций. Команда grep имеет множество опций, которые могут быть полезны. Например, если вы хотите выполнить поиск без учета регистра, используйте опцию -i:
```
grep -i "WORLD" example.txt
```
В результате вы должны увидеть те же строки, что и при обычном поиске "world".

<br>4. Поиск с использованием регулярных выражений. Команда grep поддерживает использование регулярных выражений. Попробуем найти все строки, содержащие букву "t". Используйте команду:
```
grep "t" example.txt
```
Вы должны увидеть строки:
```
This is a test file.
Grep is a powerful tool.
Let's find some text.
```
<br>5. Вывод номеров строк. Используйте опцию -n для вывода номеров строк, в которых найден текст.
```
grep -n "text" example.txt
```
Ожидаемый результат: будет выведен номер строки вместе с найденным текстом.
```
4:Let's find some text.
```
<br>6. Исключение строк: Используйте опцию -v для исключения строк, содержащих заданный шаблон.
```
grep -v "world" example.txt
```
Результат:
```
This is a test file.
Grep is a powerful tool.
Let's find some text.
```

## Задание

Теперь ваша задача — использовать команду grep с различными опциями для поиска текста в файле example.txt. При оформлении отчета, прописывать используемые команды и флаги.

1. Найдите все строки, содержащие слово "is".
2. Найдите все строки, которые не содержат слово "test".
3. Выполните поиск, который игнорирует регистр, для слова "goodbye".
4. Используйте регулярные выражения для поиска строк и их номеров, содержащих буквы "e" или "o".
5. Найдите строки с номерами, которые содержат букву "G". <br>

## Ресурсы
1. [Git Documentation](https://git-scm.com/doc)
2. [Документация по команде grep](https://man7.org/linux/man-pages/man1/grep.1.html)
3. [Примеры использования grep](https://tldp.org/LDP/abs/html/)


Эта лабораторная работа поможет вам освоить основы использования команды grep для поиска текста в файлах. Удачи!

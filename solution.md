# Лабораторная работа по теме: команда grep

## Ход работы
1. Прочитал введение, а так выполнил все шаги в нем, приступил к основному заданию.
2. Найдите все строки, содержащие слово "is". Для выполнения была использована команда `grep "is" example.txt`, в ответе получил:
```
This is a test file.
Grep is a powerful tool.
```
3. Найдите все строки, которые не содержат слово "test". Команда для выполнения -  `grep -v "test" example.txt`, ответ:
```
Hello, world!
Grep is a powerful tool.
Let's find some text.
Goodbye, world!
```
4. Выполните поиск, который игнорирует регистр, для слова "goodbye". Команда - `grep -i "goodbye" example.txt`, ответ:
```
Goodbye, world!
```
5. Выполните поиск строк, содержащих буквы "e" или "o", выполните поиск, который получит также номера этих строк. Команда - `grep -n "[eo]" example.txt`, ответ:
```
1:Hello, world!
2:This is a test file.
3:Grep is a powerful tool.
4:Let's find some text.
5:Goodbye, world!
```
6. Найдите строки с номерами, которые содержат букву "G". Команда - `grep -n "G" example.txt`, ответ:
```
3:Grep is a powerful tool.
5:Goodbye, world!
```

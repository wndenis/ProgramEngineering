# ProgramEngineering
Labs and practices

В программу подается текст из файла, состоящего из строчек формата  
`Имя Фамилия|Возраст|ТелефонныйНомер|ЭлектроннаяПочта`  
Необходимо проверить данные на корректность, и по возможности, 
исправленную версию поместить в другой файл. 
Если данные ошибочные, то часть строки оставить пустой. К примеру, из строки  
_"ИванИванов|27|+7999000 1 1 11|example@@yandex..ru"_  
может после исправления получиться строка   
_"Иван Иванов|27|+7 (999) 0001111|example@yandex.ru"_

Полный шаблон для всей строки:
#####^([^| \t\r\n]+ *[^| \t\r\n]+)\|([0-9]+)\|([\+]?[(]?([0-9]\W*){3}[)]?[-\s\.]?([0-9]\W*){3}[-\s\.]?([0-9]\W*){4,6})\|([^@ \t\r\n]+@[^@ \t\r\n]+\.[^@ \t\r\n]+)
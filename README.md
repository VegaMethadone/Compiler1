**Задание 1**
> Использовать средство синтаксического анализа по выбору, реализовать модуль для разбора текста в соответствии с языком по варианту. Реализовать построение по исходному файлу с текстом синтаксического дерева с узлами, соответствующими элементам синтаксической модели языка. Вывести полученное дерево в файл в формате, поддерживающем просмотр графического представления.

**Порядок выполнения:**

> Изучить выбранное средство синтаксического анализа
- Средство должно поддерживать программный интерфейс, совместимый с языком Си
- Средство должно параметризоваться спецификацией, описывающей синтаксическую структуру разбираемого языка
- Средство может функционировать посредством кодогенерации и/или подключения необходимых для его работы дополнительных библиотек
- Средство может быть реализовано с нуля, в этом случае оно должно использовать обобщённый алгоритм, управляемый спецификацией
> Изучить синтаксис разбираемого по варианту языка и записать спецификацию для средства синтаксического анализа, включающую следующие конструкции:
- Подпрограммы со списком аргументов и возвращаемым значением
- Операции контроля потока управления – простые ветвления if-else и циклы или аналоги
- В зависимости от варианта – определения переменных
- Целочисленные, строковые и односимвольные литералы
- Выражения численной, битовой и логической арифметики
- Выражения над одномерными массивами
- Выражения вызова функции
> Реализовать модуль, использующий средство синтаксического анализа для разбора языка по варианту
- Программный интерфейс модуля должен принимать строку с текстом и возвращать структуру, описывающую соответствующее дерево разбора и коллекцию сообщений ошибке
- Результат работы модуля – дерево разбора – должно содержать иерархическое представление для всех синтаксических конструкций, включая выражения, логически представляющие собой иерархически организованные данные, даже если на уровне средства синтаксического анализа для их разбора было использовано линейное представление
> Реализовать тестовую программу для демонстрации работоспособности созданного модуля
- Через аргументы командной строки программа должна принимать имя входного файла для чтения и анализа, имя выходного файла записи для дерева, описывающего синтаксическую структуру разобранного текста
- Сообщения об ошибке должны выводиться тестовой программной (не модулем, отвечающим за анализ!) в стандартный поток вывода ошибок
> Результаты тестирования представить в виде отчета, в который включить:
- В части 3 привести описание структур данных, представляющих результат разбора текста (3а)
- В части 4 описать, какая дополнительная обработка потребовалась для результата разбора, предоставляемого средством синтаксического анализа, чтобы сформировать результат работы созданного модуля
- В части 5 привести примеры исходных анализируемых текстов для всех синтаксических конструкций разбираемого языка и соответствующие результаты разбора

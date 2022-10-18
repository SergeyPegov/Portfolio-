A tricky cipher

Известная компания Тындекс в очередной раз проводит набор стажёров.
Заботясь о персональных данных соискателей, компания придумала хитрый алгоритм шифрования:

Подсчитывается количество различных символов в ФИО (регистр важен, А и а — разные символы).
Берётся сумма цифр в дне и месяце рождения, умноженная на 64.
Для первой (по позиции в слове) буквы фамилии определяется её номер в алфавите (в 1-индексации), умноженный на 256 (регистр буквы не важен).
Полученные числа суммируются.
Результат переводится в 16-чную систему счисления (в верхнем регистре).
У результата сохраняются только 3 младших разряда (если значимых разрядов меньше, то шифр дополняется до 3-х разрядов ведущими нулями).
Ваша задача — помочь вычислить для каждого кандидата его шифр.

Формат ввода
В первой строке вводится число N(1≤N≤10000) — количество кандидатов и шифров.
Далее следует N строк в формате CSV (fj,ij,oj,dj,mj,yj) — информация о кандидатах:

Фамилия fj, имя ij и отчество oj(1≤∣∣fj∣∣,∣∣ij∣∣,∣∣oj∣∣≤15) — строки, состоящие из латинских букв верхнего и нижнего регистра;
день рождения dj, месяц рождения mj и год рождения yj — целые числа, задающие корректную дату в промежутке от 1 января 1950 года до 31 декабря 2021 года.

Формат вывода
В единственной строке выведите N строк k1, k2, …, kN, где kj — шифр j-го кандидата (в верхнем регистре). Кандидаты нумеруются с 1 до N в порядке ввода.

____________________________________________________________________________________________________________________________________________________________

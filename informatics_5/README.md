# [A. Поиск подстроки](https://informatics.mccme.ru/mod/statements/view.php?chapterid=99#1)
*Максимальное время работы на одном тесте:	0.2 секунды*

Найти все вхождения строки $T$ в строку $S$.

### Входные данные
Первые две строки входных данных содержат строки $S$ и $T$, соответственно. Длины строк больше $0$ и меньше $50000$, строки содержат только строчные латинские буквы.
### Выходные данные
Выведите номера символов, начиная с которых строка $T$ входит в строку $S$, в порядке возрастания.
### Примеры
```
входные данные
ababbababa
aba
```
```
выходные данные
0 5 7
```

# [B. Период строки](https://informatics.mccme.ru/mod/statements/view.php?id=241&chapterid=1327#1)
Дана непустая строка $S$. Нужно найти такое наибольшее число $K$ и строку $T$, что $S$ совпадает со строкой $T$, выписанной $K$ раз подряд.

**Ограничение времени - 1 секунда.**

### Входные данные
Одна строка длины $N, 0 < N ≤ 106$, состоящая только из маленьких латинских букв.

### Выходные данные
Одно число - наибольшее возможное $K$.
### Примеры
```
входные данные
aaaaa
```
```
выходные данные
5
```

# [C. Строчки](https://informatics.mccme.ru/mod/statements/view.php?id=241&chapterid=100)
**Максимальное время работы на одном тесте:	2 секунды**

Мальчик Кирилл написал однажды на листе бумаги строчку, состоящую из больших и маленьких латинских букв, а после этого ушел играть в футбол. Когда он вернулся, то обнаружил, что его друг Дима написал под его строкой еще одну строчку такой же длины. Дима утверждает, что свою строчку он получил циклическим сдвигом строки Кирилла на несколько шагов вправо (циклический сдвиг строки *abcde* на $2$ позиции вправо даст строку *deabc*). Однако Дима известен тем, что может случайно ошибиться в большом количестве вычислений, поэтому Кирилл в растерянности – верить ли Диме? Помогите ему! По данным строкам выведите минимальный возможный размер сдвига или $-1$, если Дима ошибся.

### Входные данные
Первые две строки входных данных содержат строки Кирилла и Димы, соответственно. Длины строк одинаковы, не превышают $10000$ и не равны $0$.
### Выходные данные
Выведите единственное число – ответ  на вопрос задачи.
### Примеры
```
входные данные
zabcd
abcdz
```
```
выходные данные
4
```

# [D. Префикс-функция](https://informatics.mccme.ru/mod/statements/view.php?id=241&chapterid=1323)
Дана непустая строка $S$, длина которой $N$ не превышает $10^6$. Будем считать, что элементы строки нумеруются от $1$ до $N$.

Для каждой позиции $i$ символа в строке нас будет интересовать подстрока, заканчивающаяся в этой позиции, и совпадающая с некоторым началом всей строки. Вообще говоря, таких подстрок будет несколько, не меньше двух. Самая длинная из них имеет длину $i$, она нас интересовать не будет. А будет нас интересовать самая длинная из остальных таких подстрок (заметим, что такая подстрока всегда существует — в крайнем случае, если ничего больше не найдется, сгодится пустая подстрока).

Значением префикс-функции $π[i]$ будем считать длину этой подстроки.

Префикс-функция используется в различных алгоритмах обработки строк. В частности, с её помощью можно быстро решать задачу о поиске вхождения одной строки в другую («поиск образца в тексте»).

Требуется для всех $i$ от $1$ до $N$ вычислить $π[i]$.

### Входные данные
Одна строка длины $N, 0 < N ≤ 10^6$, состоящая из маленьких латинских букв.

### Выходные данные
Выведите $N$ чисел — значения префикс-функции для каждой позиции, разделенные пробелом.
### Примеры
```
входные данные
abracadabra
```
```
выходные данные
0 0 0 1 0 1 0 1 2 3 4
```
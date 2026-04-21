# 📘 Python для ОГЭ: Твой быстрый старт

<div align="center">

---

</div>

## 🚀 Быстрый старт: Запускаем код в PyCharm

<p>Ты открываешь книгу — значит, готов писать код. Давай сразу настроим рабочее место.</p>

**Как создать первый файл:**
<ol>
  <li>Открой PyCharm → <code>File</code> → <code>New Project</code></li>
  <li>Нажми правой кнопкой на папку проекта → <code>New</code> → <code>Python File</code></li>
  <li>Назови файл, например: <code>lesson1</code></li>
  <li>Пиши код → нажимай ▶️ <code>Run</code> или <code>Shift+F10</code></li>
</ol>

> ⚠️ **Важно:**
> <ul>
>   <li>Файлы сохраняются с расширением <code>.py</code></li>
>   <li>Код выполняется построчно, сверху вниз</li>
>   <li>Ошибки подсвечиваются красным — читай, что пишет PyCharm внизу</li>
> </ul>

💡 **Лайфхак:** Нажми <code>Tab</code> — получишь отступ. Нажми <code>Shift+Tab</code> — уберёшь. В Python отступы — это закон.

---

# УРОК 1: Введение в Python

<div style="background-color: #f0f8ff; padding: 10px; border-left: 4px solid #4169e1;">
<strong>⏱️ 60 минут</strong> • Переменные, ввод/вывод, арифметика
</div>

## 🎯 Что ты узнаешь
<ul>
  <li>Как компьютер понимает код</li>
  <li>Что такое переменная и как её назвать</li>
  <li>Как вводить данные и выводить результат</li>
  <li>Как решать задачи на цифры с помощью <code>%</code> и <code>//</code></li>
</ul>

---

## 1. Что такое программирование (0–10 мин)

<p>Компьютер понимает только нули и единицы. Писать так — нереально.</p>

**Язык программирования** — это переводчик. Ты пишешь команды на понятном языке, а компьютер превращает их в машинный код.

### Почему Python?
<table>
  <tr><td>✅</td><td>Синтаксис похож на английский</td></tr>
  <tr><td>✅</td><td>Не нужно писать лишний код для простых задач</td></tr>
  <tr><td>✅</td><td>Используется в науке, вебе, анализе данных</td></tr>
  <tr><td>✅</td><td>Идеален для задач ОГЭ №15 и №16</td></tr>
</table>

**Интерпретатор** — программа, которая выполняет твой код построчно. Написал → запустил → увидел результат. Без долгих компиляций.

---

## 2. Переменные и типы данных (10–20 мин)

**Переменная** — это именованная ячейка памяти. Ты даёшь ей имя — и кладёшь туда данные.

### 📛 Правила имён переменных
<pre style="background-color: #f5f5f5; padding: 10px; border-radius: 5px;">
✅ Можно: латинские буквы, цифры, знак _
✅ Примеры: x, score, user_name, total2
❌ Нельзя: начинать с цифры (2name — ошибка)
❌ Важно: age и Age — это разные переменные (регистр имеет значение!)
</pre>

### 🔢 Базовые типы данных
<table border="1" cellpadding="8" style="border-collapse: collapse; width: 100%;">
  <thead style="background-color: #4169e1; color: white;">
    <tr>
      <th>Тип</th>
      <th>Что хранит</th>
      <th>Примеры</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><code>int</code></td>
      <td>Целые числа</td>
      <td><code>5</code>, <code>-10</code>, <code>1000</code></td>
    </tr>
    <tr>
      <td><code>float</code></td>
      <td>Дробные числа</td>
      <td><code>3.14</code>, <code>-0.5</code>, <code>2.0</code></td>
    </tr>
    <tr>
      <td><code>str</code></td>
      <td>Текст (строки)</td>
      <td><code>"привет"</code>, <code>'123'</code>, <code>"ОГЭ 2025"</code></td>
    </tr>
  </tbody>
</table>

### 📦 Оператор присваивания `=`
<pre style="background-color: #2d2d2d; color: #f8f8f2; padding: 15px; border-radius: 5px; overflow-x: auto;">
<code>age = 15          # Записать число 15 в переменную age
name = "Анна"     # Записать текст в переменную name
score = 85 + 10   # Сначала посчитает 95, потом запишет в score</code>
</pre>

> ⚠️ **Важно:** <code>=</code> — это не математическое равенство. Это команда: «взять то, что справа, и положить в переменную слева».

---

## 3. Ввод и вывод данных (20–30 мин)

### 📤 Вывод на экран: `print()`
<pre style="background-color: #2d2d2d; color: #f8f8f2; padding: 15px; border-radius: 5px;">
<code>print("Привет, мир!")        # Выведет текст
print(42)                    # Выведет число
print("Твой балл:", score)   # Выведет текст и значение переменной</code>
</pre>

### 📥 Ввод с клавиатуры: `input()`
<pre style="background-color: #2d2d2d; color: #f8f8f2; padding: 15px; border-radius: 5px;">
<code>name = input("Как тебя зовут? ")  # Программа ждёт, пока ты введёшь текст</code>
</pre>

> ⚠️ <code>input()</code> всегда возвращает <strong>строку</strong>. Если нужно число — преобразуй его:

<pre style="background-color: #2d2d2d; color: #f8f8f2; padding: 15px; border-radius: 5px;">
<code>age = int(input("Сколько тебе лет? "))     # Целое число
price = float(input("Цена товара: "))      # Дробное число</code>
</pre>

---

## 4. Арифметические операции (30–45 мин)

<table border="1" cellpadding="8" style="border-collapse: collapse; width: 100%;">
  <thead style="background-color: #4169e1; color: white;">
    <tr>
      <th>Операция</th>
      <th>Символ</th>
      <th>Пример</th>
      <th>Результат</th>
    </tr>
  </thead>
  <tbody>
    <tr><td>Сложение</td><td><code>+</code></td><td><code>3 + 2</code></td><td><code>5</code></td></tr>
    <tr><td>Вычитание</td><td><code>-</code></td><td><code>5 - 1</code></td><td><code>4</code></td></tr>
    <tr><td>Умножение</td><td><code>*</code></td><td><code>4 * 3</code></td><td><code>12</code></td></tr>
    <tr><td>Деление</td><td><code>/</code></td><td><code>7 / 2</code></td><td><code>3.5</code></td></tr>
    <tr><td>Целочисленное деление</td><td><code>//</code></td><td><code>7 // 2</code></td><td><code>3</code></td></tr>
    <tr><td>Остаток от деления</td><td><code>%</code></td><td><code>7 % 2</code></td><td><code>1</code></td></tr>
    <tr><td>Возведение в степень</td><td><code>**</code></td><td><code>2 ** 3</code></td><td><code>8</code></td></tr>
  </tbody>
</table>

### 🧮 Примеры кода

**Пример 1. Сумма двух чисел**
<pre style="background-color: #2d2d2d; color: #f8f8f2; padding: 15px; border-radius: 5px;">
<code>a = int(input("Первое число: "))
b = int(input("Второе число: "))
print("Сумма:", a + b)</code>
</pre>

**Пример 2. Последняя цифра числа**
<pre style="background-color: #2d2d2d; color: #f8f8f2; padding: 15px; border-radius: 5px;">
<code>n = int(input("Введи число: "))
print("Последняя цифра:", n % 10)
# Почему? 123 % 10 = 3, потому что 123 = 12*10 + 3</code>
</pre>

**Пример 3. Сумма цифр двузначного числа**
<pre style="background-color: #2d2d2d; color: #f8f8f2; padding: 15px; border-radius: 5px;">
<code>n = int(input("Введи двузначное число: "))
tens = n // 10      # Десятки: 45 // 10 = 4
units = n % 10      # Единицы: 45 % 10 = 5
print("Сумма цифр:", tens + units)  # 4 + 5 = 9</code>
</pre>

---

## 💻 Практика: Реши сам (45–55 мин)

<div style="background-color: #fff3cd; padding: 10px; border-left: 4px solid #ffc107;">
<strong>🎯 Запускай PyCharm, создавай новый файл, пиши код, проверяй.</strong>
</div>

### Задание 1. Увеличь на 5
<p>Введи целое число. Выведи число, увеличенное на 5.</p>

<pre style="background-color: #2d2d2d; color: #f8f8f2; padding: 15px; border-radius: 5px;">
<code># ✅ Решение
x = int(input("Введи число: "))
print("Результат:", x + 5)</code>
</pre>

### Задание 2. Переставь цифры
<p>Введи двузначное число. Выведи число с переставленными цифрами.</p>

<pre style="background-color: #2d2d2d; color: #f8f8f2; padding: 15px; border-radius: 5px;">
<code># ✅ Решение
n = int(input("Введи двузначное число: "))
first = n // 10     # Первая цифра
second = n % 10     # Вторая цифра
print("Новое число:", second * 10 + first)
# Пример: 45 → 5*10 + 4 = 54</code>
</pre>

> 💡 **Подсказка:** Используй <code>//</code> и <code>%</code>, чтобы «разобрать» число на цифры, потом собери заново.

---

## 🏠 Домашнее задание (55–60 мин)

**Задача:** Введи трёхзначное число. Выведи сумму его цифр.

<pre style="background-color: #2d2d2d; color: #f8f8f2; padding: 15px; border-radius: 5px;">
<code># ✅ Решение
n = int(input("Введи трёхзначное число: "))
hundreds = n // 100           # Сотни
tens = (n // 10) % 10         # Десятки
units = n % 10                # Единицы
print("Сумма цифр:", hundreds + tens + units)

# Пример: 347 → 3 + 4 + 7 = 14</code>
</pre>

---

## 🧠 Мини-тест: Проверь себя (Урок 1)

<details>
<summary><strong>Вопрос 1.</strong> Что выведет этот код?</summary>
<pre style="background-color: #f5f5f5; padding: 10px;"><code>x = 10
y = 3
print(x // y, x % y)</code></pre>
<p><strong>✅ Ответ:</strong> <code>3 1</code> — потому что 10 // 3 = 3 (целая часть), 10 % 3 = 1 (остаток)</p>
</details>

<details>
<summary><strong>Вопрос 2.</strong> Как преобразовать введённую строку в целое число?</summary>
<p><strong>✅ Ответ:</strong> <code>int(input())</code></p>
</details>

<details>
<summary><strong>Вопрос 3.</strong> Какое имя переменной недопустимо в Python?</summary>
<ul>
  <li><code>user_name</code></li>
  <li><code>2fast</code></li>
  <li><code>_temp</code></li>
  <li><code>score2</code></li>
</ul>
<p><strong>✅ Ответ:</strong> <code>2fast</code> — нельзя начинать имя переменной с цифры</p>
</details>

<details>
<summary><strong>Вопрос 4.</strong> Что сделает этот код?</summary>
<pre style="background-color: #f5f5f5; padding: 10px;"><code>n = 56
print(n % 10 * 10 + n // 10)</code></pre>
<p><strong>✅ Ответ:</strong> <code>65</code> — меняет цифры местами: 56 → 65</p>
</details>

---

# УРОК 2: Условные операторы и циклы

<div style="background-color: #f0f8ff; padding: 10px; border-left: 4px solid #4169e1;">
<strong>⏱️ 60–90 минут</strong> • if, for, решение задачи №15 ОГЭ
</div>

## 🎯 Что ты узнаешь
<ul>
  <li>Как выполнять код только при определённом условии</li>
  <li>Как повторять действия без копирования кода</li>
  <li>Как решать задачу №15 ОГЭ: обработка последовательности чисел</li>
</ul>

---

## 1. Условные операторы: if, else (0–15 мин)

<p>Иногда код должен работать не всегда, а только если что-то верно.</p>

### 🔹 Базовый синтаксис
<pre style="background-color: #2d2d2d; color: #f8f8f2; padding: 15px; border-radius: 5px;">
<code>age = int(input("Сколько тебе лет? "))

if age >= 18:
    print("Ты совершеннолетний")
else:
    print("Ты ещё растёшь")</code>
</pre>

> ⚠️ **Важно:**
> <ul>
>   <li>После условия ставь двоеточие <code>:</code></li>
>   <li>Код внутри <code>if</code> или <code>else</code> пиши с отступом (нажми <code>Tab</code>)</li>
>   <li>Нет отступа = ошибка <code>IndentationError</code></li>
> </ul>

### 🔍 Операторы сравнения
<table border="1" cellpadding="8" style="border-collapse: collapse; width: 100%;">
  <thead style="background-color: #4169e1; color: white;">
    <tr>
      <th>Символ</th>
      <th>Значение</th>
      <th>Пример</th>
    </tr>
  </thead>
  <tbody>
    <tr><td><code>&gt;</code></td><td>больше</td><td><code>x &gt; 10</code></td></tr>
    <tr><td><code>&lt;</code></td><td>меньше</td><td><code>x &lt; 5</code></td></tr>
    <tr><td><code>&gt;=</code></td><td>больше или равно</td><td><code>age &gt;= 18</code></td></tr>
    <tr><td><code>&lt;=</code></td><td>меньше или равно</td><td><code>score &lt;= 100</code></td></tr>
    <tr><td><code>==</code></td><td>равно (проверка!)</td><td><code>x == 5</code></td></tr>
    <tr><td><code>!=</code></td><td>не равно</td><td><code>status != "ok"</code></td></tr>
  </tbody>
</table>

> ⚠️ Не путай: <code>=</code> — присваивание, <code>==</code> — сравнение!

### 🔹 Пример: Проверка на чётность
<pre style="background-color: #2d2d2d; color: #f8f8f2; padding: 15px; border-radius: 5px;">
<code>x = int(input("Введи число: "))

if x % 2 == 0:
    print("Число чётное")
else:
    print("Число нечётное")</code>
</pre>

### 🔹 Сложные условия: and, or
<p>Иногда нужно проверить два условия сразу.</p>

<pre style="background-color: #2d2d2d; color: #f8f8f2; padding: 15px; border-radius: 5px;">
<code># Число делится на 3 И оканчивается на 4
if x % 3 == 0 and x % 10 == 4:
    print("Подходит!")</code>
</pre>

<table border="1" cellpadding="8" style="border-collapse: collapse; width: 100%;">
  <thead style="background-color: #4169e1; color: white;">
    <tr>
      <th>Оператор</th>
      <th>Когда срабатывает</th>
      <th>Пример</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><code>and</code> (И)</td>
      <td>Когда <strong>оба</strong> условия верны</td>
      <td><code>x &gt; 0 and x &lt; 10</code></td>
    </tr>
    <tr>
      <td><code>or</code> (ИЛИ)</td>
      <td>Когда <strong>хотя бы одно</strong> условие верно</td>
      <td><code>x == 5 or x == 10</code></td>
    </tr>
  </tbody>
</table>

---

## 2. Циклы for: Повторяем без копирования (15–35 мин)

<p>Если нужно сделать одно и то же 8 раз — не пиши код 8 раз. Используй цикл.</p>

### 🔹 Синтаксис for
<pre style="background-color: #2d2d2d; color: #f8f8f2; padding: 15px; border-radius: 5px;">
<code>for i in range(5):
    print("Привет!", i)</code>
</pre>

<ul>
  <li><code>range(5)</code> — числа от 0 до 4 (всего 5 раз)</li>
  <li>Цикл выполнится ровно 5 раз</li>
  <li>Переменная <code>i</code> автоматически меняется: 0, 1, 2, 3, 4</li>
</ul>

### 🔹 Счётчик: как накопить результат
<pre style="background-color: #2d2d2d; color: #f8f8f2; padding: 15px; border-radius: 5px;">
<code>count = 0  # Создаём счётчик ДО цикла

for i in range(8):
    x = int(input("Введи число: "))
    if x % 2 == 0:  # Если чётное
        count = count + 1  # Увеличиваем счётчик

print("Чётных чисел:", count)</code>
</pre>

> 💡 **Лайфхак:** <code>count += 1</code> — это короткая запись для <code>count = count + 1</code>

---

## 💻 Разбор задачи №15 ОГЭ (35–65 мин)

### 📋 Условие
<blockquote style="border-left: 4px solid #4169e1; padding-left: 15px; margin: 20px 0;">
<strong>Введи 8 положительных целых чисел. Определи, сколько из них делятся на 3 <strong>и</strong> при этом заканчиваются на 4.</strong>
</blockquote>

### 🧭 Алгоритм шаг за шагом
<ol>
  <li>Создай переменную <code>count = 0</code> — она будет считать подходящие числа</li>
  <li>Запусти цикл на 8 повторений: <code>for i in range(8)</code></li>
  <li>Внутри цикла: введи число <code>x</code></li>
  <li>Проверь условие:
    <ul>
      <li>Делится на 3? → <code>x % 3 == 0</code></li>
      <li>Оканчивается на 4? → <code>x % 10 == 4</code></li>
      <li>Оба сразу? → <code>and</code></li>
    </ul>
  </li>
  <li>Если условие верно → <code>count += 1</code></li>
  <li>После цикла → выведи <code>count</code></li>
</ol>

### ✅ Готовый код
<pre style="background-color: #2d2d2d; color: #f8f8f2; padding: 15px; border-radius: 5px;">
<code>count = 0

for i in range(8):
    x = int(input("Введи число: "))
    if x % 3 == 0 and x % 10 == 4:
        count += 1

print("Подходящих чисел:", count)</code>
</pre>

### 🔍 Почему `x % 10` даёт последнюю цифру?
<pre style="background-color: #f5f5f5; padding: 10px;">
24 % 10 = 4   → 24 = 2*10 + 4
114 % 10 = 4  → 114 = 11*10 + 4
999 % 10 = 9  → последняя цифра 9
</pre>
<p>Остаток от деления на 10 — это всегда последняя цифра числа. Запомни этот трюк! 🎯</p>

---

## 📝 Самостоятельная работа (65–75 мин)

<div style="background-color: #fff3cd; padding: 10px; border-left: 4px solid #ffc107;">
<strong>🎯 Реши в PyCharm. Проверяй на своих данных.</strong>
</div>

### Вариант 1. Чётные числа
<p>Введи 5 чисел. Посчитай, сколько из них чётные.</p>

<pre style="background-color: #2d2d2d; color: #f8f8f2; padding: 15px; border-radius: 5px;">
<code># ✅ Решение
count = 0
for i in range(5):
    x = int(input("Число: "))
    if x % 2 == 0:
        count += 1
print("Чётных:", count)</code>
</pre>

### Вариант 2. Больше 50
<p>Введи 10 чисел. Посчитай, сколько из них больше 50.</p>

<pre style="background-color: #2d2d2d; color: #f8f8f2; padding: 15px; border-radius: 5px;">
<code># ✅ Решение
count = 0
for i in range(10):
    x = int(input("Число: "))
    if x > 50:
        count += 1
print("Больше 50:", count)</code>
</pre>

### Вариант 3. Сумма кратных 5 (сложнее)
<p>Введи 6 чисел. Посчитай сумму тех, которые делятся на 5.</p>

<pre style="background-color: #2d2d2d; color: #f8f8f2; padding: 15px; border-radius: 5px;">
<code># ✅ Решение
summa = 0
for i in range(6):
    x = int(input("Число: "))
    if x % 5 == 0:
        summa += x  # Прибавляем само число, а не +1
print("Сумма:", summa)</code>
</pre>

---

## 🏠 Домашнее задание (75–80 мин)

### 📚 Теория (ответь устно или письменно)
<ol>
  <li>Зачем в Python нужны отступы? Что будет, если их забыть?</li>
  <li>В чём разница между <code>=</code> и <code>==</code>?</li>
  <li>Что делает <code>range(5)</code>? Какие числа она генерирует?</li>
</ol>

### 💻 Практика (напиши код)

**Задача А.** Введи 3 числа. Выведи наибольшее из них.

<pre style="background-color: #2d2d2d; color: #f8f8f2; padding: 15px; border-radius: 5px;">
<code># ✅ Решение
max_num = -10**9  # Очень маленькое число для старта

for i in range(3):
    x = int(input("Число: "))
    if x > max_num:
        max_num = x

print("Наибольшее:", max_num)

# 🔁 Альтернатива с if-elif:
# a = int(input()); b = int(input()); c = int(input())
# if a >= b and a >= c:
#     print(a)
# elif b >= a and b >= c:
#     print(b)
# else:
#     print(c)</code>
</pre>

**Задача Б.** Введи 7 чисел. Посчитай количество чисел, которые кратны 7.

<pre style="background-color: #2d2d2d; color: #f8f8f2; padding: 15px; border-radius: 5px;">
<code># ✅ Решение
count = 0
for i in range(7):
    x = int(input("Число: "))
    if x % 7 == 0:
        count += 1
print("Кратных 7:", count)</code>
</pre>

---

## 🧠 Мини-тест: Проверь себя (Урок 2)

<details>
<summary><strong>Вопрос 1.</strong> Что выведет этот код?</summary>
<pre style="background-color: #f5f5f5; padding: 10px;"><code>x = 15
if x % 3 == 0 or x % 5 == 0:
    print("Да")
else:
    print("Нет")</code></pre>
<p><strong>✅ Ответ:</strong> <code>Да</code> — 15 делится и на 3, и на 5, поэтому условие <code>or</code> верно</p>
</details>

<details>
<summary><strong>Вопрос 2.</strong> Сколько раз выполнится цикл?</summary>
<pre style="background-color: #f5f5f5; padding: 10px;"><code>for i in range(3, 10):
    print(i)</code></pre>
<p><strong>✅ Ответ:</strong> <code>7 раз</code> — числа от 3 до 9 включительно (10 не входит)</p>
</details>

<details>
<summary><strong>Вопрос 3.</strong> Что не так с этим кодом?</summary>
<pre style="background-color: #f5f5f5; padding: 10px;"><code>if x = 5:
print("Пять")</code></pre>
<p><strong>✅ Ответ:</strong> Две ошибки:<br>
1. <code>=</code> вместо <code>==</code> для сравнения<br>
2. Нет отступа у <code>print</code></p>
</details>

<details>
<summary><strong>Вопрос 4.</strong> Что посчитает этот код?</summary>
<pre style="background-color: #f5f5f5; padding: 10px;"><code>s = 0
for i in range(5):
    x = int(input())
    if x > 0:
        s += x
print(s)</code></pre>
<p><strong>✅ Ответ:</strong> Сумму положительных чисел из 5 введённых</p>
</details>

---

## 🧰 Шпаргалка: Быстрый справочник

### 🔤 Переменные и ввод/вывод
<pre style="background-color: #2d2d2d; color: #f8f8f2; padding: 15px; border-radius: 5px;">
<code>name = "Твой текст"      # str
age = 15                 # int
price = 99.9             # float

print("Текст", age)      # Вывод
x = int(input())         # Ввод целого числа</code>
</pre>

### 🔢 Арифметика
<pre style="background-color: #2d2d2d; color: #f8f8f2; padding: 15px; border-radius: 5px;">
<code>a + b    # Сложение
a - b    # Вычитание
a * b    # Умножение
a / b    # Деление (всегда float)
a // b   # Целая часть от деления
a % b    # Остаток от деления
a ** b   # Возведение в степень</code>
</pre>

### 🔍 Условия
<pre style="background-color: #2d2d2d; color: #f8f8f2; padding: 15px; border-radius: 5px;">
<code>if x > 10:
    ...
elif x == 5:
    ...
else:
    ...

# Операторы: > < >= <= == !=
# Логика: and (оба), or (хотя бы один)</code>
</pre>

### 🔁 Циклы
<pre style="background-color: #2d2d2d; color: #f8f8f2; padding: 15px; border-radius: 5px;">
<code>for i in range(5):        # 0,1,2,3,4
    ...

for i in range(2, 10):    # 2,3,4,5,6,7,8,9
    ...

count = 0
for ...:
    count += 1            # Счётчик

total = 0
for ...:
    total += x            # Сумма</code>
</pre>

### 🎯 Задача №15 ОГЭ: шаблон
<pre style="background-color: #2d2d2d; color: #f8f8f2; padding: 15px; border-radius: 5px;">
<code>count = 0  # или total = 0 для суммы

for i in range(N):  # N — сколько чисел вводить
    x = int(input())
    if УСЛОВИЕ:     # например: x % 3 == 0 and x % 10 == 4
        count += 1  # или total += x

print(count)  # или print(total)</code>
</pre>

---

## 🎁 Бонус: Чек-лист перед ОГЭ

<h3>✅ Ты умеешь:</h3>
<ul>
  <li>☐ Объявлять переменные и давать им понятные имена</li>
  <li>☐ Вводить данные через <code>input()</code> и преобразовывать типы</li>
  <li>☐ Выводить результат через <code>print()</code></li>
  <li>☐ Использовать <code>//</code> и <code>%</code> для работы с цифрами числа</li>
  <li>☐ Писать условия с <code>if</code>, <code>and</code>, <code>or</code></li>
  <li>☐ Повторять действия через <code>for</code> и <code>range()</code></li>
  <li>☐ Считать количество или сумму в цикле</li>
  <li>☐ Решать задачу №15 по шаблону</li>
</ul>

<h3>✅ Ты помнишь:</h3>
<ul>
  <li>☐ Отступы в Python — обязательны</li>
  <li>☐ <code>=</code> — присвоить, <code>==</code> — сравнить</li>
  <li>☐ <code>input()</code> даёт строку → преобразуй в <code>int()</code> или <code>float()</code></li>
  <li>☐ <code>x % 10</code> — последняя цифра числа</li>
  <li>☐ <code>x // 10</code> — число без последней цифры</li>
</ul>
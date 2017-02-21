# Операційні системи
## Лабораторна робота №1 (5J)
### Задача «Постачальник – обробник - споживач»
Реалізуйте задачу по обробці інформації через  список з хх буферів обміну (наприклад, циклічний список), коли:
-	перший потік (постачальник) наповнює буфери обміну даними;
-	другий потік (обробник) перекодовує «великі» літери тексту на маленькі;
-	третій потік (споживач) записує оброблені записи даних у вихідний файл.

Коректно реалізована задача не призведе до змани тексту у вихідному файлі (по довжині, по значенню).


## Лабораторна робота №2 (2C)
### Взаємодія потоків. Паралелізм.
- Програми (процеси, потоки – згідно варіанту задачі), що реалізують функції f(x) і g(x), займаються тільки обчисленням значення над вхідним аргументом, вони не обробляють ніяких інших запитів (у тому числі – про завершення обчислень) і не взаємодіють з іншими процесами та потоками ні в який інший спосіб, окрім викликів обчислень f(x) і g(x) (тобто запуску функції на обчислення) та повернення результату (коли обчислення результату завершено).
 - Зауважити, що функції f та g – можуть бути частково визначені (тобто «зациклюватись» і ніколи не повертати результат). Потрібно коректно опрацювати таку ситуацію і запитати користувача: «продовжити обчислення, припинити або продовжити, не запитуючи більше» наприклад, кожні 10 секунд.

Обчислити f(x) && g(x), використовуючи 2 допоміжні потоки (threads): один обчислює f(x), а інший – g(x). Основна програма виконує ввод-вивід та операцію &&.

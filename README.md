МИНИСТЕРСТВО НАУКИ И ВЫСШЕГО ОБРАЗОВАНИЯ  
РОССИЙСКОЙ ФЕДЕРАЦИИ  
ФЕДЕРАЛЬНОЕ ГОСУДАРСТВЕННОЕ БЮДЖЕТНОЕ  
ОБРАЗОВАТЕЛЬНОЕ УЧРЕЖДЕНИЕ ВЫСШЕГО ОБРАЗОВАНИЯ  
«САХАЛИНСКИЙ ГОСУДАРСТВЕННЫЙ УНИВЕРСИТЕТ»  
<br><br>
Институт естественных наук и техносферной безопасности  
Кафедра информатики  
Коньков Никита Алексеевич  
<br>
Лабораторная работа №3  
**«JavaScript»**  
01.03.02 Прикладная математика и информатика  
<br><br><br><br>
Научный руководитель  
Соболев Евгений Игоревич  
<br>
Южно-Сахалинск  
2022 г.  
<br>
Введение  
<br>
HTML (или же HyperText Markup Language) - стандартизированный язык разметки документов для просмотра веб-страниц в браузере. Веб-браузеры получают HTML документ от сервера по протоколам HTTP/HTTPS или открывают с локального диска, далее интерпретируют код в интерфейс, который будет отображаться на экране монитора.  
<br>
JavaScript – мультипарадигменный язык программирования. Поддерживает объектно-ориентированный, императивный и функциональный стили. Является реализацией спецификации ECMAScript (стандарт ECMA-262). JavaScript обычно используется как встраиваемый язык для программного доступа к объектам приложений. Наиболее широкое применение находит в браузерах как язык сценариев для придания интерактивности веб-страницам.  
<br>
Цели и задачи  
1. Что выведет код ниже?  
alert( null || 2 || undefined );  
2.Что выведет код ниже?  
alert( alert(1) || 2 || alert(3) );  
3. Что выведет код ниже?  
alert( 1 && null && 2 );  
4. Что выведет alert (И)?  
alert( alert(1) && alert(2) );  
5. Что выведет этот код?  
alert( null || 2 && 3 || 4 );  
6. Напишите условие if для проверки, что переменная age находится в диапазоне между 14 и 90 включительно. «Включительно» означает, что значение переменной age может быть равно 14 или 90.  
7.Напишите условие if для проверки, что значение переменной age НЕ находится в диапазоне 14 и 90 включительно. Напишите два варианта: первый с использованием оператора НЕ !, второй – без этого оператора.  
8. Какие из перечисленных ниже alert выполнятся? Какие конкретно значения будут результатами выражений в условиях if(...)?  
if (-1 || 0) alert( 'first' );  
if (-1 && 0) alert( 'second' );  
if (null || -1 && 1) alert( 'third' );  
9. Проверка логина  
важность: 3  
Напишите код, который будет спрашивать логин с помощью prompt.  
Если посетитель вводит «Админ», то prompt запрашивает пароль, если ничего не введено или нажата клавиша Esc – показать «Отменено», в противном случае отобразить «Я вас не знаю».  
Пароль проверять так:  
Если введён пароль «Я главный», то выводить «Здравствуйте!»,  
Иначе – «Неверный пароль»,  
При отмене – «Отменено».  
Для решения используйте вложенные блоки if. Обращайте внимание на стиль и читаемость кода.  
Подсказка: передача пустого ввода в приглашение prompt возвращает пустую строку ''. Нажатие клавиши Esc во время запроса возвращает null.  
10. Какое последнее значение выведет этот код? Почему?  
let i = 3;  
while (i) {  
  alert( i-- );  
}  
11. Для каждого цикла запишите, какие значения он выведет. Потом сравните с ответом.  
Оба цикла выводят alert с одинаковыми значениями или нет?  
Префиксный вариант ++i:  
let i = 0;  
while (++i < 5) alert( i );  
Постфиксный вариант i++  
let i = 0;  
while (i++ < 5) alert( i );  
12. Для каждого цикла запишите, какие значения он выведет. Потом сравните с ответом. Оба цикла выведут alert с одинаковыми значениями или нет?  
Постфиксная форма:  
for (let i = 0; i < 5; i++) alert( i );  
Префиксная форма:  
for (let i = 0; i < 5; ++i) alert( i );  
13. При помощи цикла for выведите чётные числа от 2 до 10.  
14. Перепишите код, заменив цикл for на while, без изменения поведения цикла.  
for (let i = 0; i < 3; i++) {  
  alert( `number ${i}!` );  
}  
15. Напишите цикл, который предлагает prompt ввести число, большее 100. Если посетитель ввёл другое число – попросить ввести ещё раз, и так далее. Цикл должен спрашивать число пока либо посетитель не введёт число, большее 100, либо не нажмёт кнопку Отмена (ESC). Предполагается, что посетитель вводит только числа. Предусматривать обработку нечисловых строк в этой задаче необязательно.  
16. Натуральное число, большее 1, называется простым, если оно ни на что не делится, кроме себя и 1. Другими словами, n > 1 – простое, если при его делении на любое число кроме 1 и n есть остаток. Например, 5 — это простое число, оно не может быть разделено без остатка на 2, 3 и 4. Напишите код, который выводит все простые числа из интервала от 2 до n. Для n = 10 результат должен быть 2,3,5,7.  
17. Напишите if..else, соответствующий следующему switch:  
switch (browser) {  
  case 'Edge':  
    alert( "You've got the Edge!" );  
    break;  
  case 'Chrome':  
  case 'Firefox':  
  case 'Safari':  
  case 'Opera':  
    alert( 'Okay we support these browsers too' );  
    break;  
  default:  
    alert( 'We hope that this page looks ok!' );  
}  
18. Перепишите код с использованием одной конструкции switch:  
 const number = +prompt('Введите число между 0 и 3', '');  
if (number === 0) {  
  alert('Вы ввели число 0');  
}  
if (number === 1) {  
  alert('Вы ввели число 1');  
}  
if (number === 2 || number === 3) {  
  alert('Вы ввели число 2, а может и 3');  
}  
19. Следующая функция возвращает true, если параметр age больше 18. В ином случае она запрашивает подтверждение через confirm и возвращает его результат:  
function checkAge(age) {  
  if (age > 18) {  
    return true;  
  } else {  
    // ...  
    return confirm('Родители разрешили?');  
  }  
}  
Будет ли эта функция работать как-то иначе, если убрать else?  
function checkAge(age) {  
  if (age > 18) {  
    return true;  
  }  
  // ...  
  return confirm('Родители разрешили?');  
}  
Есть ли хоть одно отличие в поведении этого варианта?  
20. Следующая функция возвращает true, если параметр age больше 18. В ином случае она задаёт вопрос confirm и возвращает его результат.  
function checkAge(age) {  
  if (age > 18) {  
    return true;  
  } else {  
    return confirm('Родители разрешили?');  
  }  
}  
Перепишите функцию, чтобы она делала то же самое, но без if, в одну строку.  
Сделайте два варианта функции checkAge:  
Используя оператор ?  
Используя оператор ||  
21. Напишите функцию min(a,b), которая возвращает меньшее из чисел a и b.  
Пример вызовов:  
min(2, 5) == 2  
min(3, -1) == -1  
min(1, 1) == 1  
22. Напишите функцию pow(x,n), которая возвращает x в степени n. Иначе говоря, умножает x на себя n раз и возвращает результат.  
pow(3, 2) = 3 * 3 = 9  
pow(3, 3) = 3 * 3 * 3 = 27  
pow(1, 100) = 1 * 1 * ...* 1 = 1  
Создайте страницу, которая запрашивает x и n, а затем выводит результат pow(x,n).  
23. 7 kyu https://www.codewars.com/kata/highest-and-lowest  
24. 7 kyu https://www.codewars.com/kata/disemvowel-trolls  
25. 7 kyu https://www.codewars.com/kata/isograms  
26. 7 kyu https://www.codewars.com/kata/digits-explosion  
27. 6 kyu https://www.codewars.com/kata/handshake-problem  
28. 6 kyu https://www.codewars.com/kata/duplicate-encoder  
29. 6 kyu https://www.codewars.com/kata/n-th-fibonacci  
30. 6 kyu https://www.codewars.com/kata/multiples-of-3-or-5  
<br>
Решение  
<br>
Основные задачи отправлены на гит в виде .html файла  
<br>
<image src="23.jpg" alt="Задача 23">  
<image src="24.jpg" alt="Задача 24">  
<image src="25.jpg" alt="Задача 25">  
<image src="26.jpg" alt="Задача 26">  
<image src="27.jpg" alt="Задача 27">  
<image src="28.jpg" alt="Задача 28">  
<image src="29.jpg" alt="Задача 29">  
<image src="30.jpg" alt="Задача 30">  
Вывод  
<br>
Опираясь на материал с сайта w3school, формул и  иной информации с других сайтов я выполнил задачи из файла, а также познакомился с сайтом codewars, где также выполнил ряд поставленных задач

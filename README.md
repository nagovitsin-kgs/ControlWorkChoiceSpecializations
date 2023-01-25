# Дано:
## Итоговая проверочная работа
Данная работа необходима для проверки ваших знаний и навыков по итогу прохождения первого блока обучения на программе разработчик. Мы должны убедиться, что базовое знакомство с IT прошло успешно.

Задача алгоритмически не самая сложная, однако для полноценного выполнения проверочной работы необходимо:

1. Создать репозиторий на GitHub;
2. Нарисовать блок-схему алгоритма (можно обойтись блок-схемой основной содержательной части, если вы выделяете ее в отдельный метод);
3. Снабдить репозиторий оформленным текстовым описанием решения (файл README.md);
4. Написать программу, решающую поставленную задачу;
5. Использовать контроль версий в работе над этим небольшим проектом (не должно быть так, что всё залито одним коммитом, как миниммум этапы 2, 3 и 4 должны быть расположены в разных коммитах);

Задача: Написать программу, которая из имеющего массива строк,формирует массив из строк, длина которых меньше либо равна 3 символа. Первоначальный массив можно ввести с клавиатуры, либо задать на старте выполнения алгоритма. При решении не рекомендуется пользоваться коллекциями, лучше обойтись исключительно массивами.

Примеры:

"hello", "2", "world", ":-)" -> ["2", ":-)"]

["1234", "1567", "-2", "computer science"] -> ["-2"]

["Russia", "Denmark", "Kazan"] -> []

# Проект - решение:

1. Создадим новый репозиторий на GitHub, затем создадим новую папку на локальном рабочем месте. В Visual Studio Code в терминале клонируем командой git clone <ссылка из GitHub>. Затем свяжем наш локальный репозиторий с удалённым командами:

git remote add origin <https://github.com/nagovitsin-kgs/ControlWorkChoiceSpecializations.git>

git branch -M main

git push -u origin main

Добавим файл [gitignore](.gitignore).

2. Решим задачу и составим [блок-схему алгоритма](ControlTask01/01diagram.drawio.png) для составления программы (написания кода).
3. Создадим в Visual Studio Code файл [README.md](README.md) и опишем все наши действия по нашему проекту.
4. [ControlTask01](ControlTask01/Program.cs) Для того, чтобы граммотно, профессионально написать код, составим декомпозицию для решения задачи:

// 1. Создать одномерный массив из строк на старте или с клавиатуры.

// 2. Создать второй одномерный массив той же длины, что и первый.

// 3. Метод выбора значения в одномерном массиве по длине строки индекса из условия меньше либо равно 3.

// 4. Метод печати массива.

// 5. Вывод методов.

То есть перебрали по индексу i первый массив, выполнили условие <= 3, и положили по индексу j значения, согласно условия во второй массив.


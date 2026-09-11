# Лабораторная работа №1. Платформа .NET
**ФИО: Вайнбендер Артём Алексеевич**  
**Группа: ИСП-241**  
**Дата: 10.09.26**  
## 1. Краткое описание работы  
    Я изучил работу с GitHub, VS Code, терминалом и с C#
## 2. Структура проекта
    .. HelloWorld/  
        .. Program.cs/   
        .. HelloWorld.csproj/  
    .. img/  
    .. README.md/  
## 3. Примеры кода
```csharp
Console.WriteLine("Добро пожаловать в анкету!");
Console.Write("Введите ваше имя: ");
string name = Console.ReadLine();
Console.Write("Введите вашу фамилию: ");
string surname = Console.ReadLine();
Console.Write("Введите вашу группу: ");
string group = Console.ReadLine();
Console.Write("Введите ваш год рождения: ");
int birthYear = int.Parse(Console.ReadLine());
Console.Write("Введите ваш средний балл (например, 4.5): ");
double gpa = double.Parse(Console.ReadLine());
int currentYear = 2026;
int age = currentYear - birthYear;
bool isExcellent = gpa >= 4.5;
string status;
if (isExcellent == true) status = "Отличник";
else status = "Хорошист";
Console.WriteLine("Ваша анкета");
Console.WriteLine($"Имя:            {name} {surname}");
Console.WriteLine($"Группа:         {group}");
Console.WriteLine($"Возраст:        {age} лет");
Console.WriteLine($"Средний балл    {gpa}");
Console.WriteLine($"Статус:         {status}");
Console.WriteLine($"Лет до 30:      {30 - age}");
Console.WriteLine("Нажмите Enter для выхода...");
Console.ReadLine();
```
## 4. Главные выводы
    1. В С# надо прописывать тип данных переменной или var   
    2. В C# деление целых чисел (int / int) даёт целый результат
    3. В C# Для преобразования типов можно использовать Convert.ToInt32(...) или int.Parse(...) 
## 5. Итоговая таблица
|Характеристика|C# / .NET|
|--------|--------|
|Платформа  |.NET (CLR)  |
|Компиляция  |C# → IL-код → машинный код  |
|Запуск  |dotnet run  |
|Тип переменной  |Указывается явно: int x = 5;  |
|Вывод в консоль  |Console.WriteLine("текст")  |
|Ввод от пользователя  |Console.ReadLine()  |
|Интерполяция строк  |$"Привет, {name}!"  |
|Целочисленное деление  |10 / 3 = 3|
|Дробное деление  |(double)10 / 3 = 3.333...  |
|Математические функции  |Math.Abs(), Math.Pow(), и др.  |
## 6. Ответы на вопросы
    1. WriteLine() просто добавляет перенос строки в конце, а Write() нет
    2. Будет ошибка компиляции, так как ему нужно будет присвоить другой тип double
    3. Потому что оба числя являются целыми (int), для дробного числа нужно чтобы хотя бы одно любое число было дробным
    4. var это автоматическое определение типа у переменной, а в Python тип переменной спокойно изменяется
    5. Microsoft, Subnautica, Genshin Impact
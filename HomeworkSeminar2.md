//Задача 10: Напишите программу, которая принимает на вход трёхзначное число и на выходе показывает 
//вторую цифру этого числа.
//456 -> 5
//782 -> 8
//918 -> 1

Console.Clear();
Console.Write("Введите трехзначное число: ");
int num = int.Parse(Console.ReadLine()!);
int num2 = num / 10;
int result = num2 % 10;
Console.WriteLine($"{num} -> {result}");



//Задача 13: Напишите программу, которая выводит третью цифру (справа налево) заданного числа
//или сообщает, что третьей цифры нет.
//645 -> 5
//78 -> третьей цифры нет
//32679 -> 6
Console.Clear();
Console.Write("Введите число: ");
int num = int.Parse(Console.ReadLine()!);
if (num < 100)
{
    Console.WriteLine("Третьей цифры нет");
}
else
{
if (num < 1000)
{
    int res1 = num % 10;
    Console.WriteLine($"{num} -> {res1}");
}
else
{
   int res2 = 0;
    while (num > 1000)
    {
        res2 = num / 10;
    }
        Console.WriteLine($"{num} -> {res2}");

}
}



//Задача 15: Напишите программу, которая принимает на вход цифру, обозначающую день недели,
//и проверяет, является ли этот день выходным.

//6 -> да
//7 -> да
//1 -> нет

Console.Clear();
Console.Write("Введите номер дня недели ");
int num = int.Parse(Console.ReadLine()!);
if (num >= 6)
{
    Console.WriteLine($"{num} -> да");
}
else
{
    Console.WriteLine($"{num} -> нет");
}

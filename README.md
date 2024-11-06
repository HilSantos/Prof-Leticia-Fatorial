# Prof-Leticia-Fatorial
Peça ao usuario para inserir um numero inteiro positivo e, em seguida, calcule o fatorial desse numero, usando um loop for. Utilize o if para garantir que o tal numero seja positivo.

using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace FatorNumInt
{
public class Program
{
static void Main(string[] args)
{
double i, numero, fatorial;
Console.WriteLine("Informe o número");
numero = double.Parse(Console.ReadLine());

fatorial = numero;
for (i = numero - 1; i >= 1; i--)
{
Console.WriteLine($"{fatorial} * {i}");

fatorial = fatorial * i;

Console.WriteLine($"i={i}");
Console.WriteLine($"fatorial={fatorial}");
Console.WriteLine("  ");
}
Console.WriteLine($"\nFatorial de {numero} é {fatorial} ");
Console.ReadLine();
        

Console.ReadKey();
}
}
}

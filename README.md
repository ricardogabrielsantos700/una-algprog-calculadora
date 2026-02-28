# una-algprog-calculadora
resposta 1= dotnet new webapi
resposta 3= <TargetFramework>net10.0</TargetFramework>



// See https://aka.ms/new-console-template for more information
using System.Collections;

Console.WriteLine("Calculadora");
Console.WriteLine("Digite o primeiro número: ");
double num1 = Convert.ToDouble(Console.ReadLine());
Console.WriteLine("Digite o segundo número: ");
double num2 = Convert.ToDouble(Console.ReadLine());

Console.WriteLine("Escolha a operação:  ");
Console.WriteLine("1 - Adição  ");
Console.WriteLine("2 - Subtração  ");
Console.WriteLine("3 - Multiplicação");
Console.WriteLine("4 - Divisão ");

int operação = Convert.ToInt32(Console.ReadLine());

switch (operação)
{
 case 1:
 Console.WriteLine($"resultado: {num1 + num2}");
 break;
 case 2:
 Console.WriteLine($"resultado: {num1 - num2}");
 break; 
 case 3:
 Console.WriteLine($"resultado: {num1 * num2}");
 break;  
 case 4:
 if (num2 != 0)
 Console.WriteLine($"resultado: {num1 / num2}");
else
 Console.WriteLine("Erro: Divisão por zero não é permitida. ");
 break;
 default:
 Console. WriteLine("operação invalida.");
 break;
 }


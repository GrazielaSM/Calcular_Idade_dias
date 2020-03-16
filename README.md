# Calcular_Idade_dias
Calcular a idade em diasde uma pessoa.
using System;

namespace Calcular_Idade
    /*Faça um algoritmo que leia a idade de uma pessoa expressa em anos, meses e dias e escreva
     a idade dessa pessoa expressa apenas em dias.Considerar ano com 365 dias e mês com 30
     dias.*/
{
    class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("Hello!");

            const int ano = 365;
            int mes = 30;
            int dia = 12;

            Console.Write("Informe seu dia de nascimento: ");
            int dianascimento = int.Parse(Console.ReadLine());

            Console.Write("Informe seu mês de nascimento: ");
            int mesnascimento = int.Parse(Console.ReadLine());

            Console.Write("Informe seu ano de nascimento: ");
            int anonascimento = int.Parse(Console.ReadLine());


            Console.Write("Informe seu dia de atual: ");
            int mesatual = int.Parse(Console.ReadLine());

            Console.Write("Informe seu mês de atual: ");
            int diaatual = int.Parse(Console.ReadLine());

            Console.Write("Informe o ano atual: ");
            int anoatual = int.Parse(Console.ReadLine());

         
            Console.WriteLine("Você nasceu em : " + dianascimento + "/" + mesnascimento + "/" + anonascimento);

           
            int mesdia = ((mes - mesnascimento) * dia) + (dia - dianascimento);
            int idade = (anoatual - 1) - anonascimento;
            int idadedia = (idade * ano) + mesdia;
            int diasmes = (dia * mesatual) + (dia - diaatual);
            int result = idadedia + diasmes;

            Console.WriteLine("Sua idade é:" + idade + "anos");


            Console.WriteLine("Você viveu :" + result + "dias");

            Console.ReadKey();
        }
    }
}



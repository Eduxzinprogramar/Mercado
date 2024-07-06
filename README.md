using System;
using System.Runtime.Intrinsics.Arm;

namespace Projeto_do_Video
{
    internal class Program
    {
        enum MenuDeProdutos { Arroz = 1, Feijao, Picanha, Linguaca, Bacon, Aspargos, Alface, Tomate, Lasanha, Pizza, Torta, Hamburguer, Sanduiche, Tacos, BatataFrita, Sopa, Bolo, Sorvete, Geladinho, Chiclete, Bala, Caramelo, Sushi, FrutosDoMar, Lámen, SucoDeLaranja, SucoDeManga, SucoDeGraviola, SucoDeAbacaxi, Limonada }

        static void Main(string[] args)
        {

            Console.WriteLine("Seja bem-vindo ao restaurante Saboroso!");
            Console.WriteLine("Escolha o número equivalente ao seu pedido:");
            Console.WriteLine("1 - Arroz");
            Console.WriteLine("2 - Feijão");
            Console.WriteLine("3 - Picanha");
            Console.WriteLine("4 - Linguiça");
            Console.WriteLine("5 - Bacon");
            Console.WriteLine("6 - Aspargos");
            Console.WriteLine("7 - Alface");
            Console.WriteLine("8 - Tomate");
            Console.WriteLine("9 - Lasanha");
            Console.WriteLine("10 - Pizza");
            Console.WriteLine("11 - Torta");
            Console.WriteLine("12 - Hambúrguer");
            Console.WriteLine("13 - Sanduiche");
            Console.WriteLine("14 - Tacos");
            Console.WriteLine("15 - Batata Frita");
            Console.WriteLine("16 - Sopa");
            Console.WriteLine("17 - Bolo");
            Console.WriteLine("18 - Sorvete");
            Console.WriteLine("19 - Geladinho");
            Console.WriteLine("20 - Chiclete");
            Console.WriteLine("21 - Bala");
            Console.WriteLine("22 - Caramelo");
            Console.WriteLine("23 - Sushi");
            Console.WriteLine("24 - Frutos Do Mar");
            Console.WriteLine("25 - Lámen");
            Console.WriteLine("26 - Suco de Laranja");
            Console.WriteLine("27 - Suco de Manga");
            Console.WriteLine("28 - Suco de Graviola");
            Console.WriteLine("29 - Suco de Abacaxi");
            Console.WriteLine("30 - Limonada");

            int index = int.Parse(Console.ReadLine());
            MenuDeProdutos Escollha = (MenuDeProdutos)index;

            switch (Escollha)
            {
                case MenuDeProdutos.Arroz:
                    Console.WriteLine("Você pediu 1kg de Arroz!");
                    break;
                case (MenuDeProdutos.Feijao):
                    Console.WriteLine("Você pediu 1kg de Feijão!");
                    break;
                case (MenuDeProdutos.Picanha):
                    Console.WriteLine("Você pediu 1kg de Picanha!");
                    break;
                case (MenuDeProdutos.Linguaca):
                    Console.WriteLine("Você pediu 1kg de Linguiça!");
                    break;
                case (MenuDeProdutos.Bacon):
                    Console.WriteLine("Você pediu 1kg de Bacon!");
                    break;
                case (MenuDeProdutos.Aspargos):
                    Console.WriteLine("Você pediu 500g de Aspargos!");
                    break;
                case (MenuDeProdutos.Alface):
                    Console.WriteLine("Você pediu 1ª unidade de Alface!");
                    break;
                case (MenuDeProdutos.Tomate):
                    Console.WriteLine("Você pediu 500g de Tomate!");
                    break;
                case (MenuDeProdutos.Lasanha):
                    Console.WriteLine("Você pediu 200g de Lasanha!");
                    break;
                case (MenuDeProdutos.Pizza):
                    Console.WriteLine("Você pediu 1ª fatia de Pizza!");
                    break;
                    case (MenuDeProdutos.Torta):
                    Console.WriteLine("Você pediu 1ª fatia de Torta!");
                    break;
                case (MenuDeProdutos.Hamburguer):
                    Console.WriteLine("Você pediu 1 Hamburguer!");
                    break;
                case (MenuDeProdutos.Sanduiche):
                    Console.WriteLine("Você pediu 1 Sanduiche!");
                    break;
                case (MenuDeProdutos.Tacos):
                    Console.WriteLine("Você pediu 1 Taco!");
                    break;
                    case (MenuDeProdutos.BatataFrita):
                    Console.WriteLine("Você pediu 1ª porção de Batata Frita!");
                    break;
                case (MenuDeProdutos.Sopa):
                    Console.WriteLine("Você pediu 1ª Sopa!");
                    break;
                case MenuDeProdutos.Bolo:
                    Console.WriteLine("Você pediu 1ª fatia de Bolo!");
                    break;
                case MenuDeProdutos.Sorvete:
                    Console.WriteLine("Você pediu 1 Sorvete!");
                    break;
                case MenuDeProdutos.Geladinho:
                    Console.WriteLine("Você pediu 1 Geladinho!");
                    break;
                case MenuDeProdutos.Chiclete:
                    Console.WriteLine("Você pediu 1 Chiclete!");
                    break;
                case MenuDeProdutos.Bala:
                    Console.WriteLine("Você pediu 1ª Bala!");
                    break;
                case MenuDeProdutos.Caramelo:
                    Console.WriteLine("Você pediu 1 Caramelo!");
                    break;
                case MenuDeProdutos.Sushi:
                    Console.WriteLine("Você pediu uma porção de Sushi");
                    break;
                case MenuDeProdutos.FrutosDoMar:
                    Console.WriteLine("Você pediu 1ª porção de Frutos Do Mar!");
                    break;
                case MenuDeProdutos.Lámen:
                    Console.WriteLine("Você pediu 1 Lámen!");
                    break;
                    case MenuDeProdutos.SucoDeLaranja:
                    Console.WriteLine("Você pediu 1 Suco de Laranja!");
                    break;
                case MenuDeProdutos.SucoDeManga:
                    Console.WriteLine("Você pediu 1 Suco de Manga!");
                    break;
                case MenuDeProdutos.SucoDeGraviola:
                    Console.WriteLine("Você pediu 1 Suco de Graviola!");
                    break;
                    case MenuDeProdutos.SucoDeAbacaxi:
                    Console.WriteLine("Você pediu um Suco de Abacaxi!");
                    break;
                default:
                    Console.WriteLine("Este produto não está no Cardápio!");
                    break;
                case MenuDeProdutos.Limonada:
                    Console.WriteLine("Você pediu uma Limonada!");
                    break;
            }

            Console.WriteLine("Deseja fazer mais 1 pedido? (Sim/Não)");
            string resposta = Console.ReadLine();



            if (resposta == "Sim")
            {
                Main(args);
            }
            

            Console.WriteLine("Obrigado pela preferência, volte sempre!");
            Console.ReadLine();
        }          
    }
}

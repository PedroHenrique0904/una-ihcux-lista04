# una-ihcux-lista04

using System;

class Program
{
    static void Main()
    {
        Console.WriteLine("=== Sistema Robusto ===\n");

        Console.Write("Digite um número: ");

        try
        {
            int numero = int.Parse(Console.ReadLine());

            Console.WriteLine("\nNúmero digitado com sucesso!");
            Console.WriteLine($"Você digitou: {numero}");
        }
        catch (FormatException)
        {
            Console.WriteLine("\nErro: você precisa digitar um NÚMERO válido.");
            Console.WriteLine("Exemplo: 10, 25, 100...");
        }
        catch (Exception)
        {
            Console.WriteLine("\nOcorreu um erro inesperado. Tente novamente.");
        }

        Console.WriteLine("\nPressione qualquer tecla para sair...");
        Console.ReadKey();
    }
}



•	try → tenta executar o código
	•	catch → captura o erro e evita o programa quebrar
	•	int.Parse() → dá erro se não for número
	•	FormatException → erro quando digita texto

class Program
{

    static void Main(string{ } args)
{
    int[] Vetor = new int[5]; //Declaração de Vetor

//Entrada de Elementos do Vetor
    for (int i= 0; i<5; i++)
{
    Console.Write($"Digite o {i + 1}");
    Vetor[i] = int.Parse(Console.ReadLine());
}
//Variáveis para a Soma e para a Quantidade
int Soma;
int Qtde;

Soma = SomaPares(Vetor);

Qtde = ContaÍmpares(Vetor);

//Agora é só mostrar os resultados..

Console.WriteLine();

Console.WriteLine($"Soma dos Números Pares:{Soma}");
Console.WriteLine($"Quantidade de Números Ímpares:{Qtde}");

Console.Readkey();
}
//Funções 

static int SomaPares(int[]V)
{
    int S = 0; //Variável para Somar os Pares

    for (int i = 0; i < 5; i++) //Para cada elemento do Vetor...
    {
        if (V[i] % 2 == 0) //Ele é par?
            S += V{i}; //então acumula...
    }
    return S; //Retonar a Soma...
}
static int ContaÍmpares(int[]V)
{
    int Q = 0; //Variável para Contar os Ímpares

    for (int i = 0; i < V.Length; i++) //Para cada elemento do Vetor...
    {
        if (V[i] % 2 != 0) //Ele é ímpar?
            Q++; //Então conta...
    }

    return Q; // Retorna a Quantidade
}
}

![](./digital-house-header.png)

# Revisão

<details>
  <summary>Variáveis</summary>

- Identificadores são os nomes utilizados para identificar os elementos nos seus programas, como namespaces, classes, métodos e variáveis. No C#, você deve seguir as regras de sintaxe abaixo ao escolher os identificadores: 
    - Você pode utilizar apenas letras (maiúsculas ou minúsculas), dígitos e o caractere de sublinhado. 
    - Um identificador deve iniciar com uma letra (ou um sublinhado). Por exemplo, resultado, _placar, timeDeFutebol e plano9 são identificadores válidos, enquanto resultado%, timeDeFutebol$ e 9plano não são. 

- Existem 3 tipos mais comuns de variáveis; 
    - String → Usada para armazenar caracteres (textos e símbolos).
    ````c#
    string nome = "José do egito";
    ````
    - int → usada para armazenar números inteiros.
     ````c#
    int idade = 30;
    ````
    - double → usada para armazenar números reais.
     ````c#
    double altura = 1.70;
    ````
</details>

<details>
  <summary>Entrada e saída de dados</summary>

- Console
> A Console fornece suporte básico para aplicativos que leem caracteres do console e escrevem caracteres.

- Console.WriteLine
> Saída de dados no console
````c#
Console.WriteLine("Seja bem-vindo!");
````

- Console.ReadLine
> Entrada de dados no console
````c#
string nome;
Console.WriteLine("Qual seu nome?");
nome = Console.ReadLine();

string idade;
Console.WriteLine("Qual sua idade?");
idade = int.Parse(Console.ReadLine());

string altura;
Console.WriteLine("Qual sua altura?");
altura = double.Parse(Console.ReadLine());
````

> .Parse: Converte a representação de uma string de um número em seu equivalente tipo, int ou double.
</details>

<details>
  <summary>Operadores</summary>

- Adição (+)
````c#
int n1 = 2;
int n2 = 3;
int soma = n1 + n2
Console.WriteLine("A soma é" + soma); // 5
````
- Subtração (-)
````c#
int n1 = 2;
int n2 = 3;
int subtracao = n1 - n2
Console.WriteLine("A subtração é" + subtracao); // -1
````
- Multiplicação (*)
````c#
int n1 = 4;
int n2 = 3;
double multiplicacao = n1 * n2
Console.WriteLine("A multiplicação é" + multiplicacao); // 12
````
- Divisão (/)
````c#
int n1 = 4;
int n2 = 3;
double divisao = n1 / n2
Console.WriteLine("A divisão é" + divisao); // 1
````
- Resto (%)
````c#
int n1 = 4;
int n2 = 3;
double resto = n1 % n2
Console.WriteLine("O resto é" + resto); // 3
````

</details>

<details>
  <summary>Condicionais</summary>

- if 
````c#
int n1 = 4;
int n2 = 3;
if (n1 > n2) // Se a expressão for verdadeira, entra no if 
    Console.WriteLine("n1 > n2"); 
````
- if/else
````c#
int n1 = 4;
int n2 = 3;
if (n1 > n2) // Se a expressão for verdadeira, entra no if
    Console.WriteLine("n1 > n2"); 
else // se for falsa, entra no else
    Console.WriteLine("n1 < n2"); 
````
- if/else if/else
````c#
int n1 = 4;
int n2 = 4;
if (n1 > n2) {
    Console.WriteLine("n1 > n2"); 
} else if (n1 < n2) {
    Console.WriteLine("n1 < n2");
} else {
    Console.WriteLine("n1 = n2");
} 
````
- operador ternário
````c#
int n1 = 4;
int n2 = 5;
string resultado = n1 > n2 ? "n1 > n2" : "n1 < n2";
Console.WriteLine(resultado); 
````
- swicth
````c#
int opcao = 2;
swicth (opcao) {
    case 1: 
        Console.WriteLine('opção 1'); 
        break;
    case 2: 
        Console.WriteLine('opção 2'); 
        break;
    defaul:
        Console.WriteLine('opção inválida'); 
        break;
}
````
</details>

<details>
  <summary>Laço de repetição - Loop</summary>
</details>

<details>
  <summary>Array - Vetor</summary>
</details>

<details>
  <summary>Array - Matriz </summary>
</details>

<details>
  <summary>Array - Métodos </summary>
</details>
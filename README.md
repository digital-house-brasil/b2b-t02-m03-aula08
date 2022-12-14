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
    default:
        Console.WriteLine('opção inválida'); 
        break;
}
````
</details>

<details>
  <summary>Laço de repetição - Loop</summary>

- for
> É a estrutura de repetição que utilizamos quando sabemos a quantidade de repetições que um bloco de código deve ser executado

````c#
for (int i = 1; i <= 10; i++) //Vai imprimir no console a contagem de 1 a 10
  Console.WriteLine(i); 
````

- while
>  Executa o loop enquanto a condição for verdadeira. 

````c#
int i = 1;
while (i <= 10) { //Vai imprimir no console a contagem de 1 a 10
  Console.WriteLine(i);
  i++;
} 
````

- do while
> Executa o loop primeiro e depois verifica a condição.

````c#
int i = 1;
do { //Vai imprimir no console a contagem de 1 a 10
  Console.WriteLine(i);
  i++;
} while(i <= 10);
````
</details>

<details>
  <summary>Array - Vetor</summary>

- Array:
> Os arrays são estruturas que servem para guardar dados, e organizá-los. Seu objetivo é ser um espaço fixo na memória do computador que armazena elementos. Esses elementos podem ser acessados por um tipo de indicação, que chamamos de índice.

> Todo array inicia da posição 0

- Declaração de array
````c#
string semana = {"Segunda", "Terça", "Quarta", "Quinta", "Sexta", "Sábado", "Domingo"};
````

````c#
string semana = new string[] {"Segunda", "Terça", "Quarta", "Quinta", "Sexta", "Sábado", "Domingo"};
````

````c#
string semana = new string[6];
semana[0] = "Segunda";
semana[1] = "Terça";
semana[2] = "Quarta";
semana[3] = "Quinta";
semana[4] = "Sexta";
semana[5] = "Sábado";
semana[6] = "Domingo";
````

- Para acessar um valor referente ao índice do array:
````c#
Console.WriteLine(semana[3]); // Irá imprimir o valor Quinta
````

- Imprimindo todos os valores de um array
````c#
for (int i = 0; i < semana.Lenght; i++)
  Console.WriteLine(semana[i]);
````

````c#
foreach(string valor in semana)
  Console.WriteLine(valor);
````

````c#
int i = 0;
while(i < semana.Lenght) {
  Console.WriteLine(semana[i]);
  i++;
}
````

````c#
int i = 0;
do {
  Console.WriteLine(semana[i]);
  i++;
} while(i < semana.Lenght)
````

</details>

<details>
  <summary>Array - Matriz </summary>

> A matriz multidimensional pode ser declarada adicionando vírgulas entre colchetes. Por exemplo, [,] declara uma matriz bidimensional, [, ,] declara uma matriz tridimensional, [, , ,] declara uma matriz quadridimensional e assim por diante.

- Exemplo
````c#
int[,] matriz = new int[3, 3];
matriz[0, 0] = 1;
matriz[0, 1] = 1;
matriz[0, 2] = 2;

matriz[1, 0] = 8;
matriz[1, 1] = 3;
matriz[1, 2] = 1;

matriz[2, 0] = 9;
matriz[2, 1] = 9;
matriz[2, 2] = 4;

````

- Acessando o valor de um índice da matriz
````c#
Console.WriteLine(matriz[1,2]); // vai impirmir o valor 1 no console
````

- imprimindo todos os valores da matriz
````c#
for (int i = 0; i < matriz.Lenght; i++) {
    for (int j = 0; j < matriz.Lenght; j++) {
        Console.WriteLine(matriz[i, j]); 
    }
}
````

````c#
foreach(int i in matriz) {
  Console.WriteLine(i); 
}
````
</details>

# Senac

Curso Desenvolvimento de Aplicativos Móveis

Usando **DART** e **FLUTTER**

 ## Aula1 - Váriaveis

Espaço reservado em memória para armazenar um valor temporariamente

### Tipos de variaveis

- **String** - textos
- **int** - números inteiros
- **double** - números decimais

 ### Exemplo1 - Tipos de Variáveis
```
void(){
  String nome = "Brendow";
  int idade = 15;
  double altura = 1,73;
  }
  ```
  
  ### Exemplo2 - cálculo simples
  ```
  void main() {
  
  //criar variaveis para nome, sobrenome, email e ano de nascimento,
  calcular a idade e mostrar ao final uma mensagem com todos esses dados.
  
  String nome, sobrenome, email;
   nome = "Brendow";
   sobrenome = "Ribeiro";
   email = "brendowribeiro314@gmail.com";
  
  int ano_de_nascimento, idade;
  ano_de_nascimento = 2003;
  idade = 2019 - ano_de_nascimento;
  
  
  print("boa tarde $nome $sobrenome");
  print("seu email é: $email");
  print("você tem $idade anos");
  
 
  }
  ```    
  
  ## Aula 2
  
  **$(renda_pessoa.toStringAsFixed(2)}
 
 o método toStringAsFixed() foi usado para formatar as casas (2) decimais de variável(renda_pessoa) double,
 
  ```dart
  void main() {
  
  String nome, sobrenome, email, senha, cpf, endereco, sexo, celular, curso, nome_social;
  
  
  int ano_nasc, idade, qtd_moradores; 
  
 
  double renda_familiar, renda_pessoa;
  
  
  nome = "Brendow";
  sobrenome = "dos Santos Ribeiro";
  email = "brendowribeiro314@gmail.com";
  senha = "*********";
  cpf = "094.843.894-46";
  endereco = "rua dos Alfeneteiros 4";
  sexo = "masculino";
  celular = "(19)98772-7066";
  curso = "programador de Disp. Móveis";
  nome_social = "";
  
  ano_nasc = 2003;
  idade = 2019 - ano_nasc;
  qtd_moradores = 4;
  renda_familiar = 5000;
  renda_pessoa = renda_familiar / qtd_moradores;
  
  print("**************************");
  print("confirmação de cadastro");
  print("**************************");
  
  print("\nNome: $nome $sobrenome");
  if (nome_social != "")
  {
  	print("nome social: $nome_social");
  }
  print("sexo: $sexo");
  print("ano denascimento: $ano_nasc");
  print("idade: $idade");
  print("cpf: $cpf");
  print("celular: $celular");
  print("endereço: $endereco");
  
  print("\n*****************************************");
  print("confirmação de email");
  print("*****************************************");
  
  print("\nEmail: $email");
  print("Senha: $senha"); 
  
  print("\n*****************************************");
  print("informações do senac");
  print("*****************************************");
  
  print("\nquantidade de moradores: $qtd_moradores");
  print("renda familiar: R\$ ${renda_familiar.toStringAsFixed(2)}");
  print("renda por pesssoa: R\$ ${renda_pessoa.toStringAsFixed(2)}");
  print("curso: $curso");
 
  
  }
  
  ```
  
  ## Condição lógica if
  
  o if serve para determinar se um bloco de instruções **deve** ou **não** ser executado, pode-se dizer que sempre que for necessário **testar** algum valor usaremos o *if*
  
  ## Operadores lógicos
  - == *igualdade*
  - != *diferente*
  - \>= *Maior ou igual*
  - <= *Menor igual*
  - \> *Maior*
  - < *Menor*
  
  ### Sintaxe
  
  '''dart
  if(teste_logico)
  {
     //faz isso se o teste for verdadeiro
  }
  else
  {
     //faz isso se o teste for falso
  }
  
## Exemplo If

```dart
String curso = "programador android";

if(curso == "programador android")
{
   print("Parabéns, você faz ótimas escolhas.");
}
else
{
   print("Vacilão, aposto que você faz ADM.");
}   
```

## Exemplo 2

```dart
void main() {
  double nota1, nota2, media;
   nota1 = 7.3;
  	nota2 = 3.5;
 		media = (nota1 + nota2) / 2;
  
  if(media >=5)
  {
    	print("Aprovado sua média foi $media");
  }
  else
  {
    	print("Reprovado sua média foi $media");
  }
}

```

## Aula 3 - Lógica com DART

Foi importada a *biblioteca* **dart:math** para podermos usar funções matemáticas como póptência e raiz quadrada, no exemplo abaixo foi usada a função **math:sqrt()** para calcular a raiz de delta.

- Após a importação foi dado um "apelido"para chamar a função através da sintaxe **as** (dart:math as **math**)
- foram usados 2 if, 1° para dar acesso atrvés da palavra mágica SHAZAM e o 2° para fazer a equação.
- Cada if tem seu próprio else, daí a importância de *identar*, organizar o código com **TABS**

### Exemplos usando math
```dart
print(math.sqrt(9)); //exibe a raiz de nove
print(math.pi); //exibe o valor de pi 
print(math.pow(2,7)); //exibe o resultado de 2 elevado a 7.
```

### Exemplo usando If dentro de If (Login e Equação de 2º grau)

```dart
import 'dart:math' as math;
void main() {
  String palavra_magica;
 palavra_magica = "shazam"; 
  if(palavra_magica == "shazam")
 {
    print("exercício 1 - Bhaskara");  
    double delta, a, b, c;
    a = 1;
    b = -10;
    c = 25;
    delta = (b * b) - 4 * a * c ;
    print("O DELTA = $delta");
    
    if(delta < 0)
    {
      print("Nenhuma raiz real pq o delta é menor que zero");
    }
  	else
    {
     double raiz_q, x1, x2; 
      //Raiz quadrada
      raiz_q = math.sqrt(delta);
      print ("a raiz de delta = $raiz_q"); 
    	x1 = (-b + raiz_q) / (2 * a);
    	x2 = (-b - raiz_q) / (2 * a);
      print("X1 = $x1");
      print("X2 = $x2");
   } 
 } //chave do if
 else
 {
   print("acesso negado, você não é digno.");
 }
}
  
```

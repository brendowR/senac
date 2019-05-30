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
  ```
  
### Exemplo if

```dart
String curso = "programador android";

if(curso == "programador android")
{
   print("Parabéns, você faz ótimas escolhas.");
}
else
{
   print("Vacilão, aposto que você faz ADM.")
}   
```
\n = quebra de linha

# Exemplo 1 - Widget Básicos

Método principal(main) e método necessário para "inflar" o App(runApp), mostrar os widgets na tela.
Foi usado também usado o *import* no pacote/biblioteca **material.dart**, que é responsável por nos fornecer os recursos, atributos de cada
widget(cor de um objeto, tamanho, alinhamento, etc).

```dart
import 'package:flutter/material.dart';

void main() {
  runApp();
  }
  ```
  
  ## Trocar fundo de tela
  
  Foi usado um "container"(Center) e nele foi definida a cor de fundo.
  
  
  import 'package:flutter/material.dart';

```dart
void main() {
  runApp(
    new Material(
      color: Colors.lime,
    ), //Material
  );
 }
 ```
 
 ## Colocando um texto no centro da tela
 
 ```dart
import 'package:flutter/material.dart';

void main() {
  runApp(new Material(
      color: Colors.lime,
      child: Center(
        child: new Text(
          "Hello World",
          textDirection: TextDirection.ltr,
         ), //Text
       ), //Center
     ), //Material
   );
  }
  '''
  
  ## Formatando o texto:
  - tamanho do texto(font-size),
  - cor do texto(color):
  
  **style: new TextStyle(fontSize: 40,
              color: Colors.indigo),
          ),**
          
  Detalhe importante que esas propriedades são do widget Text, por isso estão dentro dos parênteses.        
          
  ```dart
  import 'package:flutter/material.dart';

void main() {
  runApp(new Material(
      color: Colors.lime,
      child: Center(
        child: new Text(
          "Hello World",
          textDirection: TextDirection.ltr,
          style: new TextStyle(fontSize: 40,
              color: Colors.indigo,
          ), //Text Style
        ), //Text
      ), //Center
    ) //Material
  ); //RunApp
}

 ```

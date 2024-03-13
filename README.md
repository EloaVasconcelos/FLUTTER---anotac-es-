# FLUTTER---anotac-es-
Somente Anotações 



Aula Pam 06/03

Instalação do Flutter (Dart Code) 

- Clicar em View
- Command Pallete 
BAIXAR: 
- Extensões (Flutter Run Doctor)
- Necessário git bash 
- Baixar SDK (CONFIGURACOES AVANÇADAS)
ADICIONAR O CAMINHO DA PASTA (SDK E JDK)

Baixar o JDK (DIRETO DO GOOGLE)
- TAMBEM É PRECISO ADICIONAR 

Variavés de ambiente 
VARIÁVEIS DE USUÁRIO
 
>PARA ABRIR NOVO PROJETO CTRL + SHITF + P
>
> SALVAR NA PASTA
>
> F5 PRA APARECER
>
>CRIAR ELEMENTOS DEPOIS
>
>@override
  Widget build(BuildContext context) {
    return const MaterialApp(
      home: Scaffold(
        body: Center(

          child: Text('Hello World!'),
          //CRIAR NOVOS ELEMENTOS (DEPOIS DO TEXT)
        ),
      ),
    );
  }
}




// TODO CÓDIGO 

/*
//CAIXA DE TEXTO 
import 'package:flutter/material.dart';


void main() {
  runApp(const MainApp());
}

class MainApp extends StatelessWidget {
  const MainApp({super.key});

  @override
  Widget build(BuildContext context) {
    return const MaterialApp(
      home: Scaffold(
        body: Center(

          child: Column(
          children:<Widget>[
            Text('hello world'),
            
          //CRIAR NOVOS ELEMENTOS (DEPOIS DO TEXT)
            Text('lallal')
          ]

          )
        ),
      ),
    );
  }
}

*/


// SLIDER
/*
import 'package:flutter/material.dart';

void main(){
  runApp(new MaterialApp(
    home: new MyApp(),
  ));
}

class MyApp extends StatefulWidget {
  @override
  _State createState() => new _State();
}

//State is information of the application that can change over time or when some actions are taken.
class _State extends State<MyApp>{

  double _value = 0.0;
  void _setvalue(double value) => setState(() => _value = value);

  @override
  Widget build(BuildContext context) {
    return new Scaffold(
      appBar: new AppBar(
        title: new Text('Escala Top'),
      ),
      //hit Ctrl+space in intellij to know what are the options you can use in flutter widgets
      body: new Container(
        padding: new EdgeInsets.all(32.0),
        child: new Center(
          child: new Column(
            children: <Widget>[
              new Text('Value: ${(_value * 100).round()}'),
              new Slider(value: _value, onChanged: _setvalue)
            ],
          ),
        ),
      ),
    );
  }
}

*/

 

 //BAR
/*
import 'package:flutter/material.dart';
import 'dart:async';

void main(){
  runApp(new MaterialApp(
    home: new MyApp(),
  ));
}

class MyApp extends StatefulWidget {
  @override
  _State createState() => new _State();
}

//State is information of the application that can change over time or when some actions are taken.
class _State extends State<MyApp>{

  int _value = 0;

  void _add() => setState(() => _value++);
  void _remove() => setState(() => _value--);

  @override
  Widget build(BuildContext context) {
    return new Scaffold(
      appBar: new AppBar(
        title: new Text('Name here'),
        backgroundColor: Colors.red,
        actions: <Widget>[
          new IconButton(icon: new Icon(Icons.add), onPressed: _add),
          new IconButton(icon: new Icon(Icons.remove), onPressed: _remove)
        ],
      ),
      //hit Ctrl+space in intellij to know what are the options you can use in flutter widgets
      body: new Container(
        padding: new EdgeInsets.all(32.0),
        child: new Center(
          child: new Column(
            children: <Widget>[
              new Text(_value.toString(), style: new TextStyle(fontWeight: FontWeight.bold, fontSize: 37.0),)
            ],
          ),
        ),
      ),
    );
  }
}
*/

// BOTÃO //
/*
import 'package:flutter/material.dart';
import 'dart:async';

void main(){
  runApp(new MaterialApp(
    home: new MyApp(),
  ));
}

class MyApp extends StatefulWidget {
  @override
  _State createState() => new _State();
}

//State is information of the application that can change over time or when some actions are taken.
class _State extends State<MyApp>{

  String _value = '';
  void _onClick(String value) => setState(() => _value = value);

  @override
  Widget build(BuildContext context) {
    return new Scaffold(
      appBar: new AppBar(
        title: new Text('Name here'),
        backgroundColor: Colors.red,
      ),
      persistentFooterButtons: <Widget>[
        new IconButton(icon: new Icon(Icons.timer), onPressed: () => _onClick('Button1')),
        new IconButton(icon: new Icon(Icons.people), onPressed: () => _onClick('Button2')),
        new IconButton(icon: new Icon(Icons.map), onPressed: () => _onClick('Button3')),
      ],
      //hit Ctrl+space in intellij to know what are the options you can use in flutter widgets
      body: new Container(
        padding: new EdgeInsets.all(32.0),
        child: new Center(
          child: new Column(
            children: <Widget>[
              new Text(_value)
            ],
          ),
        ),
      ),
    );
  }
}

*/


// CARDS 
/*import 'package:flutter/material.dart';
import 'dart:async';

void main(){
  runApp(new MaterialApp(
    home: new MyApp(),
  ));
}

class MyApp extends StatefulWidget {
  @override
  _State createState() => new _State();
}

//State is information of the application that can change over time or when some actions are taken.
class _State extends State<MyApp>{

  @override
  Widget build(BuildContext context) {
    return new Scaffold(
      appBar: new AppBar(
        title: new Text('Name here'),
        backgroundColor: Colors.red,
      ),
      //hit Ctrl+space in intellij to know what are the options you can use in flutter widgets
      body: new Container(
        padding: new EdgeInsets.all(32.0),
        child: new Center(
          child: new Column(
            children: <Widget>[
              new Card(
                child: new Container(
                  padding: new EdgeInsets.all(32.0),
                  child: new Column(
                    children: <Widget>[
                      new Text('Hello World'),
                      new Text('How are you?')
                    ],
                  ),
                ),
              ),
            
              new Card(
                child: new Container(
                  padding: new EdgeInsets.all(32.0),
                  child: new Column(
                    children: <Widget>[
                      new Text('Hello World'),
                      new Text('How are you?')
                    ],
                  ),
                ),
              ),
              
               new Card(
                child: new Container(
                  padding: new EdgeInsets.all(32.0),
                  child: new Column(
                    children: <Widget>[
                      new Text('Hello World'),
                      new Text('How are you?')
                    ],
                  ),
                ),
              )
            ],
          ),
        ),
      ),
    );
  }
}
*/



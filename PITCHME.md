![Logo](http://arquitectura.unam.mx/uploads/8/1/1/0/8110907/_2634437.png?131)
## Universidad Nacional Autónoma de México
### Facultad de Ingeniería
#### Técnicas de Programación - Ingeniería Mecatrónica

---
### Temario

- @color[gray](Importancia del software en la mecatrónica) |
- Metodología de la programación orientada a objetos |
- Desarrollo de sistemas de cómputo orientados a objetos |
- Concepto, uso y aplicaciones de las estructuras de datos compuestas |
- Interfaces gráficas de usuario |
--- 


### 2. Metodología de la programación orientada a objetos

<br>

#### Objetivo:
El alumno descubrirá los fundamentos del paradigma de programación orientado a objetos.
---

### Contenido

- Clases y objetos. Constructores, atributos y métodos |
- Encapsulación, herencia y polimorfismo |
- Sobrecarga de funciones |
- Sobrecarga de operadores |
- Manejo de errores y de excepciones |
- Arreglos y colecciones |
- Implementación de interfaces |
- Manejadores de eventos |
- Construcción de bibliotecas y reutilización de código |
- Almacenamiento, actualización y eliminación de información en base a estructuras |
- Manejo de archivos (escritura, lectura, acceso secuencial, acceso aleatorio)|

---
##### [C#]

- [Un paseo por C#](https://docs.microsoft.com/en-us/dotnet/csharp/tour-of-csharp/)
- Tipos y variables
- [Expresiones](https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/keywords/statement-keywords)

---
##### Say Hello

```
using System;

class Hello
{
    static void Main()
    {
        Console.WriteLine("Hello, World");
		Console.Read();
    }
}
```

---
##### Ejemplos Tipos y variables [int]


```
class Program
{ 
   static void Main(string[] args) 
   {
      int num=30;
      Console.Write(num);
	  Console.Read();
   }
}
```

---
##### Ejemplos Tipos y variables [double]


```
 class Program
 { 
  static void Main(string[] args) 
  {
   double num=30.33;
   Console.Write(num); 
   Console.Read();
  }
```
---
##### Ejemplos Tipos y variables [Boolean]


```
class Program
{ 
   static void Main(string[] args) 
   {
      Boolean status=true;
      Console.Write(status);
	  Console.Read();
   }
}

```

---

##### Ejemplos Tipos y variables [String]


```
class program
{
   static void Main(string[] args)
   {
      String message="Hello";
      Console.Write(message);
	  Console.Read();
   }
}

```
---

- [Instrucciones](https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/keywords/statement-keywords)

---

@fa[github fa-4x fa-spin]


-[Git / GitHub](https://www.github.com)
-[Hello World](https://guides.github.com/activities/hello-world/)
-[Cheat Sheet](https://services.github.com/on-demand/downloads/es_ES/github-git-cheat-sheet.pdf)

---
** Say hello 2 **

```
/* using keyword is used to include the System 
   namespace in the program */
using System; // 

/* A namespace is a collection of classes*/
namespace HelloWorldApplication {

   /* Classes generally contain multiple methods. 
   Methods define the behavior of the class. 
   However, the HelloWorld class has only one method Main.*/
   class HelloWorld { // class declaration. 
   
      /*Main method, which is the entry point 
	  for all C# programs*/
      static void Main(string[] args) {
	  
	     /* WriteLine is a method of the Console class 
		 defined in the System namespace. 
		 This statement causes the message 
		 "Hello, World!" to be displayed on the screen.*/
         Console.WriteLine("Hello World");

		 /*This makes the program wait for a key press 
		 and it prevents the screen from running and 
		 closing quickly*/
         Console.ReadKey(); 
      }
   }
}
```
---

### Contenido

- Clases y objetos. Constructores, atributos y métodos

---
### Class

Clase en C#

Cuando se define una clase (**class**), define un *modelo* para un tipo de datos. Esto en realidad no define ningún dato, pero define lo que significa el nombre de clase. Es decir, en qué consiste el objeto de la clase y qué operaciones se pueden realizar en ese objeto. Los objetos son instancias de una clase. Los métodos y variables que constituyen una clase se llaman miembros de la clase.

---
### Object

Objeto en C#

Un objeto es una entidad. Esto quiere decir que puede "verse" y "sentirse".
---
### Method

Método en C#

Un método define el comportamiento de los objetos de una clase.

---
*Hands on classes*

Defina las clases para los siguientes elementos

* Perro
* Coche
* Humano

---
### Constructor

Un constructor en C#

Es una miembro especial de la clase que es ejecutada cuando se crea un nuevo objeto de la clase.
Un Constructor tiene exactamente el mismo nombre que la clase que la define y no tiene ningún tipo de retorno.
Un constructor parametrizado es aquel que es utilizado para asignar valores iniciales a un objeto al tiempo de su creación.

---
*Hands on classes*

Defina los constructores para las clases previamente creadas

* Perro
* Coche
* Humano

---
### Questions?

<br>

@fa[envelope gp-contact](zmpk.fi@gmail.com)

@fa[github gp-contact](MarcoZmpk)

---
#### Encapsulación, herencia y polimorfismo

---
#### Sobrecarga de funciones

---
#### Sobrecarga de operadores

---
#### Manejo de errores y de excepciones

---
#### Arreglos y colecciones

---
#### Implementación de interfaces

---
#### Manejadores de eventos

---
#### Construcción de bibliotecas y reutilización de código

---
#### Almacenamiento, actualización y eliminación de información en base a estructuras

---
#### Manejo de archivos (escritura, lectura, acceso secuencial, acceso aleatorio)

---
### 3. Desarrollo de sistemas de cómputo orientados a objetos

<br>

#### Objetivo:
#### 

---

### 4. Concepto, uso y aplicaciones de las estructuras de datos compuestas

<br>

#### Objetivo:
#### 

---

### 5. Interfaces gráficas de usuario

<br>

#### Objetivo:
#### 
---


### Questions?

<br>

@fa[envelope gp-contact](zmpk.fi@gmail.com)

@fa[github gp-contact](MarcoZmpk)

---
#### Referencias
---

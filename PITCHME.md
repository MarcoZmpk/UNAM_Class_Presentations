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

---
### *Practica 1*

1. *Objetivos de aprendizaje* 
 
I. Objetivos generales:  Entender la diferencia entre clase y objeto. 
II. Objetivos específicos:
 
* Aprender a diseñar clases. 
* Entender el funcionamiento de los constructores. 
* Identificar los atributos y los métodos. 
* Aprender a crear objetos. 

---
#### *Encapsulación, herencia y polimorfismo*

Encapsulación

La encapsulación se define 'como el proceso de adjuntar uno o más elementos dentro de un paquete físico o lógico'. La encapsulación, en la metodología de programación orientada a objetos, impide el acceso a los detalles de implementación.

---

##### *Encapsulación*

La encapsulación es implementada utilizando *access specifiers*. 
Un *access specifier* define el alcance y la visibilidad de un miembro de la clase. C# soporta los siguiente *access specifier*

* Public
* Private
* Protected
* Internal
* Protected internal
---
##### *Encapsulación*

***Public and Private***

*Public* Es el modificador menos restrictivo. No existen restricciones para el acceso a los miembros o tipos que se hayan definido mediante public.

*Private* Los miembros privados sólo son accesibles dentro de la clase en la que se definen. Es por tanto el modificador más restrictivo.
---
##### *Encapsulación*

**Internal**

El modificador internal indica que aquellos miembros o tipos que se hayan definido con este modificador de acceso sólo serán accesibles desde los archivos del mismo ensamblado.

---
##### *Encapsulación*

**Protected and Protected Internal**

El modificador protected indica que sólo la clase en la que se ha utilizado el modificador y sus clases derivadas tendrán acceso al miembro o tipo definido como protected.
El modificador protected internal permite a la clase esconder sus variables y sus funciones de otra clase, objetos y funciones, excepto a la clase hijo de la misma aplicación.
---
##### *Herencia*

La herencia nos permite definir a una clase en términos de otra clase, lo que hace fácil crear y mantener una aplicación. Esto también provee la oportunidad de reusar funcionalidad de código y acelara el tiempo de implementación.
* Se utiliza cuando existen clases que comparten muchas de sus características
* Se extiende su funcionalidad a clases más genéricas
* Se introducen conceptos como *superclase* y *subclase*
---

```
using System;

namespace InheritanceApplication {
   class Shape {
      public void setWidth(int w) {
         width = w;
      }
      public void setHeight(int h) {
         height = h;
      }
      protected int width;
      protected int height;
   }

   // Derived class
   class Rectangle: Shape {
      public int getArea() { 
         return (width * height); 
      }
   }
   class RectangleTester {
      static void Main(string[] args) {
         Rectangle Rect = new Rectangle();

         Rect.setWidth(5);
         Rect.setHeight(7);

         // Print the area of the object.
         Console.WriteLine("Total area: {0}",  Rect.getArea());
         Console.ReadKey();
      }
   }
}
``` 

---
### *Examen 1 08/16/2018* 

---
### Questions?

<br>

@fa[envelope gp-contact](zmpk.fi@gmail.com)

@fa[github gp-contact](MarcoZmpk)


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

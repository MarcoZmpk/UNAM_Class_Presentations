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

namespace AplicacionHerencia {
   class ProbadorDeRectangulo {
      static void Main(string[] args) {
         Rectangulo Rect = new Rectangulo();

         Rect.setAncho(5);
         Rect.setAlto(7);

         // Print the area of the object.
         Console.WriteLine("Área Total: {0}",  Rect.getArea());
         Console.ReadKey();
      }
   }
   
   class Forma {
      protected int ancho;
      protected int alto;
	  
      public void setAncho(int w) {
         ancho = w;
      }
      public void setAlto(int h) {
         alto = h;
      }
   }

   // Clase derivada
   class Rectangulo: Forma {
      public int getArea() { 
         return (ancho * alto); 
      }
   }
}
``` 
---

### *Examen 1 08/16/2018* 

Desarrollar un programa en la consola de C# para realizar la suma y la divición de dos números, a partir de valores proporcionados por el usuario y mostrando los resultados correspondientes en pantalla
* El programa debe de contener el uso de clases, objetos, métodos y constructores.
* Al terminar el examen subir el programa a un repositorio personal y los resultados de las pruebas en un archivo txt a un repositorio personal llamado *Examenes*
* Enviar el link al repositorio mediante el classroom de google.
* La calificación del examen se aplicará a la práctica 0.
---

##### [Polimorfismo](http://www.itnuevolaredo.edu.mx/takeyas/Apuntes/POO/Apuntes/04.-Polimorfismo.pdf)

Es la habilidad que poseen los objetos para reaccionar de modo diferente ante los mismos mensajes.

El polimorfismo se refiere a la posibilidad de definir múltiples clases con funcionalidad diferente, pero con métodos o propiedades denominados de forma idéntica, que pueden utilizarse de manera intercambiable mediante código cliente en tiempo de ejecución.

En C# el polimorfismo está íntimamente relacionado con la sobrecarga y métodos virtuales.

---

##### Ejemplo 1

``` 
using System;

namespace PolymorphismApplication {
   class Printdata {
      void print(int i) {
         Console.WriteLine("Printing int: {0}", i );
      }
      void print(double f) {
         Console.WriteLine("Printing float: {0}" , f);
      }
      void print(string s) {
         Console.WriteLine("Printing string: {0}", s);
      }
      static void Main(string[] args) {
         Printdata p = new Printdata();
         
         // Call print to print integer
         p.print(5);
         
         // Call print to print float
         p.print(500.263);
         
         // Call print to print string
         p.print("Hello C++");
         Console.ReadKey();
      }
   }
}
``` 

---
##### Ejemplo 2

``` 
using System;

namespace PolymorphismApplication {
   abstract class Shape {
      public abstract int area();
   }
   
   class Rectangle:  Shape {
      private int length;
      private int width;
      
      public Rectangle( int a = 0, int b = 0) {
         length = a;
         width = b;
      }
      public override int area () { 
         Console.WriteLine("Rectangle class area :");
         return (width * length); 
      }
   }
   class RectangleTester {
      static void Main(string[] args) {
         Rectangle r = new Rectangle(10, 7);
         double a = r.area();
         Console.WriteLine("Area: {0}",a);
         Console.ReadKey();
      }
   }
}
``` 
---
#### Métodos, sobrecarga y sobreescritura

Creación de métodos, sobrecarga y sobreescritura.

Son procedimientos o funciones definidos dentro de una CLASE. Los métodos pueden manejar los campos de la clase incluso si son privados.

La sobrecarga es la creación dentro de la clase, de un grupo de métodos que tienen el mismo nombre pero con un número de parámetros distinto y/o bien distintos tipos de datos.
---

**Ejemplo 1**

```
public void visualización () {
  MessageBox.Show("Sr. "+Apellido+" "+Nombre+" nacido el "+FechaNac); 
}
 
public void visualización (string idioma) {
  switch (idioma) {
    case "es":  MessageBox.Show("Sr. "+Apellido+" "+Nombre+" nacido el "+FechaNac); break;
    case "en":  MessageBox.Show("Mr. "+Apellido+" "+Nombre+" was born "+FechaNac); break;
  }
}
```
---

Sabemos que las clases derivadas heredan las propiedades y métodos de su clase base. Se pueden usar sin ninguna modificación, pero sí el método no está adaptado a la nueva clase podemos sobrescribirlo. Para ello utilizamos la palabra reservada override. También es obligatorio que permitir la sobrescritura de mediante el de la palabra reservada virtual. Esto se utiliza para asegurar el polimorfismo entre las clases.

---
Ejemplo 2
```
public override void visualización () {
  MessageBox.Show("Sr. "+Apellido+" "+Nombre+" nacido el "+FechaNac+" cobra "+Salario+".-€uros/mes."); 
}
 
public sealead override void visualización () {
  base.visualizacion();
  MessageBox.Show("y cobra "+Salario+".-MXP/mes."); 
```

---
Ejemplo de método abstracto

```
  public abstract string EstadoCivil();
  //de este método no hay implementación sólo definición.
  // la clase también estará marcada como abstracta.
```

---

Métodos de extensión

Los métodos de extensión permiten añadir funcionalidades a una clase ya definida sin tener que modificar el código de esta clase. Se deben respetar las siguientes reglas:

* Pueden ser de tipo procedimientos o función. NUNCA propiedad.
* El primer parámetro irá precedido de la palabra this. La palabra clave this hace referencia a la instancia actual de la clase ,pero también se utiliza como modificador del primer parámetro de un método de extensión.
* El tipo del primer parámetro del método determina el tipo extendido por este método.
* En el momento de la ejecución, éste primer parámetro representa la instancia de la clase sobre la cual se llama el método.
* Se deben definir una clase static.
* Ellos mismos deben ser static.

```
static class ExtesionPersona {
    public static void presentacion(this Persona p) {
        Console.WriteLine("Apellido: {0}", p.apellido);
        Console.WriteLine("Nombre: {0}",p.nombre);
        Console.writeLine("Fecha de nacimiento: {0}", p.fecha_naci);
    }
}
```
---

Los métodos de extensión también también se pueden definir para los tipos básicos del Framework, como por ejemplo la clase string. El siguiente código añade a la clase string un método que permite convertir el primer carácter de una cadena en mayúsculas.

```
public static class ExtensionString
{
    public static string PrimeroMayusculas(this String s)
    {
        if ((s == null) || (s.Length == 0))
        {
            return s;
        }
        else if (s.Length == 1)
        {
 
            return s.ToUpper();
        }
        else
        {
            return s.Substring(0, 1).ToUpper() + s.Substring(1, s.Length - 1);
        }
    }
}
```
---
```
class Program
{
    static void Main(string[] args)
	{
	    Console.WriteLine(5.ElevadoALa(3));
		Console.WriteLine(7.ElevadoALa(2));
		15.Doble();
		Console.Read();
	}
	
	public static class IntegerExtensionsMethods
	{
	    public static double ElevadoALa(this int valor, int exponente)
		{
		    return Math.Pow(valor, exponente);
		}
		
		public static double Doble(this int valor)
		{
		    return valor *2;
		}
	}
}
```
---
##### [Sobrecarga de Operadores](https://docs.microsoft.com/es-es/dotnet/csharp/programming-guide/statements-expressions-operators/overloadable-operators)
```
public class Persona
{
    public Persona(double salario)
	{
	    Salario = salario;
	}
	
	public static double operator+(Persona x, Persona y)
	{
	    return x.Salario + y.Salario;
	}
	
	public double Salario {get;set;}
}

public class Program
{
    public static void Maid(string[] arg)
	{
	    Persona juan = new Persona(1000.0)
		Persona ana = new Persona(500.0)
		
		double salarioTotal = juan + ana;
		
		Console.WriteLine(salarioTotal);
		Console.Read();
	}
}

```
---

[Otros ejemplos] (https://www.tutorialesprogramacionya.com/csharpya/detalleconcepto.php?codigo=197&inicio=60)

---
### *Examen 2 08/28/2018* 

Desarrollar un programa en la consola de C# para obtener el área de un triangulo, un cuadrado y un circulo, a partir de valores proporcionados por el usuario y mostrando los resultados correspondientes en pantalla
* El programa debe de contener el uso de clases, objetos, métodos, constructores, herencia y polimorfismo.
* Al terminar el examen subir el programa a un repositorio personal y los resultados de las pruebas en un archivo txt a un repositorio personal llamado *Examenes*
* Enviar el link al repositorio mediante el classroom de google.

---
### Questions?

<br>

@fa[envelope gp-contact](zmpk.fi@gmail.com)

@fa[github gp-contact](MarcoZmpk)

---
####[Manejo de errores y de excepciones](https://www.tutorialspoint.com/csharp/csharp_exception_handling.htm)

An exception is a problem that arises during the execution of a program. A C# exception is a response to an exceptional circumstance that arises while a program is running, such as an attempt to divide by zero.

Exceptions provide a way to transfer control from one part of a program to another. C# exception handling is built upon four keywords: **try**, **catch**, **finally**, and **throw**.

---

    **try** − A try block identifies a block of code for which particular exceptions is activated. It is followed by one or more catch blocks.

    **catch** − A program catches an exception with an exception handler at the place in a program where you want to handle the problem. The catch keyword indicates the catching of an exception.

    **finally** − The finally block is used to execute a given set of statements, whether an exception is thrown or not thrown. For example, if you open a file, it must be closed whether an exception is raised or not.

    **throw** − A program throws an exception when a problem shows up. This is done using a throw keyword.

---
#####Syntax

```
try {
   // statements causing exception
} catch( ExceptionName e1 ) {
   // error handling code
} catch( ExceptionName e2 ) {
   // error handling code
} catch( ExceptionName eN ) {
   // error handling code
} finally {
   // statements to be executed
}
```

---
#####[Excepciones generadas por el compilador](https://docs.microsoft.com/es-es/dotnet/csharp/programming-guide/exceptions/compiler-generated-exceptions)

Excepción | Description
----------|------------
ArithmeticException | Una clase base para las excepciones que se producen durante las operaciones aritméticas, como DivideByZeroException y OverflowException.
ArrayTypeMismatchException | Se inicia cuando una matriz no puede almacenar un elemento determinado porque el tipo real del elemento es incompatible con el tipo real de la matriz.
DivideByZeroException | Se inicia cuando se intenta dividir un valor entero entre cero.
IndexOutOfRangeException | Se inicia cuando se intenta indexar una matriz y el índice es menor que cero o queda fuera de los límites de la matriz.
InvalidCastException | Se inicia cuando se produce un error en una conversión explícita de un tipo base en una interfaz o un tipo derivado en tiempo de ejecución.
NullReferenceException | Se inicia cuando se intenta hacer referencia a un objeto cuyo valor es null.
OutOfMemoryException | Se inicia cuando se produce un error al intentar asignar memoria con el operador new. Indica que se ha agotado la memoria disponible para el entorno Common Language Runtime.
OverflowException | Se inicia cuando se desborda una operación aritmética en un contexto checked.
StackOverflowException | Se inicia cuando se agota la pila de ejecución por tener demasiadas llamadas a métodos pendientes. Normalmente, indica una recursividad muy profunda o infinita.
TypeInitializationException | Se inicia cuando un constructor estático inicia una excepción y no existe una cláusula catch compatible para capturarla.

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

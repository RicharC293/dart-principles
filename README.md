<!-- 
  Proyecto: Fundamentos de Dart
  Autor: Richar Santiago Cangui Laica
  Descripción: Guía práctica para dar tus primeros pasos en el mundo de la programación con Dart.
  Versión: 1.0 – Octubre 2025
-->

# FUNDAMENTOS DE DART  
### Una guía práctica para dar tus primeros pasos en el mundo de la programación  
**Autor:** Richar Santiago Cangui Laica  

---

## INTRODUCCIÓN  

Aprender a programar no tiene por qué ser complicado.  
En un mundo cada vez más digital, entender cómo se crean las aplicaciones que usamos a diario puede abrirte muchas puertas: desde mejorar tu productividad hasta convertirte en parte del futuro tecnológico.  
**Dart** es un lenguaje de programación creado por Google, pensado precisamente para eso: ser fácil de entender, moderno y muy útil.  
Con Dart puedes crear aplicaciones para celulares, páginas web y programas de escritorio con una sola base de código. Es el lenguaje detrás de **Flutter**, una de las herramientas más populares para desarrollar aplicaciones móviles.  
Este folleto está diseñado para acompañarte desde cero, paso a paso, sin necesidad de tener conocimientos previos.  
Aquí aprenderás los fundamentos del lenguaje, cómo escribir tus primeras líneas de código y cómo empezar a crear tus propias ideas en la pantalla.  

<div align="center">

*“No importa tu edad, tu profesión o si nunca antes has programado: con curiosidad, paciencia y práctica, cualquiera puede aprender a programar.  
Dart es una puerta abierta al mundo del desarrollo, y este es tu primer paso para cruzarla.”*

</div>

---

## HERRAMIENTAS  

Al principio puede parecer abrumador enfrentarse a nuevas herramientas, y es completamente normal sentir dudas.  
Entender cómo funcionan es una parte esencial del aprendizaje, porque te permiten experimentar y poner en práctica todo lo que vas aprendiendo paso a paso.  
Para comenzar, no necesitas instalar programas complicados ni tener un computador potente.  
Puedes usar **DartPad**, una herramienta en línea creada por Google que te permite escribir y ejecutar código directamente desde tu navegador. Solo necesitas conexión a internet y curiosidad por probar.  
A medida que avances, descubrirás plataformas más completas como **Firebase Studio**, que te permitirán conectar tus proyectos a bases de datos, autenticación y muchas otras funciones modernas. Estas herramientas son el puente entre la teoría y la práctica, y te ayudarán a ver cómo las ideas que escribes en código se convierten en algo real.  
Cuando llegues a un nivel más avanzado, podrás instalar programas como **Visual Studio Code**, un entorno de desarrollo profesional que te permitirá practicar directamente en tu computadora y crear proyectos más grandes con total libertad. De esta forma, podrás dar el salto de los ejercicios en línea a construir aplicaciones reales, paso a paso.  

<div align="center">

*“Lo más importante no es dominar todo desde el primer día, sino atreverse a explorar, equivocarse y volver a intentarlo.  
Cada línea que escribas te acerca un poco más a convertirte en desarrollador.”*

</div>

---

## Contenido  

1. [Introducción al lenguaje y el programa “Hola Mundo”](#capitulo-1-introduccion-hola-mundo)  
2. [Tipos de datos y variables](#capitulo-2-tipos-datos-variables)  
3. [Operadores](#capitulo-3-operadores)  
4. [Estructuras de control](#capitulo-4-estructuras-control)  
5. [Funciones](#capitulo-5-funciones)  
6. [Clases y objetos](#capitulo-6-clases-objetos)  
7. [Manejo de errores y excepciones](#capitulo-7-errores-excepciones)  
8. [Programación asíncrona](#capitulo-8-programacion-asincrona)  
9. [Buenas prácticas](#capitulo-9-buenas-practicas)  
10. [Epílogo](#epilogo)  

---

<a name="capitulo-1-introduccion-hola-mundo"></a>
# 1. Introducción al lenguaje y el programa “Hola Mundo”

Dart es un lenguaje de programación moderno desarrollado por Google que combina simplicidad, potencia y flexibilidad.  
Está diseñado para ofrecer un desarrollo rápido, seguro y multiplataforma, lo que significa que puedes escribir una sola base de código y ejecutarla en dispositivos móviles, navegadores web o escritorios.  
Una de sus principales ventajas es que su sintaxis es clara y familiar para quienes provienen de lenguajes como Java, C# o JavaScript, pero también resulta accesible para principiantes, ya que evita estructuras innecesariamente complejas y promueve la legibilidad.

## 1.1. Características fundamentales de Dart

- **Multiplataforma:** permite desarrollar aplicaciones para diferentes entornos desde un mismo código fuente.  
- **Tipado estático y seguro:** el compilador verifica los tipos de datos en tiempo de compilación.  
- **Orientado a objetos:** todo en Dart es un objeto, incluso los valores más simples.  
- **Compilación eficiente:** puede compilarse a código nativo (para rendimiento) o a JavaScript (para la web).  
- **Moderno y expresivo:** su sintaxis promueve el código limpio, reutilizable y fácil de mantener.

## 1.2. Estructura básica de un programa Dart

Todo programa en Dart inicia su ejecución dentro de una función llamada `main()`. Esta función actúa como el punto de entrada del programa.  
Dentro de ella se escriben las instrucciones que se ejecutarán cuando corras el programa.

```dart
void main() {
  print('Hola Mundo');
}
```

### Análisis

- **`void`** indica que la función no devuelve ningún valor.  
- **`main()`** es la función principal del programa.  
- **`print()`** envía el texto entre comillas a la consola.  
- Las llaves `{}` delimitan el bloque de código que pertenece a la función `main()`.

Cuando este código se ejecuta, la consola mostrará:

```
Hola Mundo
```

## 1.3. Flujo de ejecución

1. Dart ejecuta la función `main()`.  
2. Dentro de ella se llama a `print('Hola Mundo')`.  
3. El texto se envía a la consola como salida.  

Este sencillo ejemplo representa el primer paso para comprender cómo se estructura un programa: cada instrucción se ejecuta de arriba hacia abajo, y los bloques de código se delimitan con llaves.  

## 1.4. Ejercicios propuestos

1. Escribe un programa que imprima tu nombre en la consola.  
2. Modifica el texto para que diga:

   ```
   ¡Hola, [tu nombre]! Bienvenido a Dart.
   ```

3. Crea un programa que imprima tres líneas: una con tu nombre, otra con tu edad y otra con tu meta al aprender programación. Intenta utilizar la función `print()` varias veces para ver el orden de ejecución.

---

<a name="capitulo-2-tipos-datos-variables"></a>
# 2. Tipos de datos y variables

Dart es un lenguaje **fuertemente tipado**. Cada dato con el que trabajas pertenece a un tipo específico, y esto le permite al compilador detectar errores en tiempo de compilación. Aunque no siempre debas declarar el tipo explícitamente, Dart lo infiere para garantizar que utilices cada valor de manera coherente.  
Además, una particularidad de Dart es que **todos los valores son objetos**: incluso los números y las cadenas tienen métodos y propiedades asociados.  

## 2.1. Tipos de datos primitivos

Los tipos más básicos que se utilizan en Dart son:

- **`int`:** números enteros positivos o negativos sin decimales.  
  Ejemplo: `int contador = 10;`  
- **`double`:** números reales con punto decimal.  
  Ejemplo: `double temperatura = 23.5;`  
- **`String`:** cadenas de texto.  
  Ejemplo: `String mensaje = 'Hola';`  
- **`bool`:** valores lógicos `true` o `false`.  
  Ejemplo: `bool activo = false;`  

Cada uno de estos tipos es un objeto con métodos. Por ejemplo, puedes convertir un número a cadena utilizando `.toString()` o comprobar si un entero es par con `.isEven`.

## 2.2. Interpolación de cadenas

Dart permite combinar variables y expresiones dentro de una cadena mediante **interpolación**.  
Existen dos formas principales:

- Usar `$variable` para insertar el valor de una variable.  
- Usar `${expresión}` para evaluar una expresión dentro de la cadena.

```dart
void main() {
  String nombre = 'María';
  int edad = 29;
  double altura = 1.70;

  print('Hola, mi nombre es $nombre y tengo $edad años.');
  print('El próximo año tendré ${edad + 1} años.');
  print('Mi altura en centímetros es aproximadamente ${altura * 100} cm.');
}
```

En este ejemplo, Dart sustituye `nombre`, `edad` y la expresión `altura * 100` por sus valores correspondientes dentro del texto.

## 2.3. Variables y constantes

Para almacenar datos en memoria utilizas **variables**. En Dart existen diferentes maneras de declararlas:

- **`var`**: permite que el compilador infiera el tipo de dato. Puede cambiar su valor.
- **`final`**: define una variable cuyo valor no puede modificarse una vez asignado. Se evalúa en tiempo de ejecución.
- **`const`**: crea una constante cuyo valor debe conocerse en tiempo de compilación.

```dart
void main() {
  var ciudad = 'Latacunga';     // tipo inferido: String
  final pais = 'Ecuador';       // no se puede modificar después
  const año = 2025;             // constante en tiempo de compilación

  ciudad = 'Quito';             // permitido
  // pais = 'Perú';             // error: final no puede reasignarse
  // año = 2026;               // error: const no puede cambiar

  print('Ciudad: $ciudad');
  print('País: $pais');
  print('Año: $año');
}
```

Es recomendable usar `final` para valores que no cambiarán y `const` para constantes definidas en tiempo de compilación.  

## 2.4. Conversión entre tipos de datos

Dart ofrece métodos para convertir entre tipos compatibles. Por ejemplo, de cadena a número y viceversa.

```dart
void main() {
  String edadTexto = '30';
  int edad = int.parse(edadTexto);     // convierte texto a entero

  double precio = 25.75;
  String precioTexto = precio.toString(); // convierte double a texto

  print('Edad (int): $edad');
  print('Precio (String): $precioTexto');
}
```

El método `int.parse()` transforma una cadena numérica en un entero. Si la cadena no representa un número válido, generará una excepción.  
El método `.toString()` convierte cualquier valor en una cadena legible.

## 2.5. Ejercicios propuestos

1. Crea variables de los tipos `int`, `double`, `String` y `bool` y muéstralas en la consola con interpolación.  
2. Escribe un programa que solicite la base y la altura de un rectángulo (puedes asignar valores directos) y calcule su área. Muestra el resultado con dos decimales.  
3. Declara una variable `edad` e imprime un mensaje que indique si una persona es mayor de edad (18 años o más) usando una estructura condicional simple.

---

<a name="capitulo-3-operadores"></a>
# 3. Operadores

Los operadores permiten realizar operaciones con valores: sumar, restar, comparar y asignar, entre otras. En Dart se dividen en varias categorías.  

## 3.1. Operadores aritméticos

Se utilizan para operaciones matemáticas básicas:

- `+` suma  
- `-` resta  
- `*` multiplicación  
- `/` división (devuelve un `double`)  
- `~/` división entera (descarta la parte decimal)  
- `%` módulo o residuo

```dart
void main() {
  int a = 10;
  int b = 3;

  print('Suma: ${a + b}');
  print('Resta: ${a - b}');
  print('Multiplicación: ${a * b}');
  print('División: ${a / b}');
  print('División entera: ${a ~/ b}');
  print('Módulo: ${a % b}');
}
```

## 3.2. Operadores relacionales y lógicos

Los operadores **relacionales** comparan dos valores y devuelven un valor booleano (`true` o `false`):

- `>` mayor que  
- `<` menor que  
- `>=` mayor o igual que  
- `<=` menor o igual que  
- `==` igual a  
- `!=` diferente de

Los operadores **lógicos** combinan o niegan valores booleanos:

- `&&` operador AND (verdadero si ambas condiciones son verdaderas).  
- `||` operador OR (verdadero si al menos una condición es verdadera).  
- `!` negación (convierte `true` en `false` y viceversa).

```dart
void main() {
  int x = 5;
  int y = 8;

  bool comparacion = (x < y) && (x != 0);
  print('Resultado lógico: $comparacion');
}
```

## 3.3. Operadores de asignación

Permiten asignar y combinar operaciones en una sola expresión:

- `=` asignación simple  
- `+=` suma y asigna  
- `-=` resta y asigna  
- `*=` multiplica y asigna  
- `/=` divide y asigna  

```dart
void main() {
  int numero = 5;
  numero += 3; // ahora vale 8
  numero *= 2; // ahora vale 16
  print(numero);
}
```

## 3.4. Precedencia y orden de evaluación

Los operadores tienen un **orden de precedencia** que determina cómo se evalúan las expresiones. La multiplicación y división tienen mayor prioridad que la suma y la resta. Los paréntesis `()` modifican el orden de evaluación.

```dart
void main() {
  int resultado1 = 2 + 3 * 4;    // primero multiplica 3*4 y luego suma 2
  int resultado2 = (2 + 3) * 4;  // primero suma y luego multiplica

  print('Resultado 1: $resultado1'); // 14
  print('Resultado 2: $resultado2'); // 20
}
```

## 3.5. Ejercicios propuestos

1. Escribe un programa que calcule el total de la factura de tres productos (precios a tu elección) y muestre el precio final.  
2. Declara dos números y utiliza operadores relacionales y lógicos para determinar si ambos son pares.  
3. Calcula el resultado de la siguiente expresión usando paréntesis para comprobar la precedencia: `8 + 2 * 5 - 3 / 2` y muestra el resultado con y sin paréntesis.

---

<a name="capitulo-4-estructuras-control"></a>
# 4. Estructuras de control

Las estructuras de control permiten dirigir el flujo de ejecución de un programa: tomar decisiones, repetir acciones y controlar cuándo finalizar ciertos procesos.

## 4.1. Condicionales `if`, `else if` y `else`

La estructura `if` evalúa una condición y ejecuta un bloque si es verdadera. Puedes añadir un bloque `else` para el caso contrario y tantos `else if` como necesites.

```dart
void main() {
  int edad = 20;

  if (edad < 13) {
    print('Eres un niño');
  } else if (edad < 18) {
    print('Eres un adolescente');
  } else {
    print('Eres un adulto');
  }
}
```

## 4.2. Operador ternario

Es una versión abreviada del `if` que se usa para asignar valores rápidos:

```dart
void main() {
  int edad = 17;
  String resultado = (edad >= 18) ? 'Mayor de edad' : 'Menor de edad';
  print(resultado);
}
```

## 4.3. Estructuras repetitivas

### 4.3.1. Bucle `for`

Se usa cuando se conoce cuántas veces se desea repetir una acción.

```dart
void main() {
  for (int i = 1; i <= 5; i++) {
    print('Iteración número $i');
  }
}
```

### 4.3.2. Bucle `while`

Se ejecuta mientras la condición sea verdadera. Es útil cuando el número de iteraciones depende de una condición externa.

```dart
void main() {
  int contador = 0;
  while (contador < 3) {
    print('Contador: $contador');
    contador++;
  }
}
```

### 4.3.3. Bucle `do-while`

A diferencia de `while`, este bucle asegura que el bloque se ejecute al menos una vez, ya que la condición se verifica al final.

```dart
void main() {
  int numero = 1;
  do {
    print('Número: $numero');
    numero++;
  } while (numero <= 3);
}
```

## 4.4. Control dentro de los bucles

Dart dispone de palabras clave para alterar la ejecución de un bucle:

- `break`: detiene el bucle inmediatamente.  
- `continue`: salta a la siguiente iteración sin ejecutar el resto del bloque.

```dart
void main() {
  for (int i = 1; i <= 5; i++) {
    if (i == 3) continue; // omite el valor 3
    if (i == 5) break;    // detiene el bucle al llegar a 5
    print('Valor: $i');
  }
}
```

## 4.5. Recorrer colecciones

### 4.5.1. Bucle `for-in`

Se utiliza para recorrer listas, conjuntos o mapas de manera simple:

```dart
void main() {
  List<String> frutas = ['Manzana', 'Banana', 'Uva'];
  for (var fruta in frutas) {
    print('Fruta: $fruta');
  }
}
```

### 4.5.2. Método `forEach()`

Ejecuta una función anónima por cada elemento de una lista:

```dart
void main() {
  List<int> numeros = [1, 2, 3];
  numeros.forEach((n) {
    print('Número: $n');
  });
}
```

### 4.5.3. Transformar colecciones con `map()`

El método `map()` aplica una función a cada elemento y devuelve una nueva colección transformada. Es útil para procesar datos sin modificar la lista original.

```dart
void main() {
  List<int> numeros = [1, 2, 3, 4, 5];
  List<int> duplicados = numeros.map((n) => n * 2).toList();
  print('Original: $numeros');
  print('Duplicados: $duplicados');
}
```

## 4.6. Sentencia `switch`

Evalúa una expresión y ejecuta el bloque que coincide con el valor. Es útil cuando se tienen varios casos posibles.

```dart
void main() {
  String dia = 'Martes';
  switch (dia) {
    case 'Lunes':
      print('Inicio de semana');
      break;
    case 'Martes':
      print('Segundo día de trabajo');
      break;
    case 'Viernes':
      print('Último día laboral');
      break;
    default:
      print('Día regular');
  }
}
```

## 4.7. Ejercicios propuestos

1. Implementa un programa que, dado un número del 1 al 7, muestre el día de la semana correspondiente utilizando `switch`.  
2. Escribe un programa que imprima todos los números pares del 1 al 20 usando un bucle `for` y la instrucción `continue` para omitir los impares.  
3. Dada una lista `[10, 20, 30, 40]`, usa `map()` para crear una nueva lista con los valores aumentados en un 15 % y muestra ambas listas.  
4. Crea una lista de nombres y utiliza `map()` para generar otra lista con la longitud de cada nombre.

---

<a name="capitulo-5-funciones"></a>
# 5. Funciones

Una función es un bloque de código reutilizable que realiza una tarea específica. Su uso permite organizar el programa, evitar duplicaciones y mejorar la legibilidad.

## 5.1. Declaración y retorno de valores

Una función se declara indicando el tipo de valor que devuelve, su nombre y los parámetros que recibe.

```dart
int sumar(int a, int b) {
  return a + b;
}

void main() {
  int resultado = sumar(5, 3);
  print('El resultado es: $resultado');
}
```

En este ejemplo, la función `sumar` recibe dos enteros y devuelve su suma. El tipo de retorno (`int`) aparece antes del nombre de la función. Cuando una función no devuelve un valor, se declara con el tipo `void`.

## 5.2. Funciones sin retorno

```dart
void saludar(String nombre) {
  print('Hola, $nombre. Bienvenido a Dart.');
}

void main() {
  saludar('María');
}
```

La función `saludar()` imprime un mensaje pero no devuelve valores, por lo que su tipo es `void`.

## 5.3. Parámetros posicionales y nombrados

En Dart, los parámetros pueden ser **posicionales** (se pasan en el orden en que se declaran) o **nombrados** (se pasan utilizando el nombre del parámetro).

### 5.3.1. Parámetros posicionales

```dart
void mostrarDatos(String nombre, int edad) {
  print('Nombre: $nombre, Edad: $edad');
}

void main() {
  mostrarDatos('Ana', 25);
}
```

### 5.3.2. Parámetros nombrados

Los parámetros nombrados se definen entre llaves y se pueden marcar como `required`.

```dart
void registrarUsuario({required String nombre, int edad = 18}) {
  print('Usuario: $nombre, Edad: $edad');
}

void main() {
  registrarUsuario(nombre: 'Carlos');
  registrarUsuario(nombre: 'Lucía', edad: 30);
}
```

Los parámetros con valores por defecto (como `edad = 18`) se utilizan cuando no se proporciona un valor en la llamada.

## 5.4. Parámetros opcionales y valores por defecto

Los parámetros opcionales posicionales se declaran entre corchetes `[]`.

```dart
void saludar([String nombre = 'invitado']) {
  print('Hola, $nombre');
}

void main() {
  saludar();        // Hola, invitado
  saludar('María'); // Hola, María
}
```

También pueden combinarse parámetros opcionales y nombrados para mejorar la legibilidad.

## 5.5. Funciones anónimas y flecha

Una función anónima no tiene nombre y se utiliza generalmente como argumento de otra función.

```dart
void main() {
  List<String> frutas = ['Manzana', 'Banana', 'Uva'];
  frutas.forEach((fruta) {
    print('Fruta: $fruta');
  });
}
```

Las **funciones flecha** (`=>`) son una forma abreviada de escribir funciones que contienen una sola expresión.

```dart
int cuadrado(int n) => n * n;

void main() {
  print(cuadrado(4)); // 16
}
```

## 5.6. Funciones como valores (callbacks)

En Dart, las funciones son valores de primera clase: se pueden asignar a variables, pasar como parámetros y devolver desde otras funciones. Cuando se pasa una función como parámetro a otra función para que la ejecute más tarde, se denomina **callback**.

```dart
int sumar(int a, int b) => a + b;

void ejecutarOperacion(int Function(int, int) operacion, int x, int y) {
  print('Resultado: ${operacion(x, y)}');
}

void main() {
  ejecutarOperacion(sumar, 5, 3);                // usa la función sumar
  ejecutarOperacion((a, b) => a * b, 4, 2);      // usa un callback anónimo
}
```

Aquí, la función `ejecutarOperacion` recibe otra función (`operacion`) y la ejecuta con los valores indicados. Este patrón es común en programación asíncrona y en bibliotecas como Flutter para manejar eventos.

## 5.7. Ámbito de variables (scope)

El ámbito determina dónde es visible una variable.  

```dart
int contadorGlobal = 0;

void incrementar() {
  int contadorLocal = 10;
  contadorGlobal++;
  print('Contador local: $contadorLocal');
}

void main() {
  incrementar();
  incrementar();
  print('Contador global: $contadorGlobal');
}
```

- `contadorLocal` solo existe dentro de la función `incrementar()`.  
- `contadorGlobal` es accesible en cualquier parte del archivo.  
- Mantener los ámbitos claros evita colisiones de nombres y hace el código más legible.

## 5.8. Ejercicios propuestos

1. Crea una función que reciba dos números y devuelva su promedio. Llámala desde `main()` e imprime el resultado.  
2. Escribe una función que reciba una lista de nombres y los imprima en mayúsculas utilizando `forEach()` y una función anónima.  
3. Implementa una función `convertirDolaresAEuros()` que reciba un valor en dólares y retorne su equivalente en euros, usando un valor fijo para el tipo de cambio.  
4. Declara una función llamada `evaluarEdad` que reciba una edad como parámetro y use un operador ternario para devolver “Mayor de edad” o “Menor de edad”.  
5. Escribe una función `aplicarOperacion` que reciba otra función como parámetro y la aplique a dos valores enteros. Prueba pasarle una función de suma y otra de multiplicación.

---

<a name="capitulo-6-clases-objetos"></a>
# 6. Clases y objetos

La **programación orientada a objetos (POO)** organiza el código en torno a **objetos**, que combinan datos (atributos) y comportamientos (métodos). Dart es un lenguaje orientado a objetos: todo valor es una instancia de una clase.  

## 6.1. ¿Qué es una clase y qué es un objeto?

Una **clase** define un conjunto de características y comportamientos comunes. Es como un plano o plantilla.  
Un **objeto** es una instancia concreta de esa clase, con valores propios para cada atributo.  
Por ejemplo, si tenemos una clase `Animal` que describe a los animales, un perro o un gato serán objetos específicos de esa clase.

## 6.2. Atributos y métodos

Los **atributos** son variables que representan las características de un objeto.  
Los **métodos** son funciones asociadas a la clase, que definen las acciones que un objeto puede realizar.

```dart
class Animal {
  String nombre = '';
  int edad = 0;

  void comer() {
    print('$nombre está comiendo.');
  }

  void dormir() {
    print('$nombre está durmiendo.');
  }
}

void main() {
  Animal perro = Animal();
  perro.nombre = 'Firulais';
  perro.edad = 5;

  perro.comer();
  perro.dormir();
}
```

En este ejemplo, `nombre` y `edad` son atributos, y `comer()` y `dormir()` son métodos. Cada objeto de la clase `Animal` tendrá sus propios valores para los atributos.

## 6.3. Constructores

Un **constructor** es un método especial que se ejecuta al crear un objeto y se utiliza para inicializar sus atributos. Existen constructores con parámetros posicionales y nombrados.

### 6.3.1. Constructor con parámetros posicionales

```dart
class Animal {
  String nombre;
  int edad;
  String tipo;

  Animal(this.nombre, this.edad, this.tipo);

  void mostrarInfo() {
    print('Soy un $tipo llamado $nombre y tengo $edad años.');
  }
}

void main() {
  Animal gato = Animal('Misu', 3, 'Gato');
  gato.mostrarInfo();
}
```

### 6.3.2. Constructor con parámetros nombrados

```dart
class Animal {
  String nombre;
  int edad;
  String tipo;

  Animal({required this.nombre, required this.edad, required this.tipo});

  void mostrarInfo() {
    print('Soy un $tipo llamado $nombre y tengo $edad años.');
  }
}

void main() {
  Animal ave = Animal(nombre: 'Loro', edad: 2, tipo: 'Ave');
  ave.mostrarInfo();
}
```

Los constructores nombrados permiten especificar el valor de cada atributo usando su nombre, lo que mejora la legibilidad cuando hay muchos parámetros.

## 6.4. Encapsulamiento, getters y setters

El **encapsulamiento** protege los datos de una clase para que no se modifiquen de manera inapropiada desde fuera de ella.  
En Dart, los nombres que comienzan con `_` son privados para el archivo en el que se encuentran. Puedes definir **getters** y **setters** para acceder y modificar esos valores de forma controlada.

```dart
class Persona {
  String _nombre;
  int _edad;

  Persona(this._nombre, this._edad);

  // Getter
  String get nombre => _nombre;

  // Setter
  set edad(int nuevaEdad) {
    if (nuevaEdad >= 0) {
      _edad = nuevaEdad;
    } else {
      print('La edad no puede ser negativa.');
    }
  }

  void presentarse() {
    print('Soy $_nombre y tengo $_edad años.');
  }
}

void main() {
  Persona p = Persona('Ana', 28);
  p.presentarse();
  p.edad = 30;       // usa el setter
  p.presentarse();
  p.edad = -5;      // intento inválido
}
```

## 6.5. Herencia y clases derivadas

La **herencia** permite crear nuevas clases basadas en otra clase existente. La clase base se denomina **superclase**, y la clase que hereda se llama **subclase**.  
Las subclases heredan los atributos y métodos de la superclase, pero también pueden agregar nuevos comportamientos o sobrescribir métodos existentes.

### 6.5.1. Ejemplo de herencia con animales

```dart
class Animal {
  String nombre;
  int edad;

  Animal(this.nombre, this.edad);

  void moverse() {
    print('$nombre se está moviendo.');
  }
}

class AnimalTerrestre extends Animal {
  AnimalTerrestre(String nombre, int edad) : super(nombre, edad);

  void caminar() {
    print('$nombre camina sobre la tierra.');
  }
}

class AnimalAcuatico extends Animal {
  AnimalAcuatico(String nombre, int edad) : super(nombre, edad);

  void nadar() {
    print('$nombre nada en el agua.');
  }
}

class AnimalAereo extends Animal {
  AnimalAereo(String nombre, int edad) : super(nombre, edad);

  void volar() {
    print('$nombre vuela por el aire.');
  }
}

void main() {
  AnimalTerrestre perro = AnimalTerrestre('Firulais', 5);
  perro.moverse();
  perro.caminar();

  AnimalAcuatico pez = AnimalAcuatico('Nemo', 1);
  pez.moverse();
  pez.nadar();

  AnimalAereo aguila = AnimalAereo('Águila Real', 4);
  aguila.moverse();
  aguila.volar();
}
```

### 6.5.2. Sobrescritura de métodos

Las subclases pueden redefinir un método heredado para personalizar su comportamiento. Para ello se usa la anotación `@override`.

```dart
class Animal {
  String nombre;
  Animal(this.nombre);

  void moverse() {
    print('$nombre se mueve.');
  }
}

class Pez extends Animal {
  Pez(String nombre) : super(nombre);

  @override
  void moverse() {
    print('$nombre nada rápidamente.');
  }
}

void main() {
  Pez pez = Pez('Dory');
  pez.moverse();
}
```

## 6.6. Ejercicios propuestos

1. Crea una clase `Libro` con los atributos `titulo`, `autor` y `anioPublicacion`. Agrega un método que imprima esta información.  
2. Define una clase `Empleado` con los atributos `nombre`, `cargo` y `salario`. Crea una subclase `Vendedor` que añada el atributo `comision` y sobrescriba un método para calcular el salario total.  
3. Implementa una clase `CuentaBancaria` con métodos `depositar()` y `retirar()`. Usa encapsulamiento para proteger el saldo y crea getters para consultarlo.  
4. Define una clase `Vehiculo` y una subclase `Motocicleta`. La subclase debe heredar los atributos de `Vehiculo` y añadir uno propio (`cilindraje`). Implementa un método que muestre toda la información.

---

<a name="capitulo-7-errores-excepciones"></a>
# 7. Manejo de errores y excepciones

En un programa pueden ocurrir situaciones inesperadas, como intentar acceder a un índice fuera de una lista o convertir un texto no numérico en un número.  
Estas situaciones se llaman **excepciones**, y manejarías sus errores permite que el programa no se detenga abruptamente.  
Dart proporciona estructuras como `try`, `catch`, `on`, `finally` y `throw` para capturar y controlar estos eventos.

## 7.1. Captura básica con `try` y `catch`

El bloque `try` contiene el código que podría generar una excepción. Si ocurre un error, el bloque `catch` lo captura.

```dart
void main() {
  try {
    int resultado = 10 ~/ 0; // división entera entre cero
    print('Resultado: $resultado');
  } catch (e) {
    print('Ocurrió una excepción: $e');
  }

  print('El programa continúa ejecutándose.');
}
```

En este ejemplo, la división entera entre cero con `~/` lanza la excepción `IntegerDivisionByZeroException`.  
Al capturarla con `catch`, el programa evita interrumpirse y continúa su ejecución.

> **Nota:** La división normal (`/`) con cero en Dart no lanza una excepción; devuelve `Infinity`, `-Infinity` o `NaN` según el caso. La división entera (`~/`) sí genera la excepción.

## 7.2. Uso de `on` y tipos específicos

Puedes capturar excepciones específicas usando la sentencia `on`.

```dart
void main() {
  try {
    var lista = [1, 2, 3];
    print(lista[5]); // acceso fuera de rango
  } on RangeError catch (e) {
    print('Error de rango: ${e.message}');
  } catch (e) {
    print('Ocurrió una excepción general: $e');
  }

  print('El programa no se detuvo.');
}
```

## 7.3. Trazas de pila (stack trace)

Puedes obtener información detallada sobre dónde ocurrió la excepción capturando el **stack trace**.

```dart
void main() {
  try {
    int valor = int.parse('abc'); // conversión inválida
  } catch (e, stackTrace) {
    print('Error: $e');
    print('Detalles del error:\n$stackTrace');
  }
}
```

El segundo parámetro de `catch` almacena la traza de ejecución, útil para depurar.

## 7.4. Bloque `finally`

El bloque `finally` se ejecuta siempre, ocurra o no una excepción. Se utiliza para liberar recursos, cerrar conexiones o mostrar mensajes finales.

```dart
void main() {
  try {
    int resultado = 100 ~/ 2;
    print('Resultado: $resultado');
  } catch (e) {
    print('Ocurrió un error: $e');
  } finally {
    print('Finalizando ejecución.');
  }
}
```

## 7.5. Generar excepciones con `throw`

Puedes lanzar excepciones manualmente para indicar que algo no está bien.

```dart
void verificarEdad(int edad) {
  if (edad < 18) {
    throw Exception('La edad debe ser mayor o igual a 18 años.');
  } else {
    print('Acceso permitido.');
  }
}

void main() {
  try {
    verificarEdad(15);
  } catch (e) {
    print('Error detectado: $e');
  }
}
```

## 7.6. Excepciones personalizadas

Puedes crear tus propias clases de excepciones para casos específicos. Estas clases implementan la interfaz `Exception`.

```dart
class SaldoInsuficienteException implements Exception {
  String mensaje;
  SaldoInsuficienteException(this.mensaje);
}

void retirar(double saldo, double monto) {
  if (monto > saldo) {
    throw SaldoInsuficienteException('Saldo insuficiente para realizar el retiro.');
  } else {
    print('Retiro exitoso. Saldo restante: ${saldo - monto}');
  }
}

void main() {
  try {
    retirar(100.0, 150.0);
  } on SaldoInsuficienteException catch (e) {
    print('Error: ${e.mensaje}');
  }
}
```

## 7.7. Ejercicios propuestos

1. Crea un programa que solicite dos números e intente dividirlos. Captura el caso de división por cero con `try` y `catch`.  
2. Escribe un programa que reciba un valor de tipo `String` y lo convierta a entero. Maneja el caso en que el valor no sea numérico con un bloque `catch`.  
3. Implementa una función `retirarSaldo(double saldo, double monto)` que lance una excepción personalizada si el monto excede el saldo disponible. Captura la excepción en `main()` y muestra un mensaje adecuado.  
4. Escribe un bloque que use `try`, `catch` y `finally` para simular la lectura de un archivo e imprime un mensaje de cierre tanto si ocurre un error como si no.

---

<a name="capitulo-8-programacion-asincrona"></a>
# 8. Programación asíncrona

En muchos casos, los programas deben realizar operaciones que toman tiempo: leer archivos, consultar bases de datos o esperar una respuesta de internet. Si estas operaciones se ejecutaran de manera estrictamente secuencial, el programa se bloquearía hasta que cada una terminara.  
Para evitarlo, Dart incluye un modelo de **programación asíncrona** que permite ejecutar tareas de larga duración sin detener el flujo principal.

## 8.1. Concepto de asincronía

Una operación asíncrona se ejecuta sin bloquear las instrucciones que siguen.  
En Dart, las operaciones asíncronas se representan mediante la clase `Future`, que actúa como una promesa de que un valor estará disponible en el futuro.  

```dart
void main() {
  print('Inicio del programa');

  Future.delayed(Duration(seconds: 2), () {
    print('Operación completada después de 2 segundos');
  });

  print('Fin del programa');
}
```

La función `Future.delayed()` ejecuta su callback después del tiempo indicado. La salida muestra que el programa no se bloquea mientras espera.

## 8.2. La clase `Future` y el método `then()`

Un `Future<T>` representa un valor de tipo `T` que estará disponible más adelante. Puedes manejarlo con el método `then()`:

```dart
Future<String> obtenerMensaje() async {
  return 'Datos recibidos correctamente';
}

void main() {
  Future<String> resultado = obtenerMensaje();
  resultado.then((valor) {
    print(valor);
  }).catchError((error) {
    print('Ocurrió un error: $error');
  });
  print('Ejecutando otras tareas...');
}
```

## 8.3. Uso de `async` y `await`

Las palabras clave `async` y `await` permiten escribir código asíncrono con un estilo más similar al código secuencial.

```dart
Future<String> obtenerUsuario() async {
  print('Consultando datos...');
  await Future.delayed(Duration(seconds: 2));
  return 'Usuario encontrado: Ana Pérez';
}

void main() async {
  print('Inicio del proceso');
  String usuario = await obtenerUsuario();
  print(usuario);
  print('Fin del proceso');
}
```

- La función marcada con `async` devuelve un `Future`.  
- `await` suspende la ejecución dentro de la función hasta que el `Future` se resuelva.  
- El hilo principal no se bloquea; simplemente espera dentro de la función asíncrona.

## 8.4. Manejo de errores en funciones asíncronas

Puedes combinar `async` y `await` con bloques `try` y `catch` para manejar excepciones dentro de funciones asíncronas.

```dart
Future<void> procesarDatos() async {
  try {
    print('Procesando información...');
    await Future.delayed(Duration(seconds: 1));
    throw Exception('Error al procesar los datos.');
  } catch (e) {
    print('Excepción capturada: $e');
  } finally {
    print('Finalizando proceso.');
  }
}

void main() async {
  await procesarDatos();
}
```

## 8.5. Ejecutar múltiples operaciones asíncronas

Cuando se tienen varias tareas asíncronas, puedes esperar a que todas se completen con `Future.wait()`.

```dart
Future<String> tareaA() async {
  await Future.delayed(Duration(seconds: 2));
  return 'Tarea A completada';
}

Future<String> tareaB() async {
  await Future.delayed(Duration(seconds: 3));
  return 'Tarea B completada';
}

void main() async {
  print('Iniciando tareas...');
  List<String> resultados = await Future.wait([tareaA(), tareaB()]);
  print(resultados);
}
```

## 8.6. Flujos de datos con `Stream`

Un `Stream` representa una secuencia de valores que se generan a lo largo del tiempo. Se utiliza para manejar eventos o datos que llegan progresivamente.

```dart
Stream<int> generarNumeros() async* {
  for (int i = 1; i <= 3; i++) {
    await Future.delayed(Duration(seconds: 1));
    yield i;
  }
}

void main() async {
  await for (int numero in generarNumeros()) {
    print('Número recibido: $numero');
  }
}
```

- La función marcada con `async*` devuelve un `Stream`.  
- `yield` emite cada valor.  
- La sintaxis `await for` permite procesar cada elemento a medida que llega.

Los flujos también pueden emitir errores. Puedes capturarlos con un bloque `try` y `catch` dentro de la construcción `await for`.

## 8.7. Ejercicios propuestos

1. Crea una función `descargarArchivo()` que simule la descarga de un archivo con un retardo de 3 segundos e imprima un mensaje al finalizar.  
2. Implementa dos funciones asíncronas que devuelvan resultados en distintos tiempos y usa `Future.wait()` para ejecutarlas en paralelo.  
3. Crea un flujo que emita los números del 1 al 5 cada segundo y que, al llegar al número 3, lance una excepción que deba capturarse.  
4. Escribe una función `consultarAPI()` que use `async`, `await` y `try`/`catch` para simular la obtención de datos desde un servidor y maneje posibles errores.

---

<a name="capitulo-9-buenas-practicas"></a>
# 9. Buenas prácticas

Aprender un lenguaje no solo consiste en conocer su sintaxis, sino también en aplicar **buenas prácticas** para escribir código legible, mantenible y coherente. A continuación se presentan recomendaciones generales para el desarrollo en Dart.

## 9.1. Convenciones de nomenclatura

Seguir un estilo de nombres consistente facilita la lectura del código:

- **Variables y funciones:** usa `camelCase`. Ejemplo: `nombreCompleto`, `calcularTotal()`.  
- **Clases:** usa `PascalCase`. Ejemplo: `Usuario`, `CuentaBancaria`.  
- **Constantes globales:** usa `lowerCamelCase`. Ejemplo: `defaultTimeout`, `maxRetries`.  
- **Constantes visuales en Flutter:** suele utilizarse el prefijo `k` seguido de `PascalCase` (práctica común, no oficial). Ejemplo: `kPrimaryColor`, `kDefaultPadding`.  
- **Privados:** usa un guion bajo `_` al inicio del nombre para indicar que solo se debe usar dentro del archivo. Ejemplo: `_contador`.

> Dart no utiliza `SCREAMING_SNAKE_CASE` para constantes como en otros lenguajes. Prefiere `camelCase` o, en Flutter, `kPascalCase`.

## 9.2. Uso de variables y constantes

- Declara variables con el tipo más adecuado.  
- Usa `final` para valores que no deberían cambiar tras su asignación, y `const` cuando el valor sea literal y conocido en tiempo de compilación.  
- Evita redefinir variables a menos que sea necesario.  

```dart
final nombre = 'Ana';      // asignado una vez
const pi = 3.1416;         // constante de compilación
```

## 9.3. Comentarios claros y útiles

Los comentarios deben explicar **por qué** haces algo, no repetir lo que el código ya expresa claramente. Para documentar funciones o clases públicas, utiliza comentarios de documentación (`///`).

```dart
/// Calcula el área de un círculo.
/// [radio] es el radio del círculo.
/// Retorna el área como double.
double calcularArea(double radio) {
  return pi * radio * radio;
}
```

## 9.4. Principio de responsabilidad única

Cada función o clase debe tener una sola responsabilidad. Esto facilita el mantenimiento y la reutilización.

```dart
class GestorUsuarios {
  void registrarUsuario(String nombre) {
    _guardarEnBaseDatos(nombre);
  }

  void _guardarEnBaseDatos(String nombre) {
    print('Usuario $nombre guardado en la base de datos.');
  }
}
```

## 9.5. Evitar código duplicado

Repetir fragmentos de código hace que sea más difícil de mantener. Extrae la lógica repetida en funciones reutilizables.

```dart
double calcularPromedio(List<double> valores) {
  if (valores.isEmpty) return 0.0;
  double suma = valores.reduce((a, b) => a + b);
  return suma / valores.length;
}
```

## 9.6. Null safety: uso de `?`, `??` y `!`

Dart incorpora **null safety** para evitar errores comunes al trabajar con valores nulos.  

- Añade `?` al tipo para indicar que puede ser nulo: `String? nombre;`.  
- Usa `??` para proporcionar un valor por defecto si una expresión es nula: `nombre ?? 'invitado'`.  
- Usa `!` cuando estás seguro de que la expresión no es nula (assertión nula), pero debe usarse con precaución porque si el valor es nulo en tiempo de ejecución, se lanzará una excepción:

```dart
void main() {
  String? nombre;
  print(nombre ?? 'invitado'); // imprime invitado

  nombre = 'Laura';
  print(nombre!.toUpperCase()); // imprime LAURA

  // Si nombre fuera null aquí, nombre!.toUpperCase() lanzaría una excepción
}
```

## 9.7. Manejo adecuado de errores

- Anticipa las excepciones y captura solo las que puedas manejar.  
- No utilices excepciones como flujo normal del programa.  
- Proporciona mensajes claros y acciones concretas cuando se produce un error.  

## 9.8. Comparaciones entre malas y buenas prácticas

| **Malas prácticas** | **Buenas prácticas** |
| --- | --- |
| Nombres de variables poco descriptivos (`void p(double r) { print(3.14 * r * r); }`) | Nombres explícitos (`void calcularAreaCirculo(double radio) { … }`) |
| Código duplicado para calcular promedios o sumas | Funciones reutilizables (`calcularPromedio()`) |
| Ignorar posibles valores nulos y usar `!` indiscriminadamente | Declarar variables como `nullable` (`?`), usar `??` y validar antes de acceder |
| No manejar excepciones en operaciones que pueden fallar (división entre cero, conversiones) | Uso de `try`/`catch` y mensajes claros |
| Comentarios redundantes que repiten el código | Comentarios que explican la intención o el propósito |

## 9.9. Ejercicios propuestos

1. Reescribe una función que imprima un mensaje usando nombres descriptivos para variables y funciones.  
2. Refactoriza una porción de código con duplicación (por ejemplo, calcular promedios en varias partes) para centralizar la lógica en una única función.  
3. Implementa un bloque `try-catch` que capture errores al convertir una cadena a entero y proporcione un mensaje claro al usuario.  
4. Revisa un código previo e identifica al menos tres malas prácticas, proponiendo alternativas correctas según lo aprendido.

---

<a name="epilogo"></a>
# Epílogo

Este documento ha sido un punto de partida. A lo largo de estas páginas, Dart nos permitió descubrir cómo las ideas pueden tomar forma mediante la lógica, la estructura y la creatividad. Cada concepto aprendido, desde las variables más simples hasta la asincronía más compleja, representa una herramienta que puedes llevar contigo para construir proyectos reales y, sobre todo, para seguir aprendiendo.  

El verdadero valor de programar no reside únicamente en escribir código que funcione, sino en **entender cómo pensar en soluciones**. Esa es la esencia de todo lenguaje de programación: ofrecer una forma distinta de razonar, de imaginar y de crear.  

Hoy, al concluir este recorrido, ya dominas los fundamentos para desarrollar con confianza en Dart y dar el siguiente paso hacia Flutter u otros entornos modernos. Pero más allá de la técnica, queda la convicción de que cada línea escrita es una oportunidad para mejorar, para descubrir y para transformar el entorno.  

> “El conocimiento es el punto de partida; la curiosidad, el camino que nunca termina.”

Gracias por acompañar este proceso de aprendizaje. Que estas páginas sirvan como una base firme, pero también como una invitación constante a seguir explorando, a crear y a compartir el conocimiento con otros.  

**Fin.**


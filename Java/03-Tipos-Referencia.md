Tipos de Referencia

Son todos los tipos de datos que no son primitivos

Solo Existen 8 tipos de datos primitivos el resto son por Referencia

El mas Importante es el de String.

String sirve para que nosotros podamos crear texto dentro de nuestras aplicaciones

Cuando a un String no le estamos llamando new String Nosotros lo llamamos String Literal es el cual vamos a utilizar en su mayoria.

Estos string tienen muchos metodos estos metodos los utilizaremos usando el nombre de la variable y un punto

```Java
String text = "Hola Mundo!";
//text es el nombre de la variable
text.lenght();
```

por ejemplo asi:

```Java
String text = "Hola Mundo!";

int largo = text.length();
System.out.println(largo);
// El resultado es 11
```

Metodos de los String literal:

Los valores que le damos a estos metodos se le conoce como "Argumentos".

Los Strings son inmutables lo que quiere decir que cualquier metodo que nosotors llamemos de un String lo que va a hacer es crear un nuevo String y devolvérmelo para que nosotos lo podamos asignar a una variable.

Podemos llamar a los metodos tambien desde los println:

```Java
System.out.println(texto.endsWith());
```

Tipos de metodos:

- length(): Retorna la cantidad de caracteres de una cadena.
- replace(old, new): Reemplaza todas las apariciones de old por new en una cadena.
- endsWith(): Me devuelve true o false dependiendo de si mi String termina con lo que yo le indique por ejemplo:

```Java
String text = "Hola Mundo!";

      int largo = text.length();
        System.out.println(largo);

        String texto = text.replace("Hola", "chao");
        System.out.println(text);

        System.out.println(texto.endsWith("undo!"));
// Devuelve true porque si termina como esta puesto en la variable texto pero si cambiaramos undo! por und o undo sin la excalamacion daria false
```

- startsWitch: Me devuelve true o false dependiendo de si mi String comienza con lo que yo le indique por ejemplo:

```Java
String text = "Hola Mundo!";

      int largo = text.length();
        System.out.println(largo);

        String texto = text.replace("Hola", "chao");
        System.out.println(text);

        System.out.println(texto.endsWith("undo!"));
        System.out.println(texto.startsWith("Ch"));
// Devuelve true porque si comienza como esta puesto en la variable texto pero si cambiaramos Ch por h daria false
```

- contains(): Este metodo se utiliza para saber si nos a servir a nosotros saber si es que nuestro string contiene o no contiene una cadena de texto en especifico.

```Java
String text = "Hola Mundo!";

      int largo = text.length();
        System.out.println(largo);

        String texto = text.replace("Hola", "chao");
        System.out.println(text);

        System.out.println(texto.endsWith("undo!"));
        System.out.println(texto.startsWith("Ch"));
        System.out.println(texto.contains("und"));
// true
```

- indexOf:

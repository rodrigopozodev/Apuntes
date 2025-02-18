# Introducción a Java

## ¿Qué es Java?

Java es un lenguaje de programación:

- **Orientado a Objetos**
- **Rápido**
- **Seguro**
- **Confiable**

Es el lenguaje preferido por los bancos y utilizado por empresas como:  
Amazon, Microsoft, Google, Netflix, Spotify, Instagram, eBay, entre otras.

El código en Java se ejecuta muy rápido.

## Características principales

Java es:

- **Multiplataforma**
- **Orientado a objetos**
- **Una plataforma de computación**
- **Ejecutado en más de 56 mil millones de dispositivos en todo el mundo**

## Historia de Java

- Proyecto iniciado en **1991**
- Lanzado en **1995** por _Sun Microsystems_
- Disponible para el público en **1996**

## Máquina Virtual de Java (JVM)

El intérprete de Java es la **JVM (Java Virtual Machine)**, encargado de proporcionar una especificación sobre cómo debe ejecutarse el código.

Para instalar una JVM en nuestro ordenador, necesitamos un **JRE (Java Runtime Environment)**, que se encarga de instalar la JVM en nuestro sistema.

### ¿Qué proporciona el JRE?

- **Archivos de configuración**
- **Librerías o bibliotecas** que la JVM utiliza

El código del JRE debe escribirse de forma independiente para cada plataforma, lo que significa que existen diferentes versiones de JRE para Mac, Linux y Windows.

## Proceso de Ejecución de Java

1. **Nuestro código en Java pasa por el compilador (Java Compiler)**.
2. **El compilador transforma el código en Java Bytecode**.
3. **El Bytecode es interpretado por la JVM**, permitiendo su ejecución en distintas plataformas.

## JDK (Java Development Kit)

Para compilar y ejecutar código Java, necesitamos el **JDK (Java Development Kit)**, que incluye:

- **Compilador (Java Compiler)**
- **JRE (Java Runtime Environment)**

# Introducción a Java

## ¿Qué es Java?

Java es un lenguaje de programación:

- **Orientado a Objetos**
- **Rápido**
- **Seguro**
- **Confiable**

Es el lenguaje preferido por los bancos y utilizado por empresas como:  
Amazon, Microsoft, Google, Netflix, Spotify, Instagram, eBay, entre otras.

El código en Java se ejecuta muy rápido.

## Características principales

Java es:

- **Multiplataforma**
- **Orientado a objetos**
- **Una plataforma de computación**
- **Ejecutado en más de 56 mil millones de dispositivos en todo el mundo**

## Historia de Java

- Proyecto iniciado en **1991**
- Lanzado en **1995** por _Sun Microsystems_
- Disponible para el público en **1996**

## Máquina Virtual de Java (JVM)

El intérprete de Java es la **JVM (Java Virtual Machine)**, encargado de proporcionar una especificación sobre cómo debe ejecutarse el código.

Para instalar una JVM en nuestro ordenador, necesitamos un **JRE (Java Runtime Environment)**, que se encarga de instalar la JVM en nuestro sistema.

### ¿Qué proporciona el JRE?

- **Archivos de configuración**
- **Librerías o bibliotecas** que la JVM utiliza

El código del JRE debe escribirse de forma independiente para cada plataforma, lo que significa que existen diferentes versiones de JRE para Mac, Linux y Windows.

## Proceso de Ejecución de Java

1. **Nuestro código en Java pasa por el compilador (Java Compiler)**.
2. **El compilador transforma el código en Java Bytecode**.
3. **El Bytecode es interpretado por la JVM**, permitiendo su ejecución en distintas plataformas.

## JDK (Java Development Kit)

Para compilar y ejecutar código Java, necesitamos el **JDK (Java Development Kit)**, que incluye:

- **Compilador (Java Compiler)**
- **JRE (Java Runtime Environment)**

---

# Programación Orientada a Objetos en Java

Java es fuertemente orientado a objetos, lo que significa que si no creamos un objeto de manera inicial, nuestras aplicaciones no se ejecutarán.

### Conceptos fundamentales:

- **Clases**
- **Objetos o instancias de clase**
  - Los objetos se componen de **métodos** y **propiedades**.
    - **Propiedades**: Características del objeto (ejemplo: color).
    - **Métodos**: Acciones que puede realizar el objeto.

### Convenciones de nomenclatura

Cuando una clase está escrita sin espacios y con mayúscula en la primera letra de cada palabra, por ejemplo `ControlPlayStation`, estamos usando **PascalCase**.  
Cuando creamos una instancia de la clase, escribimos `controlPlayStation`, donde la primera letra es minúscula. A esto se le conoce como **camelCase**.

### La clase principal: `Main`

Todas las aplicaciones en Java deben contener una clase llamada `Main`. Si no tiene esta clase, la aplicación no funcionará.

La clase `Main` contiene un método especial llamado `main`, que es el punto de entrada de cualquier aplicación en Java.

```java
public class Main {
    public static void main(String[] args) {
        System.out.println("¡Hola, Java!");
    }
}
```

El primer método que se ejecuta en una aplicación Java es el método `main` de la clase `Main`.

### Métodos en Java

Los métodos pueden estar asociados a instancias de objetos o directamente a una clase.

- **Métodos de instancia**: Asociados a objetos específicos.
- **Métodos de clase**: Pertenecen a la clase en sí y no requieren una instancia para ser llamados.

Los métodos de clase se identifican con la palabra clave `static`, lo que significa que el método es exclusivo de la clase.

```java
public class Ejemplo {
    static void metodoDeClase() {
        System.out.println("Este es un método de clase");
    }

    void metodoDeInstancia() {
        System.out.println("Este es un método de instancia");
    }
}

public class Main {
    public static void main(String[] args) {
        Ejemplo.metodoDeClase(); // Llamada a un método de clase

        Ejemplo objeto = new Ejemplo();
        objeto.metodoDeInstancia(); // Llamada a un método de instancia
    }
}
```

Los métodos de clase (`static`) y los métodos de instancia **no se mezclan**, ya que funcionan de manera diferente dentro de la programación orientada a objetos.

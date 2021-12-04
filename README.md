# Notas del Curso de Introduccion a Solidity

Profesor Sebastián Leonardo Perez @sebaleoperez

![](https://static.platzi.com/media/avatars/Platzi-f730e65b-e92b-44d3-81c0-5c59c4dc4658.png) ![](https://static.platzi.com/media/learningpath/badges/29fa8885-7536-44ba-8aea-7b32c8e39cc8.jpg) ![](https://static.platzi.com/media/achievements/solidity_badge-ca6318a4-8808-4e95-9b1a-ccdd7016589e.png)

## Tabla de Contenidos

- [Por qué debes aprender Solidity](#por-qué-debes-aprender-solidity)
  - [La importancia de Web3 y Solidity](#la-importancia-de-web3-y-solidity) 
- [Introducción a la programación con Solidity](#introducción-a-la-programación-con-solidity)
  - [Estructura de un contrato](#estructura-de-un-contrato)
- [Funciones](#funciones) 
- [Gestionando costos](#gestionando-costos)
- [Conceptos avanzados](#conceptos-avanzados)


# Por qué debes aprender Solidity

## La importancia de Web3 y Solidity

#### Web3:

Así denominamos a la evolución de las aplicaciones que funcionan sobre internet, integrando tecnologías como big data e inteligencia artificial, para lograr escenarios como las redes sociales.

#### Blockchain:

La aparición de esta tecnología juega un rol clave en la evolución de la web3, ya que agrega una característica innovadora: **La descentralización.**

#### Solidity:

No existe una sola plataforma de Blockchain, pero en la diversidad se destacan aquellas que 
agregan la capacidad de ejecutar código. Solidity es un lenguaje especialmente creado 
para el diseño de este código conocido como contratos inteligentes.

Solidity es un lenguaje de alto nivel orientado a contratos. Su sintaxis es similar a la de JavaScript y está enfocado específicamente a la Máquina Virtual de Etehreum (EVM). Solidity está tipado de manera estática y acepta, entre otras cosas, herencias, librerías y tipos complejos definidos por el usuario.

Más importante incluso que Solidity es la EVM (Ethereum Virtual Machine), por su impacto cultural y tecnológico al implementarse en distintos blockchains. Solidity es un lenguaje que compila hacia la EVM, por lo que es compatible con redes como BSC, Polygon, RSK, TRON, etc.

https://github.com/ethereum/solidity

# Introducción a la programación con Solidity

## Estructura de un contrato

#### Pragma

Todos los contratos comienzan con la sentencia pragma el cual señala la versión de Solidity a utilizar. 

Puede hacerse referencia a una versión puntual o a un rango de versiones.

#### Contract

Para comenzar la declaración del contrato debemos utilizar el keyword contract. 

Todo lo que se encuentre en el entorno de este keyword será parte del mismo contrato.

#### Constructor

Al igual que en la programación orientada a objetos, cada contrato cuenta con una función  opcional constructor la cual se ejecuta por única vez cuando se crea el contrato.


```
// Version puede representar un rango. Ej >=0.7.0 <0.9.0
pragma solidity <version>;

// Declaración de un contrato, similar a una clase
contract <name> { // Name puede ser cualquier cosa
  
  // Función de inicialización de un contrato
  constructor() {
    // Código de inicialización
  }
}
```

## Variables y tipos de datos

#### Tipos de datos:

1. **Números enteros:** No se recomiendan los números decimales.
  - **int:** Números enteros. 
  - **uint:** Son números enteros sin signos. Pueden opcionalmente indicar su tamaño en bits.
  Pueden tener una capacidad de 8 a 256 bits.

2. **bool:** Valor booleano, representa verdadero/falso.
    - true - false
    - ! (negación)
    - && (and)
    - || (or)
    - == (igualdad)
    - != (Desigualdad)

3. **address:** Almacenan direcciones de Ethereum. Sirve para relacionar cuentas y contratos. Guarda direcciones de ETH de 160 bits (20 bytes), y puede tener métodos extra como .transfer o .balance

4. **string:** Cadena de texto. Representa un texto en forma de cadena de 
caracteres.

5. **bytes:** Representa una cadena de bytes sin un 
formato específico entre 8-256.

#### Tipos de varibles:

1. **Variables locales:** Son aquellas que ocurren durante la ejecución. En la EVM es la parte correspondiente a memoria volátil. Se alojan de forma temporal para utilizarse dentro del ámbito de una función.

2. **Variables de estado:** Son variables que se almacenan en la parte de la ROM de la EVM. Es memoria persistente. Se almacenan en el contrato y que mantienen su valor aun después de finalizada la ejecución de la función.

3. **Variables globales:**

- **msg:** Toda transacción es un mensaje firmado. En este objeto vienen los datos de dicho mensaje (sender, value, etc.).

- **tx:** Represena la transacción, es distitna respecto a msg porque cosas como el sender van variando conforme se concatenan llamadas entre contratos.

- **block:** Información respecto al bloque actual.

[![1](https://github.com/hackmilo/Notas---Curso-de-Introduccion-Solidity/blob/main/img/1.png?raw=true "1")](https://github.com/hackmilo/Notas---Curso-de-Introduccion-Solidity/blob/main/img/1.png?raw=true "1")

## Struct y Arrays

- **Struct:** 
Tipo de dato estructurado que nos permite almacenar información de distintos tipos en un solo esquema. Generalmente, se usa para representar un registro. Para definir una estructura se utiliza la palabra clave struct, que crea un nuevo tipo de datos.

```
struct <name> {
  <type> <name>;
  ...
  <type> <name>;
}
```

- **Arrays:**
Es una cadena de elementos del mismo tipo de dato que se almacenan de forma consecutiva y por lo tanto se puede acceder a un elemento según su posición dentro de la misma. 

Se dividen en: 
- Arrays estáticos
- Arrays dinámicos

```
<type>[] <visibility> <name>;

// Arreglos estáticos (n = cantidad de elementos)
<type>[n] <visibility> <name>;

// Arreglos dinámicos
<type>[] <visibility> <name>;
```

# Funciones

# Gestionando costos

# Conceptos avanzados
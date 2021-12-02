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

#### Blockchain

La aparición de esta tecnología juega un rol clave en la evolución de la web3, ya que agrega una característica innovadora: **La descentralización.**

#### Solidity

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

# Funciones

# Gestionando costos

# Conceptos avanzados
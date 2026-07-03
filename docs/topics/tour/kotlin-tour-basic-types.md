---
# SPDX-FileCopyrightText: 2010-2026 JetBrains s.r.o. and Kotlin Programming
# Language contributors.
# Kotlin and the Kotlin logo are trademarks or registered trademarks of The
# Kotlin Foundation.
#
# SPDX-License-Identifier: Apache-2.0
# Documentation licensed under the Apache License, Version 2.0.
# The original work was translated from English into Brazilian Portuguese.
# https://github.com/docsdevbr/kotlin-docs-pt-br/blob/-/LICENSES/Apache-2.0.txt

# source_url: https://github.com/JetBrains/kotlin-web-site/blob/master/docs/topics/tour/kotlin-tour-basic-types.md
# source_revision: f8db6b2b52d297f11f1521058ffdc4f4e94d5400
# translation_status: ready
---

[//]: # (title: Tipos básicos)

<no-index/>

<tldr>
    <p>
      <img src="icon-1-done.svg" width="20" alt="Primeiro passo" /> <a href="kotlin-tour-hello-world.md">Olá, mundo</a><br />
      <img src="icon-2.svg" width="20" alt="Segundo passo" /> <strong>Tipos básicos</strong><br />
      <img src="icon-3-todo.svg" width="20" alt="Terceiro passo" /> <a href="kotlin-tour-collections.md">Coleções</a><br />
      <img src="icon-4-todo.svg" width="20" alt="Quarto passo" /> <a href="kotlin-tour-control-flow.md">Fluxo de controle</a><br />
      <img src="icon-5-todo.svg" width="20" alt="Quinto passo" /> <a href="kotlin-tour-functions.md">Funções</a><br />
      <img src="icon-6-todo.svg" width="20" alt="Sexto passo" /> <a href="kotlin-tour-classes.md">Classes</a><br />
      <img src="icon-7-todo.svg" width="20" alt="Último passo" /> <a href="kotlin-tour-null-safety.md">Segurança contra nulos</a></p>
</tldr>

Toda variável e estrutura de dados no Kotlin possui um tipo.
Os tipos são importantes porque indicam ao compilador o que você pode fazer com
aquela variável ou estrutura de dados. Em outras palavras, quais funções e
propriedades ela possui.

No capítulo anterior, o Kotlin conseguiu identificar, no exemplo dado, que
`customers` é do tipo
[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/).
A capacidade do Kotlin de **inferir** o tipo é chamada de **inferência de
tipo**.
A variável `customers` recebe um valor inteiro; com base nisso, o Kotlin infere
que `customers` possui o tipo numérico `Int`.
Como resultado, o compilador sabe que você pode realizar operações aritméticas
com `customers`:

```kotlin
fun main() {
//sampleStart
    var customers = 10

    // Alguns clientes saem da fila
    customers = 8

    customers = customers + 3 // Exemplo de adição: 11
    customers += 7            // Exemplo de adição: 18
    customers -= 3            // Exemplo de subtração: 15
    customers *= 2            // Exemplo de multiplicação: 30
    customers /= 3            // Exemplo de divisão: 10

    println(customers) // 10
//sampleEnd
}
```
{kotlin-runnable="true" kotlin-min-compiler-version="1.3" id="kotlin-tour-basic-types-arithmetic"}

> `+=`, `-=`, `*=`, `/=` e `%=` são operadores de atribuição aumentada.
> Para mais informações, consulte
> [Atribuições aumentadas](operator-overloading.md#augmented-assignments).
>
{style="tip"}

No total, o Kotlin possui os seguintes tipos básicos:


| **Categoria**                                                 | **Tipos básicos**                  | **Código de exemplo**                                             |
|---------------------------------------------------------------|------------------------------------|-------------------------------------------------------------------|
| [Inteiros](numbers.md#integer-types)                          | `Byte`, `Short`, `Int`, `Long`     | `val year: Int = 2020`<br/> `val amount: Long = 350_000_000`      |
| [Inteiros sem sinal](unsigned-integer-types.md)               | `UByte`, `UShort`, `UInt`, `ULong` | `val score: UInt = 100u`                                          |
| [Números de ponto flutuante](numbers.md#floating-point-types) | `Float`, `Double`                  | `val currentTemp: Float = 24.5f`<br/> `val price: Double = 19.99` |
| [Booleanos](booleans.md)                                      | `Boolean`                          | `val isEnabled: Boolean = true`                                   |
| [Caracteres](characters.md)                                   | `Char`                             | `val separator: Char = ','`                                       |
| [Strings](strings.md)                                         | `String`                           | `val message: String = "Olá, mundo!"`                           |

Para obter mais informações sobre tipos básicos e suas propriedades, consulte
[Visão geral dos tipos](types-overview.md).

Com esse conhecimento, você pode declarar variáveis e inicializá-las
posteriormente.
O Kotlin consegue lidar com isso, desde que as variáveis sejam inicializadas
antes da primeira leitura.

Para declarar uma variável sem inicializá-la, especifique seu tipo com `:`.
Por exemplo:

```kotlin
fun main() {
//sampleStart
    // Variável declarada sem inicialização
    val d: Int
    // Variável inicializada
    d = 3

    // Variável tipada e inicializada explicitamente
    val e: String = "olá"

    // As variáveis podem ser lidas porque foram inicializadas
    println(d) // 3
    println(e) // olá
//sampleEnd
}
```
{kotlin-runnable="true" kotlin-min-compiler-version="1.3" id="kotlin-tour-basic-types-initialization"}

Se você não inicializar uma variável antes de lê-la, verá um erro:

```kotlin
fun main() {
//sampleStart
    // Variável declarada sem inicialização
    val d: Int

    // Dispara um erro
    println(d)
    // Variable 'd' must be initialized
//sampleEnd
}
```
{kotlin-runnable="true" kotlin-min-compiler-version="1.3" id="kotlin-tour-basic-types-no-initialization" validate="false"}

Agora que você sabe como declarar tipos básicos, é hora de aprender sobre
[coleções](kotlin-tour-collections.md).

## Prática

### Exercício {initial-collapse-state="collapsed" collapsible="true"}

Declare explicitamente o tipo correto para cada variável:

|---|---|
```kotlin
fun main() {
    val a: Int = 1000
    val b = "mensagem de log"
    val c = 3.14
    val d = 100_000_000_000_000
    val e = false
    val f = '\n'
}
```
{validate="false" kotlin-runnable="true" kotlin-min-compiler-version="1.3" id="kotlin-tour-basic-types-exercise"}

|---|---|
```kotlin
fun main() {
    val a: Int = 1000
    val b: String = "mensagem de log"
    val c: Double = 3.14
    val d: Long = 100_000_000_000_000
    val e: Boolean = false
    val f: Char = '\n'
}
```
{initial-collapse-state="collapsed" collapsible="true" collapsed-title="Solução do exemplo" id="kotlin-tour-basic-types-solution"}

## Próximo passo

[Coleções](kotlin-tour-collections.md)

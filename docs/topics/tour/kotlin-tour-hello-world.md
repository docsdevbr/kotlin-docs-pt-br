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

# source_url: https://github.com/JetBrains/kotlin-web-site/blob/master/docs/topics/tour/kotlin-tour-hello-world.md
# source_revision: 579b02b65fce064431378d48442edf5f48a659a1
# translation_status: ready
---

[//]: # (title: Olá, mundo)

<no-index/>

<tldr>
  <p>
    <img src="icon-1.svg" width="20" alt="Primeiro passo" /> <strong>Olá, mundo</strong><br />
    <img src="icon-2-todo.svg" width="20" alt="Segundo passo" /> <a href="kotlin-tour-basic-types.md">Tipos básicos</a><br />
    <img src="icon-3-todo.svg" width="20" alt="Terceiro passo" /> <a href="kotlin-tour-collections.md">Coleções</a><br />
    <img src="icon-4-todo.svg" width="20" alt="Quarto passo" /> <a href="kotlin-tour-control-flow.md">Fluxo de controle</a><br />
    <img src="icon-5-todo.svg" width="20" alt="Quinto passo" /> <a href="kotlin-tour-functions.md">Funções</a><br />
    <img src="icon-6-todo.svg" width="20" alt="Sexto passo" /> <a href="kotlin-tour-classes.md">Classes</a><br />
    <img src="icon-7-todo.svg" width="20" alt="Último passo" /> <a href="kotlin-tour-null-safety.md">Segurança contra nulos</a>
  </p>
</tldr>

Aqui está um programa simples que imprime "Olá, mundo!":

```kotlin
fun main() {
    println("Olá, mundo!")
    // Olá, mundo!
}
```
{kotlin-runnable="true" kotlin-min-compiler-version="1.3" id="hello-world-kotlin"}

No Kotlin:

* `fun` é usado para declarar uma função.
* A função `main()` é o ponto de partida do seu programa.
* O corpo de uma função é escrito entre chaves `{}`.
* As funções
  [`println()`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.io/println.html)
  e
  [`print()`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.io/print.html)
  imprimem seus argumentos na saída padrão.

Uma função é um conjunto de instruções que realiza uma tarefa específica.
Após criar uma função, você pode usá-la sempre que precisar realizar essa
tarefa, sem ter que escrever as instruções novamente.
Funções serão abordadas com mais detalhes em capítulos posteriores.
Até lá, todos os exemplos usam a função `main()`.

## Variáveis

Todos os programas precisam ser capazes de armazenar dados, e as variáveis
ajudam você a fazer exatamente isso.
No Kotlin, você pode declarar:

* Variáveis somente leitura com `val`.
* Variáveis mutáveis com `var`.

> Você não pode alterar uma variável somente leitura depois de atribuir um valor
> a ela.
>
{style="note"}

Para atribuir um valor, use o operador de atribuição `=`.

Por exemplo:

```kotlin
fun main() {
//sampleStart
    val popcorn = 5    // Há 5 caixas de pipoca
    val hotdog = 7     // Há 7 cachorros-quentes
    var customers = 10 // Há 10 clientes na fila

    // Alguns clientes saem da fila
    customers = 8
    println(customers)
    // 8
//sampleEnd
}
```
{kotlin-runnable="true" kotlin-min-compiler-version="1.3" id="kotlin-tour-variables"}

> Variáveis podem ser declaradas fora da função `main()`, no início do programa.
> Variáveis declaradas dessa forma são consideradas declaradas no **nível
> superior**.
>
{style="tip"}

Como `customers` é uma variável mutável, seu valor pode ser reatribuído após a
declaração.

> Recomendamos declarar todas as variáveis como somente leitura (`val`) por
> padrão.
> Use variáveis mutáveis (`var`) apenas se realmente precisar.
> Dessa forma, você reduz a chance de alterar acidentalmente algo que não
> deveria ser modificado.
>
{style="note"}

## Templates de string

É útil saber como exibir o conteúdo de variáveis na saída padrão.
Você pode fazer isso usando **templates de string**.
É possível usar expressões de template para acessar dados armazenados em
variáveis e outros objetos, e convertê-los em strings.
Um valor de string é uma sequência de caracteres entre aspas duplas `"`.
Expressões de template sempre começam com um cifrão `$`.

Para avaliar um trecho de código em uma expressão de template, coloque o código
entre chaves `{}` após o cifrão `$`.

Por exemplo:

```kotlin
fun main() {
//sampleStart
    val customers = 10
    println("Há $customers clientes")
    // Há 10 clientes

    println("Há ${customers + 1} clientes")
    // Há 11 clientes
//sampleEnd
}
```
{kotlin-runnable="true" kotlin-min-compiler-version="1.3" id="kotlin-tour-string-templates"}

Para mais informações, consulte
[Templates de string](strings.md#string-templates).

Você notará que não há tipos declarados para as variáveis.
O Kotlin inferiu o tipo por conta própria: `Int`.
Este tour explica os diferentes tipos básicos do Kotlin e como declará-los no
[próximo capítulo](kotlin-tour-basic-types.md).

## Prática

### Exercício {initial-collapse-state="collapsed" collapsible="true"}

Complete o código para fazer o programa imprimir `"Maria tem 20 anos"` na saída
padrão:

|---|---|
```kotlin
fun main() {
    val name = "Maria"
    val age = 20
    // Escreva seu código aqui
}
```
{validate="false" kotlin-runnable="true" kotlin-min-compiler-version="1.3" id="kotlin-tour-hello-world-exercise"}

|---|---|
```kotlin
fun main() {
    val name = "Maria"
    val age = 20
    println("$name tem $age anos")
}
```
{initial-collapse-state="collapsed" collapsible="true" collapsed-title="Solução do exemplo" id="kotlin-tour-hello-world-solution"}

## Próximo passo

[Tipos básicos](kotlin-tour-basic-types.md)

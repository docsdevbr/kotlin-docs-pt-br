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

# source_url: https://github.com/JetBrains/kotlin-web-site/blob/master/docs/topics/getting-started.md
# source_revision: beaf883c9759ff18049666e95b833b9da43c8ef9
# translation_status: ready
---

[//]: # (title: Comece a usar o Kotlin)

<tldr>
<p>Última versão do Kotlin:<b> <a href="%kotlinLatestWhatsnew%">%kotlinVersion%</a></b></p>
</tldr>

O Kotlin é uma linguagem moderna, concisa, multiplataforma e interoperável com
Java e outras linguagens.

É iniciante no Kotlin?
Faça nosso tour para aprender os fundamentos diretamente no seu navegador.

<a href="kotlin-tour-welcome.md"><img src="start-kotlin-tour.svg" width="700" alt="Iniciar o tour do Kotlin" style="block"/></a>

## Instale o Kotlin

O Kotlin está incluído em cada versão do
[IntelliJ IDEA](https://www.jetbrains.com/idea/download/) e do
[Android Studio](https://developer.android.com/studio).
Baixe e instale uma dessas IDEs para começar a usar o Kotlin.

## Escolha seu caso de uso do Kotlin

<tabs>

<tab id="console" title="Console">

Aqui você aprenderá a desenvolver uma aplicação de console e a criar testes
unitários com Kotlin.

1. **[Crie uma aplicação JVM básica com o assistente de projetos do IntelliJ IDEA](jvm-get-started.md).**

2. **[Escreva seu primeiro teste unitário](jvm-test-using-junit.md).**

</tab>

<tab id="backend" title="Backend">

Aqui você aprenderá a desenvolver uma aplicação backend com Kotlin no lado do
servidor.

* **Introduza o Kotlin em seu projeto Java:**

  * [Configure um projeto Java para trabalhar com Kotlin](mixing-java-kotlin-intellij.md)
  * [Adicione testes em Kotlin ao seu projeto Maven Java](jvm-test-using-junit.md)

* **Crie uma aplicação backend do zero com Kotlin:**

  * [Crie um serviço web RESTful com Spring Boot](jvm-get-started-spring-boot.md)
  * [Crie APIs HTTP com Ktor](https://ktor.io/docs/creating-http-apis.html)

</tab>

<tab id="cross-platform-mobile" title="Multiplataforma">

Aqui você aprenderá a desenvolver uma aplicação multiplataforma usando
[Kotlin Multiplatform](https://kotlinlang.org/docs/multiplatform/get-started.html).

1. **[Configure seu ambiente para desenvolvimento multiplataforma](https://kotlinlang.org/docs/multiplatform/quickstart.html).**

2. **Crie seu primeiro aplicativo para iOS e Android:**

   * Crie um aplicativo multiplataforma do zero e:
     * [Compartilhe a lógica de negócios mantendo a interface nativa](https://kotlinlang.org/docs/multiplatform/multiplatform-create-first-app.html)
     * [Compartilhe a lógica de negócios e a interface](https://kotlinlang.org/docs/multiplatform/compose-multiplatform-create-first-app.html)
   * [Faça seu aplicativo Android existente funcionar no iOS](https://kotlinlang.org/docs/multiplatform/multiplatform-integrate-in-existing-app.html)
   * [Crie um aplicativo multiplataforma usando Ktor e SQLDelight](https://kotlinlang.org/docs/multiplatform/multiplatform-ktor-sqldelight.html)

3. **Explore [projetos de exemplo](https://kotlinlang.org/docs/multiplatform/multiplatform-samples.html)**.

</tab>

<tab id="android" title="Android">

Para começar a usar Kotlin no desenvolvimento para Android, leia a
[recomendação do Google para começar com Kotlin no Android](https://developer.android.com/kotlin/get-started).

</tab>

<tab id="data-analysis" title="Análise de dados">

Desde a criação de pipelines de dados até a implantação de modelos de
aprendizado de máquina em produção, o Kotlin é uma excelente escolha para
trabalhar com dados e extrair o máximo valor deles.

1. **Explore e experimente seus dados:**

   * [DataFrame](https://kotlin.github.io/dataframe/overview.html) – uma
     biblioteca para análise e manipulação de dados.
   * [Kandy](https://kotlin.github.io/kandy/welcome.html) – uma ferramenta de
     plotagem para visualização de dados.

2. **Siga o Kotlin for Data Analysis no Twitter:** [KotlinForData](http://twitter.com/KotlinForData).

</tab>

</tabs>

## Obtenha suporte

Se você encontrar dificuldades ou problemas, peça ajuda no
![Slack](slack.svg){width=25}{type="joined"} Slack:
[solicite um convite](https://surveys.jetbrains.com/s3/kotlin-slack-sign-up) ou
relate um problema em nosso
[rastreador de issues](https://youtrack.jetbrains.com/issues/KT).

Se algo estiver faltando ou parecer confuso nesta página, por favor,
[compartilhe seu feedback](https://surveys.hotjar.com/d82e82b0-00d9-44a7-b793-0611bf6189df).

---
type: doc
layout: reference
category: "Introduction"
title: "Kotlin 用于服务器端开发"
---

# 使用 Kotlin 进行服务器端开发

Kotlin 非常适合开发服务器端应用程序，可以让你编写简明且表现力强的代码，
同时保持与现有基于 Java 的技术栈的完全兼容性以及平滑的学习曲线：

 * **表现力**：Kotlin 的革新式语言功能，例如支持[类型安全的构建器](type-safe-builders.html)<!--
   -->和[委托属性](delegated-properties.html)，有助于构建强大而易于使用的抽象。
 * **可伸缩性**：Kotlin 对[协程](coroutines.html)的支持有助于构建服务器端应用程序，
   伸缩到适度的硬件要求以应对大量的客户端。
 * **互操作性**：Kotlin 与所有基于 Java 的框架完全兼容，可以让你保持<!--
   -->熟悉的技术栈，同时获得更现代化语言的优势。
 * **迁移**：Kotlin 支持大型代码库从 Java 到 Kotlin 逐步迁移。你可以开始<!--
   -->用 Kotlin 编写新代码，同时系统中较旧部分继续用 Java。
 * **工具**：除了很棒的 IDE 支持之外，Kotlin 还为 IntelliJ IDEA Ultimate 的插件提供了框架特定的工具（例如
   Spring）。
 * **学习曲线**：对于 Java 开发人员，Kotlin 入门很容易。包含在 Kotlin 插件中的自动 Java 到 Kotlin 的转换器有助于迈出第一步。[Kotlin 心印](https://www.kotlincn.net/docs/tutorials/koans.html) 通过一系列互动练习提供了语言主要功能的指南。

## 使用 Kotlin 进行服务器端开发的框架

 * [Spring](https://spring.io) 利用 Kotlin 的语言功能提供[更简洁的 API](https://spring.io/blog/2017/01/04/introducing-kotlin-support-in-spring-framework-5-0)，
从版本 5.0 开始。[在线项目生成器](https://start.spring.io/#!language=kotlin)可以让你用 Kotlin 快速生成一个新项目。

 * [Vert.x](http://vertx.io) 是在 JVM 上构建响应式 Web 应用程序的框架，
为 Kotlin 提供了[专门支持](https://github.com/vert-x3/vertx-lang-kotlin)，包括[完整的文档](http://vertx.io/docs/vertx-core/kotlin/)。

 * [Ktor](https://ktor.kotlincn.net) 是 JetBrains 为在 Kotlin 中创建 Web 应用程序而构建的框架，利用协程实现高可伸缩性，并提供易于使用且合乎惯用法的 API。

 * [kotlinx.html](https://github.com/kotlin/kotlinx.html) 是可在 Web 应用程序中用于构建 HTML 的 DSL。
它可以作为传统模板系统（如JSP和FreeMarker）的替代品。

 * [Micronaut](https://micronaut.io/) is a modern, JVM-based, full-stack framework for building modular, easily testable microservice and serverless applications. It comes with a lot of built-in, handy features.
 
 * [Javalin](https://javalin.io) is a very lightweight web framework for Kotlin and Java which supports WebSockets, HTTP2 and async requests.

 * 通过相应 Java 驱动程序进行持久化的可用选项包括直接 JDBC 访问、JPA 以及使用 NoSQL 数据库。
对于 JPA，[kotlin-jpa 编译器插件](compiler-plugins.html#jpa-支持)使
Kotlin 编译的类适应框架的要求。

## 部署 Kotlin 服务器端应用程序

Kotlin 应用程序可以部署到支持 Java Web 应用程序的任何主机，包括 Amazon Web Services、
Google Cloud Platform 等。

要在 [Heroku](https://www.heroku.com) 上部署 Kotlin 应用程序，可以按照 [Heroku 官方教程](https://devcenter.heroku.com/articles/getting-started-with-kotlin)来做。

AWS Labs 提供了一个[示例项目](https://github.com/awslabs/serverless-photo-recognition)，展示了 Kotlin
编写 [AWS Lambda](https://aws.amazon.com/lambda/) 函数的使用。

谷歌云平台（Google Cloud Platform）提供了一系列将 Kotlin 应用程序部署到 GCP 的教程，包括 [Ktor 与 App Engine](https://cloud.google.com/community/tutorials/kotlin-ktor-app-engine-java8) 应用及 [Spring 与 App engine](https://cloud.google.com/community/tutorials/kotlin-springboot-app-engine-java8) 应用。此外，
还有一个[交互式代码实验室（interactive code lab）](https://codelabs.developers.google.com/codelabs/cloud-spring-cloud-gcp-kotlin)用于部署 Kotlin Spring 应用程序。

## Kotlin 用于服务器端的用户

[Corda](https://www.corda.net/) 是一个开源的分布式分类帐平台，由各大银行提供支持
，完全由 Kotlin 构建。

[JetBrains 账户](https://account.jetbrains.com/)，负责 JetBrains 整个许可证销售和验证<!--
-->过程的系统 100％ 由 Kotlin 编写，自 2015 年生产运行以来，一直没有重大问题。


## 下一步

* [使用 Http Servlet 创建 Web 应用程序](https://www.kotlincn.net/docs/tutorials/httpservlets.html)及<!--
-->[使用 Spring Boot 创建 RESTful Web 服务](https://www.kotlincn.net/docs/tutorials/spring-boot-restful.html)教程<!--
-->将向你展示如何在 Kotlin 中构建和运行非常小的 Web 应用程序。
* 关于更深入的介绍，请查看本站的[参考文档](index.html)及
[Kotlin 心印](https://www.kotlincn.net/docs/tutorials/koans.html)。
* Micronaut 还提供了很多详细的[指南](https://guides.micronaut.io/tags/kotlin.html)，展示了如何使用 Kotlin 构建微服务。

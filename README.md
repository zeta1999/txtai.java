# txtai: AI-powered search engine for Java

[![Version](https://img.shields.io/github/release/neuml/txtai.java.svg?style=flat&color=success)](https://github.com/neuml/txtai.java/releases)
[![GitHub Release Date](https://img.shields.io/github/release-date/neuml/txtai.java.svg?style=flat&color=blue)](https://github.com/neuml/txtai.java/releases)
[![GitHub issues](https://img.shields.io/github/issues/neuml/txtai.java.svg?style=flat&color=success)](https://github.com/neuml/txtai.java/issues)
[![GitHub last commit](https://img.shields.io/github/last-commit/neuml/txtai.java.svg?style=flat&color=blue)](https://github.com/neuml/txtai.java)

[txtai](https://github.com/neuml/txtai) builds an AI-powered index over sections of text. txtai supports building text indices to perform similarity searches and create extractive question-answering based systems. txtai also has functionality for zero-shot classification.

This repository contains Java bindings for the txtai API. Full txtai functionality is supported.

## Installation

Jitpack is the recommended way to integrate txtai with Java. See [this link](https://jitpack.io/) for how to install JitPack.

The following is an example adding txtai to a project's `build.gradle` file. The same attributes can be ported to other build systems per the JitPack link above.

```gradle
implementation 'com.github.neuml:txtai.java:v1.0.0'
```

txtai can also be manually built from GitHub.

```bash
git clone https://github.com/neuml/txtai.java
cd txtai.java
./gradlew jar
```

The JAR will be available in ./build/libs

## Examples
The examples directory has a series of examples that give an overview of txtai. See the list of examples below.

| Example     |      Description      |
|:----------|:-------------|
| [Introducing txtai](https://github.com/neuml/txtai.java/blob/master/examples/src/main/java/EmbeddingsDemo.java) | Overview of the functionality provided by txtai |
| [Extractive QA with txtai](https://github.com/neuml/txtai.java/blob/master/examples/src/main/java/ExtractorDemo.java) | Extractive question-answering with txtai |
| [Labeling with zero-shot classification](https://github.com/neuml/txtai.java/blob/master/examples/src/main/java/LabelsDemo.java) | Labeling with zero-shot classification |

txtai.java connects to a txtai api instance. See [this link](https://github.com/neuml/txtai#api) for details on how to start a new api instance.

Once an api instance is running, do the following to run the examples.

```
git clone https://github.com/neuml/txtai.java
cd txtai.java/examples
../gradlew embeddings|extractor|labels
```

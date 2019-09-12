---
title: Annot8
tagline: Structure from the unstructured
---

# Welcome to Annot8

Annot8 is a framework for extracting structured information from unstructured data. For a simple example, this could be extracting e-mail addresses from a collection of text documents, or faces from a collection of images.

## Terminology

* *Annotation* - Some information highlighted in Content, for example a span of text
* *Content* - A "view" on an Item, for example the text extracted from a Word document
* *Item* - A data object for processing, for example a Word document
* *Processor* - A processor is an Annot8 component that processes Content in some way, for example annotating e-mail addresses
* *Property - A property is a key-value pair on an Annot8 object (such as an Annotation, an Item or Content) which provides additional meta-data, for example the author of a document
* *Source* - An Annot8 component which creates new Item objects, for example by finding files in a folder on your hard drive

Read more about Annot8 concepts:

* [concepts/data.md] Data
* [concepts/components.md] Components

# Getting Started

The Annot8 framework is split into a number of different levels. If you just want to use the low level framework, you can do so by starting with `annot8-core`, but if you want to use the high level aspects and have access to a number of pre-built components then you probably want to start with `annot8-components`.

These are available through Maven Central (https://mvnrepository.com/artifact/io.annot8) or through the OSSHR Sonatype snapshot repository. You can add the snapshot repository to your POM via:

```
  <repositories>
    <repository>
      <id>oss-sonatype</id>
      <name>oss-sonatype</name>
      <url>https://oss.sonatype.org/content/repositories/snapshots/</url>
      <snapshots>
        <enabled>true</enabled>
      </snapshots>
    </repository>
  </repositories>
```

```

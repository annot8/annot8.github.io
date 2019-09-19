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

* [Data](concepts/data.md)
* [Components](concepts/components.md)

# Getting Started

The Annot8 framework is split into two repositories, each of which contain a number of projects.

* [Annot8](https://github.com/annot8/annot8) - This repository contains all the projects relating directly to the Annot8 framework, including default implementations of the framework interfaces.
* [Annot8 Components](https://github.com/annot8/annot8-components) - This repository contains processors and sources developed to work in the Annot8 framework

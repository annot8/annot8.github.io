# Data

## Items

Annot8 is about processing *Items*.  An Item is a holder for *Content*. 

An item could be anything but typically it's an something of significance:

* A file
* An email from an inbox
* An image

Through processing items can be broken down into sub items:

* A directory item could be divided down into its files.
* A video could be divided into its individual (image) frames.

The original item can be *discarded* (or continued to be processed)  

## Content

An Item can have multiple pieces of content. 

Content is a representation of data in the item. 

If we have an item which represents a file it could have: 

* File content (FileContent) which links to the original file on the file system
* Text content (Text) which contains the text extracted from the file
* One or more piece of image content which contain the diagrams in the file

Through processing content can be created and deleted from an item.

Let's assume the file is written in French, a processor might produce a translated version:

* Original Text content in French
* Translated Text content in English

## Annotation

We want to identify aspects within content which are of interest. 

This could be anything:

* A face in an image
* A word in text
* A point in a document where the topic changes
* A section of a video which is outdoors

We create annotations on content.  Annotations live in the AnnotationStore on Content.  

## Bounds

Annotations have bounds. The bounds of an annotation define which part of the content it applies to. 

Examples of bounds are:

* A word or words in a text document (Span Bounds)
* A position in a file (PositionBounds)
* An area of an image
* A frame of a video

## Groups

Often we have a assoication between Annotataions:

* Two annotated people (Bob and Robert) might be the same person
* A relation between a person and a place, (Bob-lives in-London)
* Technical information about annotations, for example, dependency parsing.

We can store this information in Groups.

Within a group, annotations have a role. For example, from the lives in relation example above:

* Bob is 'who'
* London is 'where'

You have have many annotations with the same role. Bob and Jane lived in London, or have roles which are missing, Bob and Jane lived in London in 2000.

Groups can link annotations accross differnt content within an item. We could have a group which capures that an annotated face in the image relates to the name in the caption. 

Groups live in the GroupStore on Item.

## Common elements: types, properties

Annotations and groups have types. These allow us to distinguish what the annotation or group is. 

Annotations, groups, etc have properties. These are a collection of additional data which relates to the element. For example, if we annotate a area of an image because it contains a particular object, we can use the properties to store information about that object.   






---
title: Markdown Basics
type: exploration
level: beginner
topics:
- markdown
- structured writing
- research-documentation
technologies: 
- markdown
---

# Markdown Basics

## Introduction

[Markdown](https://en.wikipedia.org/wiki/Markdown) is a lightweight markup language that allows us to create structured documents using plain text. Instead of relying on visual formatting tools—such as Word—Markdown uses a simple system of symbols to define headings, lists, links, images, quotations, and other elements.

Markdown files use the .md extension and can be opened with any ordinary text editor. Platforms such as GitHub can also render them into formatted documents.

In this exploration, we will learn the fundamental Markdown syntax and experiment with creating our first structured document.


## Where can you write Markdown?

Markdown is a writing format, not a particular application. You can create Markdown documents using different kinds of software: simple text editors, dedicated Markdown applications, code editors, or online services.

A Markdown document is a plain-text file, usually saved with the `.md` extension. This means that you are not tied to a particular application. You can create a document in one environment, open it in another, and continue editing it.

### Text editors

The simplest option is to use an ordinary text editor.

- **TextEdit** (macOS): switch to plain-text mode and save your document with the `.md` extension.
- **Notepad** (Windows): create a plain-text document and save it with the `.md` extension.

These applications allow you to write Markdown, although they do not provide a dedicated rendered preview.

### Dedicated Markdown applications

Some applications are specifically designed for writing and organizing Markdown documents.

- **Obsidian**: organizes Markdown files into interconnected collections of notes. It supports links, tags, backlinks, and graph views. Particularly useful for research notebooks and field diaries.
- **Typora**: offers a minimalist writing environment in which Markdown formatting is rendered as you type.
- **Joplin**: an open-source note-taking application that uses Markdown and supports notebooks, tags, and attachments.

- **MarkdownEditor**: a native app for iPad and iPhone dedicated to write and read markdowns. It is the one mainly used to write this project.

### Code editors

Code editors provide a more extensive environment for working with Markdown and other digital materials.

- **Visual Studio Code**: a free editor with built-in Markdown support, syntax highlighting, and a live preview. It is particularly useful when working with Markdown alongside CSV files, images, HTML, CSS, JavaScript, and other research materials. **This one is highly recommended for working around this lab**

### Online editors

You can also write Markdown directly in your browser.

- **StackEdit**: an online editor with a live preview.
- **Dillinger**: a simple browser-based Markdown editor with export options.

These services are useful for trying Markdown without installing additional software.

### Writing directly in GitHub

GitHub allows you to create and edit Markdown files directly in a repository. It automatically renders Markdown documents when you view them.

This makes GitHub more than a place to store finished documents: it can also become an environment for writing, documenting, organizing, revising, and sharing research materials.

### Choosing an environment

Different applications support different ways of working. You might use Obsidian to maintain a field diary, Visual Studio Code to work with Markdown and computational materials, and GitHub to version and publish your documents.

The important thing is that Markdown is portable: the document is not owned by the application in which it was created.

——

## 1. Creating a Markdown file

A Markdown document is simply a text file saved with the .md extension.

For example:

first-research-note.md

You can create one using a code editor, a plain text editor, or directly through GitHub.

The content is written as plain text, using Markdown syntax to indicate how different elements should be organized.

## 2. Heading

Headings organize the structure of a document. Markdown uses the hash symbol (#) to define different heading levels.

# Main heading
```
# Main heading
```

## Section heading

```
## Section heading
```

### Subsection heading
```
### Subsection heading
```

#### Smaller heading
```
#### Smaller heading
```

The number of hash symbols determines the heading level. One hash represents the main heading, two represent a section, and so on.

Experiment: Create a document about an observation and organize it using a main heading, two section headings, and at least one subsection.

## 3. Paragraphs and line breaks

Ordinary text becomes a paragraph. To create a new paragraph, leave an empty line between blocks of text.

Markdown generally treats consecutive lines as part of the same paragraph. A blank line creates a new paragraph.

Experiment: Write two short paragraphs describing a place, an encounter, or an observation.

## 4. Emphasis

Markdown allows us to emphasize text using asterisks or underscores.

*Italic text*
**Bold text**
***Bold and italic text***

Emphasis can help distinguish concepts, important observations, or particular expressions in a document.

Experiment: Write a short observation and use bold to highlight an important detail and italics to emphasize a concept or expression.

## 5. Lists

Markdown supports both unordered and ordered lists.

### Unordered lists

Use a hyphen (-), a plus sign (+), or an asterisk (*) to create a bullet point.

- Trees
- Benches
- River
- Footpath

### Ordered lists

Use numbers followed by periods.

1. Arrive at the location.
2. Observe the surroundings.
3. Record the encounter.
4. Take photographs.

Lists can help organize inventories, observations, materials, procedures, and sequences of events.

## 6. Blockquotes

Use the greater-than symbol (>) to create a blockquote.

> This is a sample of a blockquote.
> You can add multiple lines.

Blockquotes can be used for quotations, fragments of conversations, extracts from documents, or observations you want to distinguish from your own commentary.

Experiment: Include a short quotation or a fragment of speech in your research note.

## 7. Links

Markdown allows us to connect documents and external resources using hyperlinks.

The basic syntax is:

```
[Link text](https://example.com)
```

For example:

```
[GitHub](https://github.com)
```

[GitHub](https://github.com)

You can also link to another Markdown file in the same repository using a relative path:

```
[Previous observation](../previous-observation.md)
```

Links make it possible to connect research notes, references, images, datasets, and other materials.

Experiment: Add one link to an external resource and one link to another Markdown document.

## 8. Images

Images can be included using an exclamation mark followed by alternative text and the image path.

```![Description of the image](images/river-01.jpg) ```

The text inside the square brackets describes the image and can also help with accessibility.

If the image is stored in the repository, use its relative path.

Experiment: Add a photograph to your research note. Include a descriptive alternative text.

## 9. Horizontal rules

Three hyphens, asterisks, or underscores can create a horizontal rule.

---

Horizontal rules can help visually separate sections of a document.

## 10. Tables

Markdown allows us to create simple tables using vertical bars and hyphens.

```
| Time | Observation | Location |
|---|---|---|
| 16:00 | People sitting beneath trees | Riverbank |
| 16:30 | Increased pedestrian activity | Footpath |
| 17:00 | Shade extending over benches | Riverbank |
```

| Time | Observation | Location |
|---|---|---|
| 16:00 | People sitting beneath trees | Riverbank |
| 16:30 | Increased pedestrian activity | Footpath |
| 17:00 | Shade extending over benches | Riverbank |

Tables are particularly useful for presenting inventories, comparisons, classifications, and structured observations.

However, tables are not always the best format for fieldnotes. They can impose categories and relationships before we fully understand what is happening.

Experiment: Create a small table recording three observations. Consider what information becomes easier to compare and what details might be lost.

## 11. Code blocks

Code blocks allow us to display text or code without Markdown interpreting its contents as formatting.

Use three backticks before and after the block.

```javascript
const observation = "People sitting beneath trees";
console.log(observation);
```

You can specify a language after the opening backticks, such as javascript, python, html, or csv, to enable syntax highlighting on supported platforms.

Code blocks are useful for documenting programming experiments, displaying data structures, and including technical examples in research documentation.

## 12. Further possibilities

Markdown can do much more than format text. It can become a foundation for organizing research materials and developing interconnected collections of documents.

Once familiar with the basic syntax, we can explore:

* Writing structured fieldnotes.
* Adding metadata and frontmatter.
* Linking observations, photographs, and other research materials.
* Building a digital field diary.
* Maintaining documents through Git and GitHub.
* Using Markdown files as source material for other computational processes.

---
## Final reflection

Markdown is a simple format, but its implications for ethnographic research are worth exploring.

What happens when fieldnotes become structured text files? What possibilities emerge when observations can be linked, searched, reorganized, and versioned? What do we gain, and what might we lose, when we introduce structures into the practice of writing?

These questions will accompany the next explorations.
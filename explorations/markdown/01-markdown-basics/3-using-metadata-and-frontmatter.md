---
title: Using Metadata and Frontmatter
type: exploration
level: beginner
topics:
- markdown
- metadata
- frontmatter
- research-documentation
technologies: 
- markdown
- Yaml
Latest update: 2026-11-18
---

# Using Metadata and Frontmatter

## Exploring Metadata

A Markdown document contains written content, but it can also contain information describing the document itself. This information is called metadata.

For example, a field note might contain an observation made in a park in a neighborhood of a city, on a particular date, as part of a research project on urban transformation. We might also want to know who wrote it, which topics it concerns, whether it includes photographs, and whether it is an original entry or a revised document. Metadata makes this information explicit.

In this exploration, we introduce YAML frontmatter as a simple way to describe Markdown documents and experiment with its possibilities for organizing ethnographic research materials.

## What is frontmatter?

Frontmatter is a block of structured information commonly placed at the beginning of a Markdown document--each one of the files in this project has its own frontmatter--before its main content. It is usually written in [YAML](https://yaml.org), a human-readable format for representing structured information. A frontmatter block begins and ends with three hyphens:

`---`

  `title: An Afternoon Near the Sea`

  `date_observed: 2026-11-15`

  `location: Cunit`

  `topics:`

   `\- urban-heat`

   `\- shade`

   `\- public-space`

  `\---`

  `\# An Afternoon Near the Sea`

  `I arrived at the beach shortly after four in the afternoon.`

The information between the two sets of hyphens describes the document. The content following the second set of hyphens is the actual fieldnote.

Frontmatter is not part of the narrative itself. It provides a descriptive layer that can help us identify, organize, and retrieve documents.

## Working with YAML

As already introduced, YAML is a format for organizing information using readable text. Some basic elements are particularly useful when writing metadata.

### 1. Key-value pairs

A key identifies a piece of information, while its value provides the corresponding information.

`title: An Afternoon Near the Sea`
`location: Cunit`
`status: experimental`

Each line describes one attribute of the document.

### 2. Lists

When a document has several topics, methods, or technologies, we can use a list.

`topics:`

- `urban-heat`

- `shade`

- `public`

- `space`

The list belongs to the `topics` key.

### 3. Dates

Dates can be written in the [ISO](https://en.wikipedia.org/wiki/ISO_8601) format:

    date_observed: 2026-06-15

This format follows the order year-month-day, making dates easier to compare and sort.

### 4. Text values

Values containing spaces can be written without quotation marks, although quotation marks can be useful when values contain special characters.

    title: An Afternoon Near the River
    
    researcher: "Santiago Orrego"

The important thing is to maintain consistent formatting throughout a collection.

## Why use metadata in ethnographic research?

Metadata can help to describe different dimensions of a research document.

For example:

- **Identification:** What is this document? Does it have a unique identifier?

- **Chronology:** When did the observation take place? When was it written?

- **Location:** Where did the observation take place?

- **Research context:** Which project or investigation does it belong to?

- **Topics:** What subjects or phenomena does it address?

- **Methods:** What research practices or instruments were involved?

- **Media:** Does it contain photographs, audio, video, sketches, or other materials?

- **Status:** Is it a preliminary note, an ongoing record, or a completed document?

These dimensions can be described through metadata fields.

The metadata should reflect the nature of the document and the research context in which it was produced.

## Consistency and flexibility

Metadata becomes particularly useful when several documents belong to the same collection.

Imagine maintaining a field diary with fifty entries. If each entry uses different names for the same location, topic, or research method, organizing and comparing the documents becomes difficult.

**Consistency matters.**

For example, choose one term such as `urban-heat` and use it consistently rather than alternating between `heat`, `urban-heat`, `temperature`, and `urban-temperature` without a clear distinction.

At the same time, metadata should not become an exhaustive classification system. It is perfectly acceptable to leave some fields empty or introduce new ones when the research requires them.

The purpose is to make documents more useful, not to force every observation into a rigid schema.

## Important considerations

### Automatization is manual

Creating a frontmatter and adding metadata is a manual process. 

### Metadata is not automatically a database

Adding frontmatter to a Markdown document does not automatically make it searchable as a structured database.

The metadata is written in a structured format, but additional tools are needed to extract, index, compare, or visualize information across multiple documents.

This is where Markdown begins to connect with other computational practices, including CSV, JSON, scripts, and databases.

### GitHub and frontmatter

GitHub can store and display Markdown documents containing frontmatter, but it does not automatically turn every YAML field into searchable tags or database entries.

Frontmatter can be processed by other tools and publishing systems. For example, GitHub Pages uses Jekyll, which can interpret YAML frontmatter.

### Preserve the history of documents

Research documents can have several important dates:

- The date an observation took place.

- The date the document was originally written.

- The date it was digitized.

- The date it was subsequently revised.

These dates should not be confused.

Version-control systems such as Git can record changes to a document, but they do not necessarily preserve the original date of an observation or the creation date of a handwritten note.

If you digitize an existing field diary, preserve its original dates in the document metadata.

### Be careful with sensitive information

Metadata can also contain sensitive information. Exact coordinates, personal names, contact details, or identifying descriptions may expose research participants or vulnerable locations.

Consider what information should be included in a public repository and what should remain in private research materials.

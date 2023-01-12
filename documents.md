---
bibliography: co2rr.bib
---

Documents
==================

I think we should try using Markdown for the documents. It is simple, and supported by many editors. Notably, [Obsidian](https://obsidian.md/) supports it, and it has plugins for inserting citations from a bibtex file. There is some configuration required for this that has to be documented, e.g. use this plugin https://github.com/hans/obsidian-citation-plugin, and some settings in it for specifying the bibtex file. After that, we should be able to insert a citation like this [@koolen-2022-from-singl], using a keyboard shortcut (I had to assign it to C-] in Obsdian).

For each paper, you can have a specific document for a reference (Open it with C-S-o, which prompts you to search for it).

For an example topic document see [[screening-studies]].

## Citation syntax

We have to agree on a syntax. Bracketed pandoc syntax seems like a good choice. We should only use a syntax like this. This will be easy to parse later.
```
Blah blah [@smith04; @doe99].
```

## Why Markdown?

Markdown is simple, can be parsed for analysis, e.g. find all citations in a document for NLP purposes, and it can be converted to other formats including PDF and HTML, maybe even Word. It is also plain text, and future proof.

Many editors can work with Markdown files:
- Obsidian
- logseq
- Emacs/vim

In theory this means you choose how you do your writing. All of the options listed above can integrate with Bibtex databases for citations.

## Limitations

Obsidian is not currently used for writing scientific papers. It is not as advanced as [org-ref](https://github.com/jkitchin/org-ref) but it is much easier to set up. It is not easy to extend, and requires Java/Typescript skills to do that.

Obsidian supports some non-standard syntax, e.g. Wikilinks instead of standard Markdown links. That works fine in Obsidian, but is not supported in other editors, or in exports with pandoc.


# References
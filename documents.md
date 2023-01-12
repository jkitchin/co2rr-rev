Documents
==================

I think we should try using Markdown for the documents. It is simple, and supported by many editors. Notably, [Obsidian](https://obsidian.md/) supports it, and it has plugins for inserting citations from a bibtex file. There is some configuration required for this that has to be documented, e.g. use this plugin https://github.com/hans/obsidian-citation-plugin, and some settings in it for specifying the bibtex file. After that, we should be able to insert a citation like this [@koolen-2022-from-singl], using a keyboard shortcut (I had to assign it to C-]).

For each paper, you can have a specific document for a reference (Open it with C-S-o, which prompts you to search for it).

For an example topic document see [[screening-studies]].

## Why Markdown?

Markdown is simple, can be parsed for analysis, e.g. find all citations in a document for NLP purposes, and it can be converted to other formats including PDF and HTML, maybe even Word. It is also plain text, and future proof.

## Limitations

Obsidian is not currently used for writing scientific papers. It is not as advanced as [org-ref](https://github.com/jkitchin/org-ref) but it is much easier to set up. It is not easy to extend, and requires Java/Typescript skills to do that.



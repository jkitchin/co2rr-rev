Documents
==================
  
I think we should try using Markdown for the documents. It is simple, and supported by many editors. Notably, [Obsidian](https://obsidian.md/) and [logseq](https://github.com/logseq/logseq)supports it, and it has plugins for inserting citations from a bibtex file. There is some configuration required for this that has to be documented, e.g. use this plugin https://github.com/hans/obsidian-citation-plugin, and some settings in it for specifying the bibtex file. After that, we should be able to insert a citation like this [@koolen-2022-from-singl], using a keyboard shortcut (I had to assign it to C-] in Obsdian).
  
For each paper, you can have a specific document for a reference (Open it with C-S-o, which prompts you to search for it).  
  
For an example topic document see [[screening-studies]].

## Citation syntax
We have to agree on a syntax. Bracketed pandoc syntax seems like a good choice. We should only use a syntax like this.
```
Blah blah [@smith04; @doe99].
```

## Why Markdown?

Markdown is simple, can be parsed for analysis, e.g. find all citations in a document for NLP purposes, and it can be converted to other formats including PDF and HTML, maybe even Word. It is also plain text, and future proof.

Many editors can work with Markdown files:
- Obsidian
- logseq
- Emacs/vim
- VS Code  

In theory this means you choose how you do your writing. All of the options listed above can integrate with Bibtex databases for citations.

## Limitations

Obsidian/logseq are not currently used for writing scientific papers. They are not as advanced as [org-ref](https://github.com/jkitchin/org-ref) but are easier to set up. They are not easy to extend, and requires Java/Typescript skills to do that.

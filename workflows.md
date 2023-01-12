# Review workflow

I think the best strategy for a team review is the following:
1. Each user forks the literature review repo. That means everyone has their own copy.
2. They do some portion of work, e.g. review #1, review#2, writing, clean up, etc.
3. They commit their work to their repo, push it and make a pull request
4. Someone else on the team reviews the pull request and either iterate or approve and merge.

Workflow tools
=======================

These will be a set of scripts that automate as many things as can be done. For example, you might run a script (probably a Python script) that pulls new articles from the last month down, and converts them to a data file for review. Maybe this even runs automatically from a GitHUB action, and you just sync with it.

Then, you might run another command that presents the articles to you in a way that facilitates making decisions about where they go (e.g. discard or next step). For example, it might generate a task file that you interact with in an editor, or at the command line.

When you are done for the time being, you would run a command that checks in your work, and synchronizes it with the team repo.

## Exporting documents

We probably want to export the markdown files to some other format for reading, e.g. publish HTML files to GitHUB pages. This could be done with pandoc, for example, in an automated way. 

Here is a command to export all the files to HTML.

```
for i in *.md ; do echo "$i" && pandoc -C -s $i -o html/$i.html ; done
```

It leaves something to be desired, eg. it doesn't show figures and internal links that Obsidian uses non-standard syntax for.

## Utilities
1. Script that extracts bibtex entries from a Markdown file.
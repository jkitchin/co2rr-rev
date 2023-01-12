# Workflow tools

These will be a set of scripts that automate as many things as can be done. For example, you might run a script (probably a Python script) that pulls new articles from the last month down, and converts them to a data file for review. Maybe this even runs automatically from a GitHUB action, and you just sync with it.
  
  Then, you might run another command that presents the articles to you in a way that facilitates making decisions about where they go (e.g. discard or next step). For example, it might generate a task file that you interact with in an editor, or at the command line.
  
  When you are done for the time being, you would run a command that checks in your work, and synchronizes it with the team repo.

## Exporting documents
We probably want to export the markdown files to some other format for reading, e.g. publish HTML files to GitHUB pages. This could be done with pandoc, for example, in an automated way.

## Utilities
1. Script that extracts bibtex entries from a Markdown file.

# Limitations and challenges
Git may be a challenge for new users. We can probably automate a lot, but merge conflicts are probably inevitable.
I think the pull request mechanism is important for team cohesion and communication, but it also adds some friction.

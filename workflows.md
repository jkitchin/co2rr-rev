# Workflow tools

These will be a set of scripts that automate as many things as can be done. For example, you might run a script (probably a Python script) that pulls new articles from the last month down, and converts them to a data file for review. Maybe this even runs automatically from a GitHUB action, and you just sync with it.
  
Then, you might run another command that presents the articles to you in a way that facilitates making decisions about where they go (e.g. discard or next step). For example, it might generate a task file that you interact with in an editor, or at the command line.
  
When you are done for the time being, you would run a command that checks in your work, and synchronizes it with the team repo or creates a review pull request.

For the first step, there will be a directory called something like bucket-1 that contains data files. There will be a command that opens a data file for you to process what is in it, which either means discard it, or move it to bucket-2. There will be different ways we add things to bucket-1. Some ways will be scripts that automatically pull entries from databases online. Some ways will be for manual additions.

Bucket-2 will also have data files for papers that need to be read. These will also be either discarded or put into the database. Now is the time to create paper notes for the ones that go in the database, and to add them to a topic document. There will be a command to identify entries in the database that are not in the topic documents or that are missing not

## Exporting documents

We probably want to export the markdown files to some other format for reading, e.g. publish HTML files to GitHUB pages. This could be done with pandoc, for example, in an automated way.

## Utilities

1. Script that extracts bibtex entries from a Markdown file.



# Limitations and challenges

Git may be a challenge for new users. We can probably automate a lot, but merge conflicts are probably inevitable. I have had them just working from home and the office already.

I think the pull request mechanism is important for team cohesion and communication, but it also adds some friction.

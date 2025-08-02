# Gambling and Stats Book

View Book Here: https://bodhi-root.github.io/gambling-stats-bookdown/

This project began as an R project using R markdown, but has since been converted to a Quarto book format.

You can preview the book by running the following command in your terminal:

```
quarto preview
```

NOTE: Make sure your virtual environment is activated before running the command.

This will create the output files for the book and open a web browser for you to view them. Changes made to your files will automatically trigger a re-create of the respective page.

When you are ready to render the book, use the following command:

```
quarto render
```

## Environment Setup

If you're using codespaces, this should be relatively easy. The devcontainer is setup to use the docker image "ghcr.io/mcanouil/quarto-codespaces:latest". This includes the Quarto CLI as well as Python, R, and Julia. The only thing we have to do is add our Python dependencies. This is done automatically by the devcontainer via the "postCreateCommand":

```
pip install -r requirements.txt
```

requirements.txt is build from requirements.in using:

```
uv pip compile requirements.in -o requirements.txt
```

## Old Notes (Bookdown)

This is yet another attempt by me to record some of my favorite applications of statistics and computer analysis: gambling.  I've tried this before in different formats: notebooks, Word, Confluence.  I'd like to build it in a way that is:

1. Easy to edit and add new topics
2. Easy to convert to new formats, if needed
3. Persistent

I think bookdown will meet these needs, allowing me to build the content of the book in markdown and persit it in GitHub.  Let's see how it goes.

When creating this book I began with the simple "bookdown-demo", deleted some files, altered some titles, and then started writing.

NOTE: [Cool reference on equations in R Markdown](https://www.montana.edu/rotella/documents/502/MarkdownEqnExamples.Rmd) and a [Visual Editor](http://visualmatheditor.equatheque.net/VisualMathEditor.html).

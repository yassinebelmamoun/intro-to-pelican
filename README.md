# Introduction

Pelican is a static site generator written in Python.

This document is a short and practical introduction to Pelican. Its main goal is to get you up and running within 30 minutes.

# Installation

The following librairies are needed:

``` shell
pipenv install pelican markdown typogrify
```

# Quick start

Once the installation of dependencies completed, we can start our pelican project:

``` shell
pelican-quickstart
```

Once all questions replied to, multiple files will be generated including:

- Makefile
- pelicanconf.py
- publishconf.py
- tasks.py

# Generate output

``` shell
pelican -s pelicanconf.py -o output content
```

# Write your first article in Markdown content

Write your first article following this structure in the `output/` folder:

``` markdown
title: myTitle
slug: my-slug
tags: tag-1, tag-2, tag-3
summary: The summary goes here

The content will go here
```

# Run the local server

``` shell
make serve
```

And open your browser: http://localhost:8000

# References

Pelican website: https://docs.getpelican.com/en/stable/

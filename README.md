# cmd-style-guide

My personal style guide for Batch scripts.

## Background

Batch scripts are a bit of a nightmare to read. There are so many different ways to do the same thing in a script. For example, there are three different ways to write comments:

```cmd
rem Like this
:: Like this
%= or like this =%
```

Other points of contention are case-insensitivity, treating quotes as regular characters, and lack of basic facilities like `case` or `while` statements. This document attempts to define a standard way of writing these constructs, so that other humans can more easily read your Batch script.

**IMPORTANT:** It should be noted that for now, this is very much a work in progress. For now, all I'll be doing is listing my preferred way of doing these things in a bunch of bullet points. As this document grows, I'll eventually organize these into coherent sections and eventually a full-fledged style guide. This is **not** complete by any means.

## Content

- Variable names and label names should be camelCase. For example:

  ```cmd
  :: good
  :setFileContents
  set "fileContents=..."
  
  :: bad
  :set_file_contents
  set "FileContents=..."
  ```

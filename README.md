# Quarto CLI Bugs

This repository is just to demonstrate quarto bugs.

Really, there are two problems described in this repo, but they are separate
bugs and should probably be treated as separate even though they conbine in a
very frustrating way.

## Issue 1: Case-insensitivity in quarto filenames in the CLI

If I have a directory with a file named `foo.qmd` and run
`quarto render Foo.qmd`, quarto should give me an error rather than generating
unexpected output files.

## Issue 2: Incorrect output directory

When the user has explicitly set an `output-dir` in `_quarto.yml`, it should be
respected even when quarto decides to override the name of the output file.

# Pandoc-citeproc demonstration

Pandocize this file using:
s
    pandoc -F pandoc-citeproc do-citeproc.md -o do.pdf

And get this ref [@super-test]

---
link-citations: true
references:
  - id: super-test
    author: me
    date: now
    title: Just do it. A citeproc test.
    url: www.cidco.ca
...

# Style guide for PowerShell-Docs

## Titles/Headings

* Titles/headings (anything preprended by \#) should be followed with a newline
* Only the first letter of a title and any proper nouns in that title should be capitalized
* Only use \# style headers (as opposed to = or \- style headers):

### Correct

```
# Header 1

## Header 2

### Header 3
```

### Incorrect

```
Header 1
========

Header 2
--------

### Header 3
```

## Syntax

* All PowerShell syntax blocks should use ```powershell, even if they're only one line
* Output emitted by PowerShell should be wrapped in its own syntax block, using only ```

## Lists

* Do not end list items with a period (unless they contain multiple sentences)
* If your list contains multiple sentences, consider using a header 3/4/5 (as applicable) underneath your primary idea

# Installation

Install *remotes* if you don't already have it:

```r
install.packages('remotes')
```

Install the *readmarkdown* package:

```r
remotes::install_github('yea-hung/readmarkdown')
```

# Example

Define the Markdown table:

```r
markdown_table<-"
| state | capital | area |
| --- | --- | --- |
| California | Sacramento | 163700 |
| Massachusetts | Boston | 10565 |
| Illinois | Springfield | 57914 |
"
```

Read the table:

```r
read_markdown(markdown_table)
```

Equivalently, read the table using using native piping:

```r
markdown_table |> read_markdown()
```

# Details

This package uses base R.

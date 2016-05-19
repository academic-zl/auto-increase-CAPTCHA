## 论文

这里是论文所在目录，内容在 `main.md` 中。LaTeX样式在 `cqu.latex` 和 `cqu.cls` 中定义。

## 编译命令

### Markdown -> pdf

```shell
pandoc --filter pandoc-crossref --filter pandoc-citeproc --biblio reference.bib --csl chinese-gb7714-2005-numeric.csl --latex-engine=xelatex --template=cqu.latex main.md -o main.pdf
```

### Markdown -> tex

```shell
pandoc --filter pandoc-crossref --filter pandoc-citeproc --biblio reference.bib --csl chinese-gb7714-2005-numeric.csl --latex-engine=xelatex --template=cqu.latex main.md -o main.tex
```

### Markdown -> docx

```shell
pandoc --filter pandoc-crossref --filter pandoc-citeproc --biblio reference.bib --csl chinese-gb7714-2005-numeric.csl --latex-engine=xelatex  main.md -o main.docx
```


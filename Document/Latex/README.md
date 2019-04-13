## Run the following commands in target folder

### Fonts

1. tex-gyre

    [https://ctan.org/pkg/tex-gyre?lang=en](https://ctan.org/pkg/tex-gyre?lang=en)

2. th-sarabun-new

    [https://www.f0nt.com/release/th-sarabun-new/](https://www.f0nt.com/release/th-sarabun-new/)

### To compile
```
 xelatex -interaction=nonstopmode -file-line-error -synctex=1 MathCS-tutorial.tex
```

### To generate bibliography
```
bibtex MathCS-tutorial.aux
```

### To generate .eps file from .pdf file
```
    pdf2eps [no_page_in_pdf] [figure_file_name]
```

### For example
```
    pdf2eps 1 er_diagram
```
This command will generate "er_diagram.eps" from page no. 1 of "er_diagram.pdf".

### วิธีการรัน
```
Compilation: *require XeTeX
  [When citations/references are changed.]
  1. xelatex -interaction=nonstopmode -file-line-error -synctex=1 MathCS-tutorial.tex
  2. bibtex MathCS-tutorial.aux
  3. xelatex -interaction=nonstopmode -file-line-error -synctex=1 MathCS-tutorial.tex
  4. xelatex -interaction=nonstopmode -file-line-error -synctex=1 MathCS-tutorial.tex

  [When citations/references are not changed.]
  1. xelatex -interaction=nonstopmode -file-line-error -synctex=1 MathCS-tutorial.tex
```

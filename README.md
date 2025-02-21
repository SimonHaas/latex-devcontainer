# latex devcontainer

This is a latex environment inside a devcontainer.

Tested with:
- github codespaces

.tex files should be rendered automatically, if not you can do it manually:

``` shell
latexmk -output-directory=output -pdf hello-world.tex

# cleanup temporary files
latexmk -output-directory=output -c

# cleanup temporary files including .pdf
latexmk -output-directory=output -C
```

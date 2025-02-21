# latex devcontainer

[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://codespaces.new/SimonHaas/latex-devcontainer?quickstart=1)

This is a latex environment inside a devcontainer.

Tested with:
- github codespaces
- docker
    - ubuntu
    - WSL with docker desktop on Windows
    - Mac with Apple Silicon

I could not get it to run with:
- podman
    - ubuntu
    - WSL with podman desktop
    - WSL with `apt install podman`

.tex files should be rendered automatically, if not you can do it manually:

``` shell
latexmk -output-directory=output -pdf hello-world.tex

# cleanup temporary files
latexmk -output-directory=output -c

# cleanup temporary files including .pdf
latexmk -output-directory=output -C
```

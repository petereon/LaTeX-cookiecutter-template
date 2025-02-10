# What is this
This is the closest I've been able to get to Overleaf in VSCode with but a few tools and extensions to get a similar experience.

## Tooling Setup
Install `xelatex`. In MacOS you can get it as a part of `mactex-no-gui`:
```sh
brew install --cask mactex-no-gui
```

Install `just`:
```sh
brew install just
```

Install `watchexec`:
```sh
brew install watchexec
```

Install `cookiecutter`:
```sh
brew install cookiecutter
```

## VSCode setup
Install [`vscode-pdf` extension](https://marketplace.visualstudio.com/items?itemName=tomoki1207.pdf) (this is included in the cookiecutter and VSCode will offer to install it for you)

## Creating a new project

You can clone the repository using the `cookiecutter`:
```sh
cookiecutter https://github.com/petereon/LaTeX-cookiecutter-template
```

It will ask you for a project name, a prefered language and you are set up.

## Overleaf experience

Open the folder you have created in the VSCode and in the terminal run:
```
just watch render
```

The folder `build` will be created. Right-click the PDF file within the folder and `Open to the Side`.

Whenever you edit the `main.tex` file the PDF will be rerendered and updated in the view to see the results.

### Shortcuts

When editing any `.tex` file within the workspace you can start typing any of the following to create a boilerplate for some of the annoying to type out structures.
- `section`
- `subsection`
- `cite`
- `begin`
- `math`
- `textit`
- `textbf`
- `figure`
- `newline`
- `newpage`
- `itemize`
- `item`
- `table`



My Neovim config with lazy.nvim inspiered by [[https://github.com/cpow/neovim-for-newbs]].

## Colorscheme
catppuccin but with transparent background

## Package Manager
lazy.nvim

## Includes Following Plugins:
- code completion + lsp
- indent-blankline
- lualine
- neotree
- neoscroll
- noice
- none-ls
- notify
- telescope
- treesitter
- vimtex

And more

# How to use:

### Requirements
Neovim 0.9 or newer, git, a C compiler for treesitter (gcc or clang), ripgrep for telescope and nodejs for the LSP servers. For vimtex you also want a TeX distribution and a PDF viewer.

### Install
The config goes into `~/.config/nvim`. If something is already there back it up first:

```bash
mv ~/.config/nvim ~/.config/nvim.bak
```

Then clone the repo into that path:

```bash
git clone <repo-url> ~/.config/nvim
```

### First start
Just run `nvim`. lazy.nvim pulls itself on the first start and installs all plugins automatically. Wait until lazy is done, then restart once.

For the LSP servers open `:Mason` and pick what you want, or run `:MasonInstall <server>`. Treesitter parsers come via `:TSInstall <language>`.


#### kleine randnotiz für potentielle profs:

neovim basiert auf vim. vim basiert auf vi.

der unterschied ist am ende nur die config. mit neovim hat man lua zum configurieren.

##### so ein paar shortcuts für den anfang:

Navigation (normal mode, hier kann man nicht tippen nur navigieren):

- h -> cursor nach links
- j -> cursor nach unten
- k -> cursor nach oben
- l -> cursor nach rechts

In der navigation bearbeiten (normal mode editing):

- dd -> zeile löschen (ist in der zwischenablage von vim)
- yy -> zeile kopieren
- p -> aus zwischenablage einfügen

Ich will schreiben (insert mode):
- i -> links vom cursor kann man jetzt tippen
- a -> rechts vom cursor kann man jetzt tippen
- I -> ganz am anfang (links) der zeile kann man tippen
- A -> ganz am ende der zeile (rechts) kann man tippen
- o -> neue zeile unter der aktuellen und man kann direkt tippen
- O -> neue zeile über der aktuellen und man kann direkt tippen
- ESCAPE -> insert mode verlassen zum normal mode

"How to exit vim":
mit `:` kann man 'commands' eingeben. man braucht erstmal nur `:w` zum speichern. `:q` zum quitten (warum auch immer). 
das kann man aber auch kombinieren zu `:wq` zum speichern UND schließen. `:wqa` speichert und schließt ALLE offenen fenster (in nvim)

Extras:
- Strg+N -> öffnet sidepanel (toggle)






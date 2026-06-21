
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

-------------------------------------------------------------------------

## kleine randnotiz für potentielle profs

neovim basiert auf vim. vim basiert auf vi.
der unterschied ist am ende nur die config. 
mit neovim hat man lua zum configurieren.

eine weitere sache. 
man kann die vim keybinds in fast allen code editoren nutzen (vscode, intellij, etc) aber wenn man neovim (`nvim`) oder vim nutzt hat man die meisten vorteile und man lernt es am besten! 
wenn man die maus benutzt macht man was falsch :)

### so ein paar shortcuts für den anfang

**Navigation** (normal mode, hier kann man nicht tippen nur navigieren):

| taste | macht |
| --- | --- |
| `h` | cursor nach links |
| `j` | cursor nach unten |
| `k` | cursor nach oben |
| `l` | cursor nach rechts |
| `w` | ein wort nach vorne |
| `b` | ein wort zurück |
| `0` | an den anfang der zeile |
| `$` | ans ende der zeile |
| `gg` | ganz nach oben in die datei |
| `G` | ganz nach unten in die datei |

**In der navigation bearbeiten** (normal mode editing):

| taste | macht |
| --- | --- |
| `dd` | zeile löschen (ist in der zwischenablage von vim) |
| `yy` | zeile kopieren |
| `p` | aus zwischenablage einfügen |
| `x` | einzelnes zeichen löschen |
| `u` | letzte änderung rückgängig |
| `Strg+r` | rückgängig wieder rückgängig (redo) |

**Ich will schreiben** (insert mode):

| taste | macht |
| --- | --- |
| `i` | links vom cursor kann man jetzt tippen |
| `a` | rechts vom cursor kann man jetzt tippen |
| `I` | ganz am anfang (links) der zeile kann man tippen |
| `A` | ganz am ende der zeile (rechts) kann man tippen |
| `o` | neue zeile unter der aktuellen und man kann direkt tippen |
| `O` | neue zeile über der aktuellen und man kann direkt tippen |
| `ESCAPE` | insert mode verlassen zum normal mode |

**Markieren** (visual mode):

| taste | macht |
| --- | --- |
| `v` | von hier ab zeichenweise markieren |
| `V` | ganze zeilen markieren |
| `y` | das markierte kopieren |
| `d` | das markierte löschen |

**Suchen** (im normal mode):

mit `/text` sucht man nach `text` und springt mit `n` zum nächsten treffer, mit `N` zum vorherigen. die suche leeren tut man hier mit `<leader>h` (leader ist die leertaste).

### "How to exit vim"

mit `:` kann man 'commands' eingeben. man braucht erstmal nur `:w` zum speichern. `:q` zum quitten (warum man quitten will weiß ich nicht).
das kann man aber auch kombinieren zu `:wq` zum speichern UND schließen. `:wqa` speichert und schließt ALLE offenen fenster (in nvim). will man rausspringen ohne zu speichern dann `:q!`.

### neo-tree (der dateibaum)

mit `Strg+N` macht man den dateibaum auf und zu (kommt bei mir rechts raus). drin navigiert man ganz normal mit `j` und `k`, mit ENTER macht man einen ordner auf oder eine datei auf. 
um zwischen den 2 fenster zu springen `STRG+L` zum rechten fenster und `STRG+H` zum linken fenster.

| taste | macht |
| --- | --- |
| `a` | neue datei anlegen. packt man am ende ein `/` hin wird es ein ordner (zb `lua/` macht den ordner, `lua/test.lua` die datei) |
| `d` | löschen |
| `r` | umbenennen |
| `c` | kopieren |
| `x` | ausschneiden |
| `p` | einfügen |

### Extras

| taste | macht |
| --- | --- |
| `Strg+N` | öffnet sidepanel (toggle) |


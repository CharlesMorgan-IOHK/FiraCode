# Fira Code: Mono-Spaced Font with Programming Ligatures
## Awesome for all of your IDEs By Nikita Prokopov

<img src="https://dl.dropboxusercontent.com/u/561580/imgs/fira_code_logo.svg">

### Problem

Programmers use a lot of symbols, often encoded with several characters. For human brain sequences like `->`, `<=` or `:=` are single logical token, even if they take two or three places on the screen. Your eye spends non-zero amount of energy to scan, parse and join multiple characters into a single logical one. Ideally, all programming languages should be designed with full-fledged Unicode symbols for operators, but that’s not the case yet.

### Solution

Fira Code is a Fira Mono font extended with a set of ligatures for common programming multi-character combinations. This is just a font rendering feature: underlying code remains ASCII-compatible. This helps to read and understand code faster. For some frequent sequences like `..` or `//` ligatures allow us to correct spacing.

### Fira Code (with ligatures):

<img src="./showcases/all_ligatures.png" />

Compare to Fira Mono (without ligatures):

<img src="./showcases/no_ligatures.png" />

### Editor support

Do **not** work:

- Atom ([bug](https://github.com/atom/atom/issues/6055))
- SublimeText ([vote here](http://sublimetext.userecho.com/topic/433445-opentype-support-ligatures-curly-quotes-contextual-and-alternate-symbols/))
- Intellij Idea ([vote here](https://youtrack.jetbrains.com/issue/IDEA-127539))
- XCode
- iTerm 2 ([feature request](https://gitlab.com/gnachman/iterm2/issues/3568))
- OS X Terminal.app
- Emacs
- gVim, MacVim
- Eclipse ([vote here](https://bugs.eclipse.org/bugs/show_bug.cgi?id=398656))

Do work:

- Visual Studio
- TextMate 2
- QtCreator
- LightTable ([instructions](https://github.com/LightTable/LightTable/issues/1459#issuecomment-57366504))
- BBEdit — enter this command in a terminal to enable ligatures:  
  `defaults write com.barebones.bbedit "EnableFontLigatures_Fira Code" -bool YES`
- RStudio
- Chocolat

Should work (copied from [Hasklig README](https://github.com/i-tu/Hasklig)):

- Geany
- gEdit
- Kate
- Konsole
- KWrite
- Smultron
- Vico

_Note:_ I’m not a font designer, and Fira Code is built in sort of [a hacky way](https://github.com/mozilla/Fira/issues/62) from OTF version of Fira Mono. Please forgive me if it doesn’t work for you. Help will be greatly appreciated.

### Code examples

Ruby:

<img src="./showcases/ruby.png" />

JavaScript:

<img src="./showcases/javascript.png" />


Erlang:

<img src="./showcases/erlang.png" />

Go:

<img src="./showcases/go.png" />

Haskell:

<img src="./showcases/haskell.png" />

### Alternatives

Another monospaced fonts with ligatures:

- [Hasklig](https://github.com/i-tu/Hasklig) (free)
- [PragmataPro](http://www.fsd.it/fonts/pragmatapro.htm) (€59)
- [Monoid](http://larsenwork.com/monoid/) (free)

### Credits

This work is based on OFL-licensed [Fira Mono font](https://github.com/mozilla/Fira). Original Fira Mono font was not changed, only extended

Fira Code was inspired by [Hasklig font](https://github.com/i-tu/Hasklig): Ligatures for Haskell code

### Changelog

**0.6**:

Redrawn from Fira Mono 3.204 (slightly heavier weight)

Added:

`**` `***` `+++` `--` `---` `?:`  
`/=` `/==` `.=` `^=` `=~` `?=` `||=` `|=`  
`<<<` `<=<` `-<<` `-<` `>-` `>>-` `>=>` `>>>`  
`<*>` `<|>` `<$>` `<+>`  
`<!--` `{-` `-}` `/**`  `\\` `\\\`
`..<` `??` `|||` `&&&` `<|` `|>`  
  
and Powerline support

**0.5**: `#{` `~-` `-~` `<==` `==>` `///` `;;` `</`

**0.4**:

- Added `~=` `~~` `#[`
- Rolled back `&&` and `||` to more traditional look
- `===` and `!==` are now rendered with 3 horisontal bars

**0.3**: `~@` `#?` `=:=` `=<`

**0.2.1**: Fixed width of `&&` and `||`

**0.2**: `-->` `<--` `&&` `||` `=>>` `=/=`

**0.1**

`>>=` `=<<` `<<=` `->>` `->` `=>` `<<-` `<-`  
`===` `==` `<=>` `>=` `<=` `>>` `<<` `!==` `!=` `<>`  
`:=` `++` `#(` `#_`  
`::` `...` `..` `!!` `//` `/*` `*/` `/>`  


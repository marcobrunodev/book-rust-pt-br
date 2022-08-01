# A Linguagem de Programção Rust

![Build Estatos](https://github.com/rust-lang/book/workflows/CI/badge.svg)

Este repositório contem a fonte do livro "A Linguagem de Programação Rust".

[O livro está disponível em formato de *dead-tree* na *No Starch Press*][nostarch].

[nostarch]: https://nostarch.com/rust

Você pode também ler o livro de graça e online. Por favor, veja o livro de Rust nas versões [estável], [beta] ou [nightly]. Esteja ciente que questões já podem ter sido resolvidas nessa versão, uma vez que aquelas versão são atualizadas com menos freqüência.

[estável]: https://doc.rust-lang.org/stable/book/
[beta]: https://doc.rust-lang.org/beta/book/
[nightly]: https://doc.rust-lang.org/nightly/book/

Veja as [releases] para download apenas dos códigos apresentados no livro.

[releases]: https://github.com/rust-lang/book/releases

## Requisitos

Para buildar o livro é necessário o [mdBook], idealmente a mesma versão que rust-lan/rust usa, [este aquivo][rust-mdbook]. Para instalar o mdBook:

```bash
$ cargo install mdbook --vers [version-num]
```

[mdBook]: https://github.com/rust-lang-nursery/mdBook
[rust-mdbook]: https://github.com/rust-lang/rust/blob/master/src/tools/rustbook/Cargo.toml

```bash
$ cargo install mdbook --vers [version-num]
```

## Buildando

Para buildar o livro, execute:

```bash
$ mdbook build
```

O livro estará no subdiretório `book`. Para verificar, abra o arquivo `book/index.html` no seu navegador: 

_Firefox:_
```bash
$ firefox book/index.html                       # Linux
$ open -a "Firefox" book/index.html             # OS X
$ Start-Process "firefox.exe" .\book\index.html # Windows (PowerShell)
$ start firefox.exe .\book\index.html           # Windows (Cmd)
```

_Chrome:_
```bash
$ google-chrome book/index.html                 # Linux
$ open -a "Google Chrome" book/index.html       # OS X
$ Start-Process "chrome.exe" .\book\index.html  # Windows (PowerShell)
$ start chrome.exe .\book\index.html            # Windows (Cmd)
```

Para todas os testes:

```bash
$ mdbook test
```

## Description

Simple Haskell subset interpreter on Haskell itself.

_Код простого интерпретатора подмножества языка Haskell на самом Haskell._

https://habrahabr.ru/post/335366/

## Installation

```
sudo apt-get install haskell-platform alex happy
```

## Build

```
alex Lex.x
happy Synt.y
ghc Interpreter.hs
```

## Usage

```
./Interpreter
```

Test examples:

```
let a = 2 in a*2`
4
```

```
let a = 8 in (let b = a - 1 in a*b)
56
```
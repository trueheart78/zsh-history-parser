# ZSH History Parser

A parser for the ZSH history file that can help you identify commands to alias.

Built in Ruby.

## Setup

Requires no gem installs.

```sh
ln -s history_parser ~/bin/history_parser
```

## Usage

```sh
./history_parser
```

### Example

You can pass in the minimum command length to identify, as well as the number of results you
would like to see.

The default command with no arguments is akin to the following:

```
./history_parser 4 20
```

Does it's best to tell you the most used commands that meet the minimum length requirement.
_You should consider aliasing those commands_.

```
./history_parser
Top 20 most used commands (min length: 4)
[bundle] 77
[rails] 65
[brew] 46
[rake] 38
[echo] 37
[mkdir] 33
[psql] 32
[sudo] 29
[less] 28
[mysql] 27
[command] 23
[ping] 20
[whatis] 18
[touch] 17
[clear] 17
[open] 13
[tail] 12
[head] 11
[history] 11
[passwd] 11
[whoami] 10
```

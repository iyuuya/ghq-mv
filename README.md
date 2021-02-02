# ghq-mv

move repository (when repository owner transfer and else)

## Usage

```
ghq-mv src dest [remote]

```
#### option
- [remote] default value is`origin`

### Examples
#### Full path
```
$ ghq-mv github.com/iyuuya/ghq-mv github.com/for-you/ghq-mv-2
```

#### Short path
host is github.com when not specified host.

```
$ ghq-mv iyuuya/ghq-mv for-you/ghq-mv-2

same

$ ghq-mv github.com/iyuuya/ghq-mv github.com/for-you/ghq-mv-2
```

#### When very short dest
same owner when not specified owner.

```
ghq-mv iyuuya/ghq-mv ghq-mv-2"

same

ghq-mv github.com/iyuuya/ghq-mv github.com/iyuuya/ghq-mv-2
```

## Requirements
- ruby 2.6 or higher
- ghq (**Use ghq root first value**)
- git

```
[ghq]
root = ~/ghq <--- Choose this script
root = ~/go/src/
```

## Installation
### Git
```
git clone https://github.com/iyuuya/ghq-mv 
cd ghq-my
ln -s $PWD/ghq-my PATH_TO/bin:ghq-mv
```


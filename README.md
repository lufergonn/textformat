# TextFormat

TextFormat is a Python library for data cleaning.

## Installation

Use the package manager [pip](https://pip.pypa.io/en/stable/) to install textformat.

```bash
pip install textformat
```
or

```bash
pip install -i https://test.pypi.org/simple/ textformat
```

## Usage

```python
from textformat import TextFormat

t = TextFormat()

t.tUrl('ejemplo de https://github.com url') 
# return: ejemplo de  url

t.fReplace('El acento grรกfico o tilde es un signo ortogrรกfico') 
# return: El acento grafico o tilde es un signo ortografico

t.fEmoji('Some examples of emojis are ๐, ๐ง๐ปโโ๏ธ, ๐, ๐, ๐, ๐, ๐, โฅ๏ธ, ๐, and ๐') 
# return: Some examples of emojis are , , , , , , , ๏ธ, , and

t.fTag('ejemplo de #pruebaTag')
# return: ejemplo de prueba tag

t.fFormat('Eejemplo 123de formato {รฑ45', 'a-z')
# return: ejemplo de formato

# t.fTweet('tweet') --> Sin # o @ al inicio
# t.format('tweet') --> Todas las funciones anteriores
```

## License
[MIT](https://choosealicense.com/licenses/mit/)

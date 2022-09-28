# Clipette
Python clipboard utility that works natively on python with its inbuilt modules to exchange data with the windows clipboard. Designed specifically to be used for Blender (for [ImagePaste](https://github.com/Yeetus3141/ImagePaste)).

## Usage
Must call `open_clipboard()` before using any clipboard function. Preferably through an `if` statement.
Should call `empty_clipboard()` before setting any data to clipboard.
Must call `close_clipboard()` at the end.

Example (to get unicode text from clipboard):
```
from . import clipette

if clipette.open_clipboard():
    text = clipette.get_UNICODETEXT()
    print(text)
    clipette.close_clipboard()
```

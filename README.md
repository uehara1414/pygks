# pygks
Python GetKeyState module free from win32api and win32con module

Additionally it contains is_any_pressed and is_all_pressed function.

## How To Install
    pip install git+https://github.com/uehara1414/pygks.git

It works only on Windows

## Example Usage

```python
    >>> import pygks
    >>> pygks.GetKeyState(pygks.VK_A)
    True
    >>> pygks.is_any_pressed(pygks.VK_A, pygks.VK_B, pygks.VK_C)
    False
    >>> pygks.is_all_pressed(pygks.VK_CONTROL, pygks.VK_SHIFT, pygks.VK_Q)
    True
```

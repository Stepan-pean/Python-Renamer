# Pyren
*files renamer in console Bash*

Current version 1.5, use Python 3.2+, no compiled

**Features:**
- help and safe input arguments
- text GUI
- works with regular expressions and filenames containing dots
- fixed duplicate new filenames (added '(copy)' to filename)
- methods:
- - **`ins`** insert pattern at position
- - **`rem`** remove all from position to position
- - **`rep`** replace pattern by pattern
- modes (switches):
- - **`w`** write mode
- - **`s`** short output format
- - **`r`** recursive mode

**Examples:**

- `pyren ins -4 'any string'`

  'abcd.ef.xyz' --> 'abcd.efany string.xyz' in only simulation mode

- `pyren rem 2 100 -sw`

  'abcd.ef.xyz' --> 'ab' in short output format, write mode

- `pyren rep ^[0-9][0-9] '' -rn`

  '12 a1bcd00' --> ' a1bcd00' in recursive, only simulation mode
  
**How to install**

As superuser (sudo) save file **pyren** into `/bin` and set `chmod 755`. Now you may any directory open in bash and write `pyren`.

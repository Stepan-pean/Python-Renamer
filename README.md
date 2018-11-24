# Pyren
*files renamer in console Bash*

Current version 1.3, use Python 3.2+, no compiled

**Features:**
- help and safe input arguments
- text GUI
- works with regular expressions and filenames containing dots
- fixed duplicate new filenames (using char '_' added before last dot)
- methods:
- - insert pattern at position
- - remove from position to position
- - replace pattern by pattern
- modes:
- - simulation
- - short output format
- - recursive

**Examples:**
- `pyren ins -4 'any string' -n`
'abcd.ef.xyz' --> 'abcd.efany string.xyz' in simulation
- `pyren rem 2 100 -s`
'abcd.ef.xyz' --> 'ab' in short output
- `pyren rep ^[0-9][0-9] '' -rn`
'12 a1bcd00' --> ' a1bcd00' in recursive, simulation

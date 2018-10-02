# FindHiddenMessage
Find and decode hidden messages in BitCore's (BTX) blockchain explorer.

# Usage
Decode messages of BitCore block ranges between 1 and 20:

```bash
$ python3 FindHiddenMsgBlockchain.py -s 1 -f 20 -r n
```
If nothing was wrong, you'll have 20 new files in each one of them the decoded message hidden in the blocks.

## special regex
* ``-r y`` to filter the output and have only human readable characters
* ``-r n`` to have the converted output without modifying it

# Help

```sh
$ python3 FindHiddenMsgBlockchain.py -h

usage: FindHiddenMsgBlockchain.py [-h] -s START -f FINAL -r REGEX

This script can decode hidden messages in BitCore's block raw transactions

optional arguments:
  -h, --help            show this help message and exit
  -s START, --start START
                        First index of BitCore's block range
  -f FINAL, --final FINAL
                        Last index of BitCore's block range
  -r REGEX, --regex REGEX
                        Catch only human readable characters
```

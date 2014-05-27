JazzyDicts
==========

Mirror of JazzyDicts repository


About
-----

These utilities are basically conversions of munch/unmunch from the
official MySpell sources.

They are used to convert MySpell dictionaries to original word lists and the
other way round.

Build instructions for wordlist2myspell and myspell2wordlist utilities
----------------------------------------------------------------------

Under Linux run the following to create exacutables:

gcc -O2 -owordlist2myspell -I. wordlist2myspell.c

or

gcc -O2 -omyspell2wordlist -I. myspell2wordlist.c


After that to see the correct syntax, run:

./wordlist2myspell

or

./myspell2wordlist

You should see an output such as:

./myspell2wordlist
correct syntax is:
myspell2wordlist dic_file affix_file

Example:

./myspell2wordlist ./en_EN-pack/en_US/en_US.dic en_affix.dat > jazzy_dics/en_US_dictionary.txt

en_US.dic file has been taken from OpenOffice project https://wiki.openoffice.org/wiki/Dictionaries

Lastly the affix file for English has been taken from https://github.com/bpieber/Cuis-Smalltalk-StyledTextEditor/tree/master/scowl-7.1/speller/aspell
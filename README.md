JazzyDicts
==========

Mirror of JazzyDicts (sourceforge.net/projects/jazzydicts)

Pack of tools to convert myspell dictionaries to Jazzy word list format and vice versa. 

For dictionaries, the OpenOffice project has a number of them  at wiki.services.openoffice.org/wiki/Dictionaries


About
-----

These utilities are basically conversions of munch/unmunch from the
official MySpell sources.

They are used to convert MySpell dictionaries to original word lists and the
other way round.

Build instructions for wordlist2myspell and myspell2wordlist utilities
----------------------------------------------------------------------

Under Linux run the following to create exacutables:

    gcc -O2 -omyspell2wordlist -I. myspell2wordlist.c

or

    gcc -O2 -owordlist2myspell -I. wordlist2myspell.c


These will create exacutables myspell2wordlist and wordlist2myspell. When you run the exacutables without any parameter it shows the correct syntax:

    ./myspell2wordlist
    correct syntax is:
    myspell2wordlist dic_file affix_file

Example usage:

    ./myspell2wordlist ./en_EN-pack/en_US/en_US.dic ./en_affix.dat > ./jazzy_dics/en_US_dictionary.txt

For more dictionary packs you can visit OpenOffice project wiki at https://wiki.openoffice.org/wiki/Dictionaries

Lastly the affix file for English has been taken from https://github.com/bpieber/Cuis-Smalltalk-StyledTextEditor/tree/master/scowl-7.1/speller/aspell

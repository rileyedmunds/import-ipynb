## Motivation

Suppose you want to import the contents of A.ipynb into B.ipynb

## How to use

Place import_ipynb.py and both ipynb files in the same directory. Then, in the B.ipynb:

>import import_ipynb

>import A

Congratulations! You can not run any functions defined in A.ipynb, from B.ipynb!

## How it works

Essentially, the code in import_nb.py allows you to 'import' ipynb files. This entails:

1. load the notebook document into memory
2. create an empty Module
3. execute every cell in the Module namespace

Note that since every cell in the A.ipynb is executed when you import the the file, A.ipynb should only contain classes and function definitions (otherwise you'll end up loading all variables and data into memory).
 





# iapack
**iapack** is a small utility program that converts compiled inverse assemblers for HP logic analyzers (a.k.a. `.R`-files) into files readable by the logic analyzer.

## Installation
On Unix-like operating systems, simply run these commands:
```bash
git clone https://github.com/meyer-ac/iapack
cd iapack
g++ -o iapack iapack.cpp
```

**WARNING: ** This software has only been tested under a Debian 12 setup together with the HP 1663E logic analyzer.

## Usage
The `iapack` utility expects an input file (the `.R`-file), a name for the output file (by convention the same as the input file without the extension) and a short description, which will be displayed in the file browser of the logic analyzer. Example:
```bash
iapack -i I8086_I.R -o I8086_I -d "IA for the 8086"
```
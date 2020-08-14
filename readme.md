# btools-qmake

> _Distributed under the same licenses as original repo_

- Maintained minimal necessary hand picked QMake source code files cloned from  of https://github.com/qt/qtbase
- Choose a brach to see
	- QMake source code
	- Build instructions
- See [Rreleases](https://github.com/codemodify/btools-qmake/releases) for binaries for each platform


#### Examples
- C
```sh

# https://doc.qt.io/qt-5/qmake-variable-reference.html#sources
SOURCES = main.c

# https://doc.qt.io/qt-5/qmake-variable-reference.html#headers
HEADERS = procol.h

# https://doc.qt.io/qt-5/qmake-variable-reference.html#template
TEMPLATE = app

# https://doc.qt.io/qt-5/qmake-variable-reference.html#config
CONFIG = release warn_on cmdline
CONFIG-= qt

# https://doc.qt.io/qt-5/qmake-variable-reference.html#libs
LIBS=-levent

# https://doc.qt.io/qt-5/qmake-variable-reference.html#target
TARGET=server

# https://doc.qt.io/qt-5/qmake-variable-reference.html#destdir
DESTDIR=bin
```

- `qmake -o Makefile qmake.pro && make && make clean && rm Makefile .qmake.stash`

# ginit
ginit is a simple initializer for projects - creates minimum required files to start and initializes an empty git project for the specified language.

## Usage
`ginit lang`
`-pn --projectname` sets the name of the project
`-d --dir` creates a directory where git is initiated and eventual template files appear
`-l --libraries` creates a buildfile with required information for specified library

## Currently implemented languages
* c with make

## Currently implemented libraries
* raylib

## C project
### Make options

make builds everything in src
make clean cleans the build folder

### Folder structure
```
projectname
├── Makefile
└── src
    └── main.c
```
After running make
```
projectname
├── Makefile
├── build
│   └── main.o
├── projectname
└── src
    └── main.c
```


# Intel 4001 emulation

This was built to learn a little about CPU emulation following a guide:

1. https://megalomaniacbore.blogspot.com/2014/04/virtual-cpu-in-c-4001-cpu.html
2. https://megalomaniacbore.blogspot.com/2014/04/write-your-own-virtual-cpu-in-c-4001.html
3. https://megalomaniacbore.blogspot.co.uk/2014/04/loadsave-virtual-cpu-memory-state.html
4. https://megalomaniacbore.blogspot.co.uk/p/virtual-cpu-house-keeping-following.html

## Build
Just run `make` - simple.

## Run
`./4001` will bring up an interactive session with the various things you can do!

## Commands map

| op code | command   | explanation                                                                |
|---------|-----------|----------------------------------------------------------------------------|
| 0       | HALT      | Ends program                                                               |
| 1       | LOAD0     | Loads the following byte into register 0                                   |
| 2       | LOAD1     | Loads the following byte into register 1                                   |
| 3       | ADD       |                                                                            |
| 4       | BEEP      | Makes a beep                                                               |
| 5       | STORE     | Stores the contetent of register 0 to the address denoted by the next byte |
| 6       | PRINT     | Print the data from the address                                            |
| 7       | CLEAR0    |                                                                            |
| 8       | CLEAR1    |                                                                            |
| 9       | JUMPTO    |                                                                            |
| 10      | JUMPEQUAL |                                                                            |
| 11      | COPY0     |                                                                            |
| 12      | COPY1     |                                                                            |
| 13      | CLEAR     |                                                                            |
| 14      | MULTIPLY  |                                                                            |

underflow/overflow will not be dealt with

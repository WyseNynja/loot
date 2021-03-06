# Loot

Easily divide treasure between a party as fairly as possible.

An interactive mode will be written eventually. For now, as the game progresses, add what they find to the end of the command. Whenever the party decides to split the loot, press enter and the program will do its calcualtions.


# Quick Setup with Docker

1. Install Docker from https://www.docker.com/

2. Run the following command in your terminal:
```bash
docker run --rm -it bwstitt/loot -n 4 90cp 700sp 2000gp 18pp "1 chicken"
```

# Setup without Docker

To install all of the requirements in a virtualenv:
```bash
. setup.source_me
```

Upgrading requirements:
```bash
pip install pip-tools
pip-compile requirements.in
pip install -U -r requirements.txt -e .
```

To enter the virtualenv:
```bash
. env/bin/activate
```

Example run:

```bash
$ loot -n 4 90cp 700sp 2000gp 18pp "1 chicken"
split 18 pp into 4 piles of 4 with 2 leftover...
giving 1 of 2 pp to the poorest character...
giving 1 of 1 pp to the poorest character...
giving 1 of 2000 gp to the poorest character...
giving 1 of 1999 gp to the poorest character...
giving 1 of 1998 gp to the poorest character...
giving 1 of 1997 gp to the poorest character...
giving 1 of 1996 gp to the poorest character...
giving 1 of 1995 gp to the poorest character...
giving 1 of 1994 gp to the poorest character...
giving 1 of 1993 gp to the poorest character...
giving 1 of 1992 gp to the poorest character...
giving 1 of 1991 gp to the poorest character...
giving 1 of 1990 gp to the poorest character...
giving 1 of 1989 gp to the poorest character...
giving 1 of 1988 gp to the poorest character...
giving 1 of 1987 gp to the poorest character...
giving 1 of 1986 gp to the poorest character...
giving 1 of 1985 gp to the poorest character...
giving 1 of 1984 gp to the poorest character...
giving 1 of 1983 gp to the poorest character...
giving 1 of 1982 gp to the poorest character...
giving 1 of 1981 gp to the poorest character...
split 1980 gp into 4 piles of 495 with 0 leftover...
split 700 sp into 4 piles of 175 with 0 leftover...
giving 1 of 1 chicken to the poorest character...
giving 1 of 90 cp to the poorest character...
giving 1 of 89 cp to the poorest character...
giving 1 of 88 cp to the poorest character...
giving 1 of 87 cp to the poorest character...
giving 1 of 86 cp to the poorest character...
giving 1 of 85 cp to the poorest character...
giving 1 of 84 cp to the poorest character...
giving 1 of 83 cp to the poorest character...
giving 1 of 82 cp to the poorest character...
giving 1 of 81 cp to the poorest character...
giving 1 of 80 cp to the poorest character...
giving 1 of 79 cp to the poorest character...
giving 1 of 78 cp to the poorest character...
giving 1 of 77 cp to the poorest character...
giving 1 of 76 cp to the poorest character...
giving 1 of 75 cp to the poorest character...
giving 1 of 74 cp to the poorest character...
giving 1 of 73 cp to the poorest character...
giving 1 of 72 cp to the poorest character...
giving 1 of 71 cp to the poorest character...
giving 1 of 70 cp to the poorest character...
giving 1 of 69 cp to the poorest character...
giving 1 of 68 cp to the poorest character...
giving 1 of 67 cp to the poorest character...
giving 1 of 66 cp to the poorest character...
giving 1 of 65 cp to the poorest character...
giving 1 of 64 cp to the poorest character...
giving 1 of 63 cp to the poorest character...
giving 1 of 62 cp to the poorest character...
giving 1 of 61 cp to the poorest character...
split 60 cp into 4 piles of 15 with 0 leftover...

The loot divided equally :)
Character 0 gets 56275 cp worth of valuables:
- 5 pp
- 495 gp
- 175 sp
- 1 chicken
- 15 cp
Character 1 gets 56275 cp worth of valuables:
- 5 pp
- 495 gp
- 175 sp
- 25 cp
Character 2 gets 56275 cp worth of valuables:
- 4 pp
- 505 gp
- 175 sp
- 25 cp
Character 3 gets 56275 cp worth of valuables:
- 4 pp
- 505 gp
- 175 sp
- 25 cp
```


# Todo

 * [ ] Command to add more types of valuables to games yamls (and export them)
 * [ ] If a valuable type isn't recognized, prompt for its value and then save that for later calls
 * [ ] Rename the main function to split and add functions for adding new games and valuables
 * [ ] Clean up ~/.cache during docker runs


# Authors

- Bryan Stitt <bryan@stitthappens.com>


# License

The MIT License (MIT)
Copyright (c) 2016 Bryan Stitt

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

# bww2abc

`bww2abc` is a simple tool to convert **.bww** files (Bagpipe Writer format) into **.abc** notation.

Many bagpipe tunes are available in **.bww** format here:  
👉 [Bagpipe Tunes Collection](https://bagpipetunes.intertechnics.com/)  

For more information about **ABC notation**, see:  
👉 [ABC notation reference](http://moinejf.free.fr/)

---

## Features

- Convert `.bww` files to `.abc`
- Simple command-line usage
- Available as a global command with `npm link`
- Works with any `.bww` tune
- Compatible with ABC tools, viewers, and editors

---

## Requirements

- [Node.js](https://nodejs.org/) (v14 or higher recommended)
- npm (comes with Node.js)

---

## Installation

Clone the repository and install globally with npm:

```bash
git clone https://github.com/your-username/bww2abc.git
cd bww2abc
npm link
This will create a symbolic link from npm’s global binaries directory to your local script.
Result: the bww2abc command becomes available globally on your machine.

Usage
Convert a tune from .bww to .abc:

bash
Copier le code
bww2abc tune.bww > tune.abc
Examples
Example 1: Convert a simple tune
bash
Copier le code
bww2abc AmazingGrace.bww > AmazingGrace.abc
Output (AmazingGrace.abc):

abc
Copier le code
X:1
T:Amazing Grace
M:3/4
L:1/8
K:D
D2 | F2 A2 B2 | A4 D2 | ...
Example 2: Using node directly (without linking)
bash
Copier le code
node bww2abc.js ScotlandTheBrave.bww > ScotlandTheBrave.abc
Example 3: Batch conversion
Convert all .bww files in a folder into .abc:

bash
Copier le code
for f in *.bww; do
  bww2abc "$f" > "${f%.bww}.abc"
done
Development
You can run the script directly without linking:

bash
Copier le code
node bww2abc.js tune.bww > tune.abc
Contributing
Contributions are welcome!
If you’d like to improve this project:

Fork the repository

Create a new branch (git checkout -b feature/my-feature)

Commit your changes (git commit -m "Add my feature")

Push to the branch (git push origin feature/my-feature)

Open a Pull Request

License
This project is licensed under the MIT License.
See the LICENSE file for details.

Author
Developed and maintained by [Your Name].

ABC notation reference: http://moinejf.free.fr/

Bagpipe tunes in .bww format: https://bagpipetunes.intertechnics.com/

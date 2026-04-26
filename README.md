# 🧬 Mutagen - Bitcoin Puzzle Solver

**🔍 Description**: A tool for mutating private keys from previous Bitcoin puzzles to find solutions for subsequent ones using bit-flipping mutations.

## ✨ Idea

Takes a private key from a previous puzzle (e.g. `000...5749f` for Puzzle 19) and the next puzzle's hash160 address, then performs controlled bit mutations to efficiently search the solution space.

## 🚀 Installation

git clone [[https://github.com/MikeWazovksy/Mutagen.git](https://github.com/RohaCode/Mutagen.git)](https://github.com/RohaCode/Mutagen.git)

cd Mutagen

make

## 💻 Basic solve:

./mutagen -p 38 -t 8 -f 21

## 🔑 With custom key:

./mutagen -p 38 -t 8 -f 21 -k 123456

## 🔒 With fixed bits:

./mutagen -p 38 -t 8 -f 21 -k 123456 -x 4

## 🏁 Default settings:

./mutagen -h

## 🛠 **Command Options**

| 🟢 **Option**   | 🟡 **Description**                       |
| --------------- | ---------------------------------------- |
| `-p, --puzzle`  | Puzzle number (20-101)                   |
| `-t, --threads` | CPU threads to use                       |
| `-f, --flips`   | Override default flip count              |
| `-k, --key`     | Custom base private key                  |
| `-x, --exclude` | Number of fixed prefix bits (default: 0) |

## 🔧 **Optimizations**

- **AVX2** accelerated cryptography
- Multi-threaded with **OpenMP**
- Batched processing for **cache efficiency**
- Intelligent bit mutation patterns

## 👏 **Credits**

- _**Idea**: Roha 💡 [![Donate](https://img.shields.io/badge/donate-Bitcoin-ff9900)](https://blockchair.com/bitcoin/address/bc1qa3c5xdc6a3n2l3w0sq3vysustczpmlvhdwr8vc)
- _Thanks for the help, **NoMachine1**!_ 🔧 [![Donate](https://img.shields.io/badge/donate-Bitcoin-ff9900)](https://blockchair.com/bitcoin/address/bc1qdwnxr7s08xwelpjy3cc52rrxg63xsmagv50fa8)

✨ **Happy solving!**  
If you find this useful, please ⭐️ the repo!  
And if you'd like to support the project, you can donate 💰

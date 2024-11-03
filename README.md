---

# Snake

This is a clone of the legendary Snake game.

![snake.png](https://github.com/arunava-12/Snake_in_8086/blob/main/snake.png)

I created this version in pure x86 assembly language for the DOS operating system. It can be run in DosBox on modern systems. This is a 16-bit retro game designed to work on anything compatible with an Intel 8086 processor or newer. The graphics are rendered in the classic 13H mode with a resolution of 320x200 pixels, using a custom color palette and screen buffering. Fonts utilize the BIOS's built-in glyphs from system memory, while sprites and images were generated with a custom tool to convert them into byte arrays.

## How to Compile It

The precompiled version, `snake.com`, is included in the folder, so you can directly run it in DosBox. If you'd like to build it yourself, follow these steps:

1. **Install NASM (Netwide Assembler)**:
   - On Windows, download and install NASM from the [official website](https://www.nasm.us/).

2. **Compile the Assembly Code**:
   - Open Command Prompt.
   - Navigate to the folder where `snake.asm` is located.
   - Run the following command:
     ```bash
     nasm -f bin snake.asm -o snake.com
     ```

## How to Run It

1. **Clone this repository** or download `snake.com` into a folder.

2. **Install DosBox**:
   - Download and install [DosBox](https://www.dosbox.com/) for Windows.

3. **Run DosBox** and mount the directory containing `snake.com`:
   - In DosBox, enter:
     ```bash
     MOUNT D D:\path\to\snake\folder
     D:
     snake.com
     ```

### Controls

- **Arrow Keys**: Control the snake's direction (Up, Down, Left, Right)
- **ESC**: Quit the game
- **A**: Show game information
- **P**: Pause the game

---

### Personal Note

To run the game in DosBox on your system:

1. Run the following in DosBox:
   ```bash
   MOUNT D D:\coaproject
   D:
   snake.com
   ```

2. First, convert the `.asm` file to `.com` using Command Prompt:
   ```bash
   nasm -f bin snake.asm -o snake.com
   ```

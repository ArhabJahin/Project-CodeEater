# HELLO WORLD | Python Alphabet Search Animation

A beginner-friendly Python terminal project that builds **HELLO WORLD** one letter at a time. Instead of printing the message directly, the program searches through uppercase letters from **A to Z**, keeping each correct letter as it finds the next one.

## How it works

1. `range(65, 91)` generates the ASCII values for uppercase **A–Z**.
2. `chr(val)` converts each value into a character.
3. Nested `for` loops test letters in sequence until they match **H**, **E**, **L**, **L**, **O**, **W**, **O**, **R**, **L**, and **D**.
4. `time.sleep(0.05)` introduces a short delay so you can watch the search progress in the terminal.
5. After reaching **HELLO WORLD**, the program pauses briefly and starts again because it runs inside `while True`.

The program prints the letters it tries, not just the final message.

## Example terminal output

```text
A
B
C
...
H
HA
HB
HC
...
HE
HEA
HEB
...
HEL
...
HELLO W
...
HELLO WORLD
HELLO WORLD
...
```

*Output shortened for readability. The actual program prints many more intermediate lines and repeats the completed message.*

## Run locally

**Requirements:** Python 3. No external libraries are needed.

1. Save the Python code as `hello_world.py`.
2. Open a terminal in that folder.
3. Run:

   ```bash
   python hello_world.py
   ```

   On systems where Python 3 uses a separate command, run `python3 hello_world.py`.

4. Press **Ctrl + C** to stop the infinite loop.

## Concepts practiced

- Python `while` and nested `for` loops
- `range()` and `chr()`
- ASCII character codes
- `if` conditions and `break`
- `print()` with `end=""`
- Timing delays with the built-in `time` module

## Notes

- This is a learning experiment, not an efficient way to print text.
- The program uses hard-coded checks for each letter in **HELLO WORLD**.
- The variable `start_time` records the start time but is not used to calculate or display elapsed time.
- The outer `while True` loop means the animation keeps restarting until you stop it.

## Possible improvements

- Replace the deeply nested loops with a reusable function.
- Accept any target phrase as input.
- Show the search on one terminal line instead of printing every attempt on a new line.
- Use `start_time` to report elapsed time.
- Add an option to run the animation only once.

## License

You may add a license file if you want to specify how others can reuse your code.

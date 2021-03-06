# arduino-morse-code-led

A beginner _hello world_ project to blink the on board LED of the Arduino Uno using the Rust programming language.

To use your own morse code, change the following line from `src/main.rs`:

```rust
const MORSE_CODE: &str = "...";
```

## Building the Source

#### Clone this repo

```sh
# Using GitHub CLI
gh repo clone brianwow/arduino-morse-code-led
# Or, using git
git clone https://github.com/brianwow/arduino-morse-code-led
```

#### Install the dependencies

```sh
pacman -S avr-libc avr-gcc avrdude # Arch Linux
sudo apt install avr-libc gcc-avr avrdude # Ubuntu

cargo install ravedude
```

#### Allow writing to Arduino

Run this whenever you get a permission error while running the code:

```sh
sudo chmod a+rw /dev/ttyACM0
```

#### Run

```sh
cargo run
```

---

This project was generated using [avr-hal-template](https://github.com/Rahix/avr-hal-template).

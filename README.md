# rofipass: Orchestrate your Passwords

`rofipass` is an efficient `rofi` script designed to complement the [passwordstore](https://www.passwordstore.org/). This tool integrates the functionalities of `pass`, `pass-otp`, and `pass-tomb` within `rofi`, enabling you to access your passwords swiftly and effortlessly.

<div align="center"><a href="https://github.com/janpstrunn/elegantvagrant/tree/main/rofi">
  <img src="./assets/pass-rofi.png" alt="pass-rofi image">
  <p>pass-rofi with Elegant Vagrant Theme</p>
</a>
</div>

## Features

- **Password Management**: Create, copy, and delete passwords and OTP password with ease using your preferred `$EDITOR`.
- **Tomb Management**: Open and close a `tomb` seamlessly.

## Requirements

- [pass](https://www.passwordstore.org/)
- [pass-otp](https://github.com/tadfisher/pass-otp)
- [pass-tomb](https://github.com/roddhjav/pass-tomb)
- `rofi`

## Installation

```
git clone https://github.com/janpstrunn/rofipass
cd rofipass
chmod 700 src/rofipass
mv src/rofipass "$HOME/.local/bin"
```

## Usage

```
  ---------------------------------------------------
  ---------------------rofi-pass---------------------
  ---------------------------------------------------
  -------------A rofi extension for pass-------------
  ---------------------------------------------------

Usage: pass-rofi [options] <command> [arguments]

Options:
  -f             Force swap restrictions
  -h             Display this help message and exit
  -l             Default password length on generation
  -t             Default terminal emulator (for tomb)
  -v             Display the current version number

Commands:
  help                     Display this help message and exit
  version                  Display the current version number

Examples:
  rofipass -f -l 72 -t kitty
```

## Notes

This script has been only tested in a Linux Machine.

## License

This repository is licensed under the MIT License, a very permissive license that allows you to use, modify, copy, distribute and more.

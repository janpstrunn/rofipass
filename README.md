# rofipass: Orchestrate your Passwords

`rofipass` is an efficient `rofi` script designed to complement the [passwordstore](https://www.passwordstore.org/). This tool integrates the functionalities of `pass`, `pass-otp`, and `pass-tomb` within `rofi`, enabling you to access your passwords swiftly and effortlessly.

<div align="center"><a href="https://github.com/janpstrunn/elegantvagrant/tree/main/rofi">
  <img src="https://git.disroot.org/janpstrunn/images/raw/branch/main/pass/2025-05-16-rofipass.webp" alt="pass-rofi image">
  <p>pass-rofi with Elegant Vagrant Theme</p>
</a>
</div>

## Features

- **Password Management**: Create, copy, and delete passwords and OTP password with ease using your preferred `$EDITOR`.
- **Tomb Management**: Open and close a `tomb` seamlessly.

## Requirements

- [pass](https://www.passwordstore.org/)
- [pass-otp](https://github.com/tadfisher/pass-otp)
- [pass-tomb](https://github.com/roddhjav/pass-tomb) (optional)
- [rofi](https://github.com/davatorium/rofi)
- [zbar](https://github.com/mchehab/zbar) (to add OTP)

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
  -f             Lift swap restrictions (for tomb)
  -h             Display this help message and exit
  -l             Default password length on generation
  -t             Default terminal emulator (for tomb)
  -v             Display the current version number

Commands:
  help                     Display this help message and exit
  version                  Display the current version number

Examples:
  rofipass -f -l 72 -t foot
```

### Managing the Files

`pass` does not impose any limitations on how the files should be written, but it will always return the first line of the file as the password. `pass-otp`, whatsoever will look for the OTP key in the very last line. Any string in between won't be used, thus can have any data.

`rofipass` also has a way to grab some data from the encrypted file. If a line starts with `email=` it will recognize that, and will allow to copy the email to the clipboard.

## Notes

This script has been only tested in a Linux Machine.

## License

This repository is licensed under the MIT License, a very permissive license that allows you to use, modify, copy, distribute and more.

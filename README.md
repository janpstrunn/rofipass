# rofipass: A rofi script for passwordstore

`rofipass` is a `rofi` script, meant to be used alongside [passwordstore](https://www.passwordstore.org/), not to be confused with [pass](https://github.com/janpstrunn/pass).

It's a tool that combines all the `pass` and [pass-otp](https://github.com/tadfisher/pass-otp) functionalities within `rofi` to allow you to easily get the password and OTP you need faster than anyone else.

## Requirements

- [pass](https://www.passwordstore.org/)
- [pass-otp](https://github.com/tadfisher/pass-otp)
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
./rofipass
```

## Notes

This script has been only tested in a Linux Machine.

## License

This repository is licensed under the MIT License, a very permissive license that allows you to use, modify, copy, distribute and more.

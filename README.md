[busted](https://github.com/Olivine-Labs/busted) wrapper for testing neovim plugin

## Requirements
- neovim

## Installation

`luarocks --lua-version=5.1 install vusted`

## Usage

```console
$ vusted
ok 1 - vusted can use vim module
printed
ok 2 - vusted can print
1..2
```

### Helper functions

See [vusted.helper](https://github.com/notomo/vusted/blob/master/lua/vusted/helper.lua)'s function comments.

### Environment variables

- `VUSTED_NVIM`
    - vusted uses this command to execute neovim.
    - default: `nvim`
- `VUSTED_ARGS`
    - vusted uses this arguments to execute neovim.
    - default: `--headless --clean`
- `VUSTED_SLOW`
    - For example if you set 1000, add summary of the tests that elapsed 1000ms or more.
    - This can use only if the output handler is `vusted.default`.

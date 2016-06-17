crystal_lib_gen
===============

Automatic binding generator for Crystal

## Install (OSX)

```sh
brew install llvm --with-clang
brew link llvm --force
brew install crystal
brew install mruby

bundle install
```

## Install (Ubuntu)
```sh
sudo apt install llvm-3.5 libclang3.4-dev ruby2..-dev bundler
bundle install
```

## Usage
```sh
# Just an example
bin/crystal-lib-gen path/to/config.rb
# Use another dynamic library name (e.g. libclang-3.4)
# Use this if it can't find clang
FFI_GEN_CLANG=clang-3.4 bin/crystal-lib-gen path/to/config.rb
# Use compatibility mode (disable chdir to script directory, which is enabled by default)
CLG_COMPAT=1 bin/crystal-lib-gen path/to/config.rb
```

## See Also
* [Crystal](https://github.com/manastech/crystal)
* [ffi-gen](https://github.com/neelance/ffi-gen)

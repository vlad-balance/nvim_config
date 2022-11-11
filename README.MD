# install and configuration nvim for python and rust language.

```sh
arch -arm64 brew install nvim
```

Install LSP server pyright and rust-analyzer:
```sh
npm install -g pyright
brew install rust-analyzer
```

Create config:
```
mkdir -p ~/.config/nvim
nvim ~/.config/nvim/init.vim
```

Install plugin manager for vin/nvim (https://github.com/junegunn/vim-plug).

Сopy the contents of the file [~/.config/nvim/init.vim] to your config.

Done!


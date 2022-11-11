# install and configuration nvim for python and rust language.

```sh
arch -arm64 brew install nvim
```

Install LSP server pyright and rust-analyzer:
```sh
npm install -g pyright
arch -arm64 brew install rust-analyzer
```

Create config:
```
mkdir -p ~/.config/nvim
nvim ~/.config/nvim/init.vim
```

Install plugin manager for vin/nvim (https://github.com/junegunn/vim-plug).

Сopy the contents of the file [~/.config/nvim/init.vim] to your config.

Install config and plugin. In nvim write command:
```
:so %
:PlugInstall
:so %
```
**Pyright needs git repo and a config in your work directory to work.**

Init git repo:
```sh
git init
```

Create virtual enviroment:
```sh
python3 -m venv env
```

Activate venv:
```sh
. ./env/bin/activate
```

Create file pyrightconfig.json
```sh
nvim pytightconfig.json
```

Copy this is contents to your file [pyrightconfig.json]:
```json
{
  "venv": "env",
  "venvPath": "."
}
```

And rust-analyzer is already wirking!

Done!


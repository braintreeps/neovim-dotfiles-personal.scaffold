# Neovim personal configuration

The clean way to make our neovim-dotfiles yours. It's a reference scaffold for tweaking braintreeps/neovim-dotfiles.

Use taste, judgement, and don't spoil a pair's UX. Prefer to contribute additive improvements upstream.

Install [neovim-dotfiles](https://github.com/braintreeps/neovim-dotfiles) first. This scaffold adds personal options, keymaps, and plugins.

Install this repository at `nvim/lua/personal`. The destination must not already exist. Both commands use `$XDG_CONFIG_HOME`, falling back to `$HOME/.config` when it is unset.

Clone directly into the personal directory:

```sh
config_dir=${XDG_CONFIG_HOME:-$HOME/.config}
mkdir -p "$config_dir/nvim/lua"
git clone https://github.com/cosgroveb/neovim-dotfiles-personal.scaffold.git "$config_dir/nvim/lua/personal"
```

Or, from an existing checkout's root, symlink it into the personal directory:

```sh
config_dir=${XDG_CONFIG_HOME:-$HOME/.config}
mkdir -p "$config_dir/nvim/lua"
ln -s "$PWD" "$config_dir/nvim/lua/personal"
```

Then start Neovim with `nvim`. Use this repository as a template and substitute your repository URL if you want your own remote. For a nondefault configuration, use its `lua/personal` directory.

The examples in this repository are comments. Uncomment an example to use it.

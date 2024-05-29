# eza-preview.yazi

[Yazi](https://github.com/sxyazi/yazi) plugin to preview directories, can be switched between list and tree modes.

![list.png](https://raw.githubusercontent.com/sharklasers996/eza-preview.yazi/main/list.png)
![tree.png](https://raw.githubusercontent.com/sharklasers996/eza-preview.yazi/main/tree.png)

## Requirements

- [yazi](https://github.com/sxyazi/yazi)

## Installation

### Linux/MacOS

```sh
git clone https://github.com/sharklasers996/eza-preview.yazi ~/.config/yazi/plugins/eza-preview.yazi
```

## Usage

Add `eza-preview` to previewers in `yazi.toml`:

```toml
prepend_previewers = [
	{ name = "*/", run = "eza-preview" },
]
```

Set key binding to switch between list and tree modes in `keymap.toml`:

```toml
[manager]
keymap = [
	{ on = [ "E" ], run = "plugin eza-preview",  desc = "Toggle tree/list dir preview" },
]
```
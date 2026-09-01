# My tmux config

## Refresh config

```bash
tmux source-file ~/.config/tmux.conf
```

## Compare with upstream/master

```bash
nvim -d .tumx.conf.local tmux.conf.local
```

## Known issues

- Disabled extended-keys due to neovim pasting issue
  - <https://github.com/gpakosz/.tmux/issues/776>
  - As a result, any `Ctrl+Shift+letter` will be indistinguishable from and thus fall back to `Ctrl+letter` inside tmux

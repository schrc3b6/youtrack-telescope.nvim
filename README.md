# Youtrack Telescope Extension

Youtrack allows issue management via smart commits. For the smart commits you need to know the issue ID.
This extension lists all Youtrack Issues assigned you, shows a small description in the preview and returns the issue id on selection.

![](demo.gif)

## How To

1. Install this repository with your favorite plugin manager.
``` lua
use 'schrc3b6/youtrack_telescope.nvim'
```

2. Add youtrack to the telescope extensions 

`url` and `token` are mandetory parameters. The query parameter can be optionally adjusted.

```lua
extensions = {
    youtrack = {
        url = "youtrack.example.com",
        token = "perm:XXX",
		query = "for: me #Unresolved ",
    },
    ...
}
```

3. Add keybindings. The extension can be started via:
`Telescope youtrack youtrack`

To leave telescope in insert mode:
```lua
	require("telescope").extensions.youtrack.youtrack({ insert_mode = true })
```

## Status

This is my first time writing lua and my first vim plugin, so it's probably littered with bugs :)

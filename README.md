# Youtrack Telescope Extension

Youtrack allows issue management via smart commits. For the smart commits you need to know the issue ID.
This extension lists all Youtrack Issues assigned you, shows a small description in the preview and returns the issue id on selection.

## How To

add Youtrack to the telescope extensions 

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

## Status

This is my first time writing lua and my first vim plugin, so it's probably littered with bugs :)

## Open ToDos

[ ] Fix Pagination


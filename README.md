# yatline-tab-path.yazi

An addon to display the tab-path and file filter colorized 
in your [yatline.yazi](https://github.com/imsi32/yatline.yazi).

## Requirements

- [yazi](https://github.com/sxyazi/yazi) version >= 0.4.0
- [yatline.yazi](https://github.com/imsi32/yatline.yazi)

## Installation

```sh
ya pack -a blackdaemon/yatline-tab-path.yazi
```

## Usage

> [!IMPORTANT]
> Add this to your `~/.config/yazi/init.lua` after yatline.yazi's initialization.

With default settings:
```lua
require("yatline-tab-path"):setup()
```

Override the default settings:
```lua
require("yatline-tab-path"):setup({
        path_fg = "brightwhite", 
        filter_fg = "brightyellow", 
        search_label = "search", 
        filter_label = "filter", 
        flatten_label = "flatten", 
        no_filter_label = "no filter",
        separator = ", ",
})
```

Then, add it in one of your sections in the yatline configuration using:

```lua
{ type = "coloreds", custom = false, name = "yatline-tab-path" }
```

## Credits

- [Yazi](https://github.com/sxyazi/yazi)
- [yatline.yazi](https://github.com/imsi32/yatline.yazi)

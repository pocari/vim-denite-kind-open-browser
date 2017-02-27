# vim-denite-kind-open-browser

`vim-denite-kind-open-browser` is a `Kind` for [denite.nvim](https://github.com/Shougo/denite.nvim).

This plugin can open denite's candidate that has `url` as key by browser.

## depends

This plugin depends on:

* [denite.nvim](https://github.com/Shougo/denite.nvim)
* [open-browser.vim](https://github.com/tyru/open-browser)

## install

For [dein.vim](https://github.com/Shougo/dein.vim)

   ```
   call dein#add('Shougo/denite-nvim')
   call dein#add('tyru/open-browser.vim')
   call dein#add('pocari/vim-denite-kind-open-browser')
   ```

## Kind info

You can this `Kind` with your denite `Source` in this way.

```
class Source(Base):

    def __init__(self, vim):
        super().__init__(vim)
        # set 'open_browser' to self.kind
        self.kind = 'open_browser'
        # ... other codes
```

## Kind action

- open ... It open Selected candidate by `OpenBrowsser` plugin.


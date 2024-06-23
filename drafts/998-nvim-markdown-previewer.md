# How I set up and utilize a markdown previewer on neovim.

As I found myself writing more documentation and blog posts with [markdown](https://daringfireball.net/projects/markdown/), I quickly realized that it wasn't realistic to continuously cycle between editing, upating a pull request, and checking a GitHub preview environment.

I therefore set out to find a sort of previewer that would allow me to keep development closer to my IDE, and settled on [iamcco/markdown-preview.nvim](https://github.com/iamcco/markdown-preview.nvim).


## Installation

At the time of this post, I'm using [kickstart.nvim](https://github.com/nvim-lua/kickstart.nvim), and added the following material to my ~.config/nvim/init.lua file:

```lua
  {
    'iamcco/markdown-preview.nvim',
    cmd = { 'MarkdownPreviewToggle', 'MarkdownPreview', 'MarkdownPreviewStop' },
    build = 'cd app && yarn install',
    init = function()
      vim.g.mkdp_filetypes = { 'markdown' }
    end,
    ft = { 'markdown' },
  },
```
## Use

At the moment, I feel I'm using it in a basic way, i.e., only running `:MarkdownPreview` to open a preview window.

## How it works


## Concluding thoughts



from: https://www.google.com/search?q=lazy+nvim+clone+series+parallel

# Google Gemini:
>## Managing Series (Sequential) Installations
>While lazy.nvim handles most things in parallel, there are edge cases, such as on lower-powered devices (like a Raspberry Pi) or when dealing with complex plugins that conflict, where you might need to force a serial installation.
>- **Concurrency Settings**: You can control the number of parallel tasks by adjusting the concurrency setting in your lazy setup configuration. If you set concurrency = 1, all plugins will be installed sequentially (in series).
>- **Fixing "Clone Failed" Errors**: If you encounter clone failed errors, it is often due to too many parallel operations, which can be resolved by setting the concurrency option to a lower number or 1 in your lazy.lua file.

reference: https://github.com/LazyVim/LazyVim/discussions/4396

in: ~/.config/nvim/lua/config/lazy.lua
```
-- Example: Setting concurrency to 1 to force serial installation
require("lazy").setup(plugins, {
  concurrency = 1, -- Limit to 1 plugin at a time
})
```

# Doc:
https://lazy.folke.io/installation

# sch:
https://www.google.com/search?q=lazy+nvim+concurrency

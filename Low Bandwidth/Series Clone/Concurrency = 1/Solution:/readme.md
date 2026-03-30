from: https://www.google.com/search?q=lazy+nvim+clone+series+parallel

```
-- Example: Setting concurrency to 1 to force serial installation
require("lazy").setup(plugins, {
  concurrency = 1, -- Limit to 1 plugin at a time
})
```

https://github.com/LazyVim/LazyVim/discussions/4396

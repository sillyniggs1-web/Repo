# luac-decompiler

Decompiles LuaJIT bytecode (.luac) to Lua using
[luajit-decompiler-v2](https://github.com/marsinator358/luajit-decompiler-v2) via GitHub Actions.

## Usage
1. Put your `.luac` files in `luac/` (subfolders are fine).
2. Push to GitHub, or run the workflow manually: Actions > "Decompile luac to Lua" > Run workflow.
3. Get the results from `lua_out/` (committed back automatically) or from the `decompiled-lua` artifact.

## Notes
- Only LuaJIT bytecode is supported (not plain Lua 5.1-5.4 bytecode).
- Remove the last workflow step if you don't want results committed back.
- Check the "Show decompiler options" step log for the exe's available flags.

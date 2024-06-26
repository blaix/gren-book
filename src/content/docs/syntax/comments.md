---
title: Comments
description: Comments in Gren
---

Lines starting with `--` are ignored by the compiler, and are useful for describing something to human readers.

```elm
-- Nothing to see here
```

You can also use `{- -}` to have comments span multiple lines.

```elm
{- This comment
spans
multiple lines
-}
```

Comments can be used pretty much everywhere, as they're completely ignored by the compiler.

## Documentation comments

There are special kinds of comments, called documentation comments, which are recognized by the compiler as being documentation for a module or a value.

These comments are enclosed within `{-| -}` and will be used to render documentation on [packages.gren-lang.org](https://packages.gren-lang.org).

```elm
{-| This is an approximation of pi
-}
pi = 3.14
```

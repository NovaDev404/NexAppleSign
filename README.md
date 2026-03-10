# NexAppleSign (AltSign)

Swift package for NexStore - Fork of AltSign

## Dependencies

This package relies on git submodules, including the nested `libplist` submodule inside `Dependencies/ldid`.

After cloning, initialize dependencies with:

```sh
git submodule sync --recursive
git submodule update --init --recursive
```

If the `ldid-core` target fails with `'node.h' file not found`, verify that `Dependencies/ldid/libplist/libcnary/include/node.h` exists. That header comes from the nested `libplist` checkout used by `Dependencies/ldid/libplist/src/xplist.c`.

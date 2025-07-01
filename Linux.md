#linux
## .tar.gz
it’s a **compressed archive**, similar to a `.zip` file on Windows.

It’s actually two formats combined:

- **`.tar`** – short for “tape archive”  
    This bundles multiple files and folders into a single file.
- **`.gz`** – short for “gzip”  
    This compresses that `.tar` file to reduce size.

So `.tar.gz` = **archive (tar) + compression (gzip)**

### How to extract a compressed archive?

```zsh
tar -xzvf my-archive.tar.gz
```
- `x` = extract    
- `z` = it's gzip-compressed
- `v` = show progress
- `f` = filename follows
# Create Code Blocks

WIP to automatically create common code blocks, like *if*, *for* or simply closing certain brackets with indentation. I would like to replace [autoclose](https://github.com/Townk/vim-autoclose) since I tend not to make good use of it, but I would like a similar plugin that fits into my workflow better.

I will attempt to keep the _**WIP**_ marks up to date on all sections, but this is supposed to be [Readme Driven Development](https://tom.preston-werner.com/2010/08/23/readme-driven-development.html), so what you read in this file details what I intend, not necessarily what I have implemented.

Latest progress on branch [development](https://github.com/SonkeWohler/CreateCodeBlocks/development), latest stable (hopefully) version on [master](https://github.com/SonkeWohler/CreateCodeBlocks/master).

## _**WIP**_ Functionality

Where `_` is the cursor location.

By default `codeCompleteLeader` is set to your `<Leader>`, which vim sets to `\` by default. I'll use that for any demonstrations.

### Autoclose {}

In insert mode:

```
{_
```

Creates: 

```
{
  _
}
```

If you only want to write `{` without closing it use `\{` instead.

### _**WIP**_ Generate Simple Code Blocks

Use:

```
\if
```

To create:

```
if (_) {

}
```

### _**WIP**_ Customisation

You can redefine `codeCompleteLeader` to any key you like, including <F24>. This last part is useful if you want other shortcuts, like `i_<C-i>` to be mapped to do what `\if` would otherwise.

You can also simplly call the functions.

## FAQ

**Why not use IDE-like plugins for vim?**  
To learn stuff, and because I don't want to add plugins for any language prematurely. For example, I like coding small perl files, but I doubt I would use all that functionality for small files. Any functionality I don't need I will probably not understand and may interfere with the functionality I actually use.

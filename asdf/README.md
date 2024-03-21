# ASDF

This is a cli fastantic tool. We can manage several languages or software version through only one tool. There is a common core and we can add several plugin to work with differents software or languages programming.
The official web is the next [asdf](https://asdf-vm.com/).

This notes is a little summary of the most common functionality of the tool. I will help in the future when I will not remember something. Here We will be able to find the basic information to use the tool.

Each language or tool need a plugin to manage its, the follow command list the plugins that I have installed.

```zsh
    asdf plugin list
```

There is a list with every plugins in the [index](https://github.com/asdf-vm/asdf-plugins). We can show all plugin of index

```zsh
    asdf plugins list all
```

When We have installed some plugin we can manage this tool, in other hand we need install a version of this tool. For instance we are going to work with nodejs.

```zsh
    asdf plugin add <name>
    asdf plugin update <name>
    asdf plugin remove <name>
    asdf plugin update --all
    asdf plugin add nodejs
```

Above we can find some helpful command of plugins. But we need install a version of tool, choose the version and list the posibilities versions of tools.

```zsh
    asdf shim-versions node
    asdf list-add nodejs
    asdf install nodejs <version>
```

Finally we need to set the version for this moment, there is several context, local, shell and global.
```zsh
    asdf global nodejs latest
```

The most interesing website of this tool is [A guide of asdf command](https://vergaracarmona.es/guia-del-comando-asdf/).

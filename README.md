# About

Shortcuts for Kickstart extension development. In the past, `cd`-ing into all these different directories becomes painful.
This shell tool automatically detects the location of your themes and components, allowing you to run commands in their submodules or `cd` into them.

# Not yet available

I hope to complete this at some point, but for now it exists as a documentation prototype.

# Shortcuts

## Run a command in an extension directory

    kst <t [theme]|c [component]> <extension name> <shell command>
    
Example:

    kst t mytheme git commit -am "Updating colors"
    kst c mycomponent git commit -am "Fixing JS bug."
    
These are equivalent to:

    cd ./lib/sass/themes/mythemes/ && git commit -am "Updating colors"
    cd ./lib/sass/vendor/mycomponent && git commit -am "Fixing JS bug."

You can also cd into the extension like this

    kst cd t mytheme
    git commit -am "Updating colors"

    kst cd c mycomponent
    git commit -am "Fixing JS bug."

## Return home

Where home is the root of the project, not your machine's home `~` directory.

    kst cd ~

# Shortcuts

## Run a command in an extension directory

    kickstart <t [theme]|c [component]> <extension name> <shell command>

    kickstart t mytheme git commit -am "Updating colors"
    kickstart c mycomponent git commit -am "Fixing JS bug."

You can also cd into the extension like this

    kickstart cd t mytheme
    git commit -am "Updating colors"

    kickstart cd c mycomponent
    git commit -am "Fixing JS bug."

## Return home

Where home is the root of the project, not your machine's home `~` directory.

    kickstart cd ~

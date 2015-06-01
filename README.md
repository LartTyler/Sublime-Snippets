# About Sublime Snippets
`Sublime Snippets` is a collection of useful snippets for Sublime Text 2+. It includes various snippets that I've put
together over time, ranging from library specific snippets (such as Doctrine or Symfony) to general, time-saving snippets
for code I write every day.

# Installation
First, navigate to your Sublime user packages directory. The default path for each system is below, but may be slightly
different depending on which version of Sublime you are using.

**Windows**:
>  C:\Users\\{user}\AppData\Roaming\Sublime Text 2\Packages\User

**OSX**:
> /Users/{user}/Library/Application Support/Sublime Text 2/Packages/User

**Linux**:
> ~/.config/sublime-text-2/Packages/User

Then, execute the follwing command (requires the `git` command [duh...]).

```
git clone https://github.com/LartTyler/Sublime-Snippets.git Sublime-Snippets
```

The final argument ("Sublime-Snippets") will be the name of the directory that the snippets are stored in. It can be
anything you like, but I recommend naming it something that will allow you to distinguish it from any other packages
in the folder.

After that, you're good to go. Sublime will automatically find the new snippets and let you immediately begin using them.

**Important note for HTML snippets*: I recommend adding the following line to your Sublime user preferences.

```
"auto_complete_selector": "sources, text.html, text.html.twig"
```

Otherwise, you'll have to type out the entire snippet trigger for snippets within HTML and Twig scopes.

# Usage
The naming scheme for each snippet denotes how and when they can be triggered. The format is
`<scope>.<namespace>.<tab-trigger>.sublime-snippet`.

In most cases, the trigger text for a snippet is <namespace> concatenated with <tab-trigger>. So, for example, you can
trigger the snippet for creating a Doctrine query builder any time you're in the PHP scope using `doctrineqbcreate` (or
any shorthand variation thereof, such as `dqbc`).

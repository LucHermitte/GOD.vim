# GOD.vim

Get online doc link directly from vim

---

This plugin helps you to help people!

You are writting something about Vim on a site which handles markdown language *(like [vi.se](https://vi.stackexchange.com) or [/r/vim](https://reddit.com/r/vim) or even a github Readme file like this one)*, you want to direct your readers to a page of Vim doc?

Simply use the command `:GOD {help-topic}` to get in your clipboard a markdown string allowing you to link to the http://vimhelp.appspot.com/ online help.


# Example

The command:

    :GOD holy-grail
    
Will put in your clipboard the following string:


    [`:h holy-grail`](http://vimhelp.appspot.com/index.txt.html#holy%2dgrail)
    
Which will appears like this for your users:

[`:h holy-grail`](http://vimhelp.appspot.com/index.txt.html#holy%2dgrail)


# Configuration

GOD.vim provides two variables that you can defined in your `vimrc`:

## Disable the plugin

To disable the plugin you can put the following line in your `vimrc`:

    let g:loaded_god_vim = 1

## Automatically close the help buffer

When you use the `:GOD` command, the corresponding help buffer will be open. If you don't want to see it you can add the following line to your `vimrc`:

    let g:god_close_help_buffer = 1
    
# GOD.vim? What's this name?

It actually stands for **G**et **O**nline **D**oc *:)*

# Thanks

I'd like to thanks [Carpetsmoker](https://arp242.net/) who helped me improve the encoding of the generated urls.

This plugin was inspired by this question on the site vi.stackexchange.com: [How can I quickly convert a Vim help tag to a vimhelp.appspot.com link?](http://vi.stackexchange.com/q/4346/1841)

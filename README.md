# Voxed Color Scheme

# [Installation](#install)
# [FAQ](#faq)

## Voxed is a Color scheme for the [Helix Editor](https://helix-editor.com/)

I was bored one day so I decided to make my own color scheme

I don't consider this complete as I didn't configure all the for Helix


# Screenshots

## Python (Random python code I wrote)
![Alt text](./python-screenshot.png?raw=true "Python Code")

## C (Screenshot of [raudio.c](https://github.com/raysan5/raylib/blob/master/src/raudio.c) from the raylib source code)
![Alt text](./c-screenshot.png?raw=true "C Code")

## Rust (Screenshot of the [syn crate](https://github.com/dtolnay/syn/blob/master/src/buffer.rs) source code) 
![Alt text](./rust-screenshot.png?raw=true "Rust Code")

# Install
A pull request has been made to [Helix](https://github.com/helix-editor/helix/pull/9164)
to the master branch after it is reviewed and accepted you should be able to have the theme If
you build from master

But until that happens you can download voxed.toml and put it in ~/.config/helix/themes/
if you do not have the themes directory create it

It should look like this 
~/.config/helix/themes/voxed.toml

After that you can enable the theme at runtime doing

**:theme voxed**

or if you want to set the theme in your configuration file:

Inside of config.toml in ~/.config/helix/

**theme = "voxed"**


# FAQ

## The theme background is transparent how do I turn that off?
The theme is transparent so that way I have terminal blur
If you want to turn it off you can modify voxed.toml 

and go to the line **51** or search for **"ui.background"**

and change:

**"ui.background" = { fg = "#25262B", bg = "" }**

to:

**"ui.background" = { bg = "#25262B" }**

and that should fix it, if it does not or you have problems feel free to open up an issue

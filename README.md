# karabiner

MacOS Karabiner-Elements config dir. PC keys like Linux or Windows, a personal extension. US keyboard.

You can do it too! That's the motivational purpose of this repo. Of course, the most recent version will always
reflect a very personal use case. But you can have a look at the first commits in history, to see that everything
is based on https://ke-complex-modifications.pqrs.org/#pc_shortcuts - the commit messages should be comprehensible
and show when and what is introduced.

## Requirements

MacOS, https://karabiner-elements.pqrs.org/ installed and running.

Ideally no keyboard modifications outside of karabiner, so no settings adaptions in MacOS. (Yes, no
Command-Option-swapping or whatsoever. Better to be handled at one place - karabiner, even for multiple physical
keyboards.)

## Usage 

For example: Clone this repo somewhere, rename your karabiner config dir (typically ~/.config/karabiner) and replace
it by a link to the repo.

## Personal extensions

Have no fear modifying the karabiner.json directly. With copy and paste this is the most convenient and cleanest way.
Additional imports might be ok, but perhaps only if functionally disjoint.

### Looking at the json - I need to list and handle every application under the sun explicitly?

No, mostly it says `frontmost_application_unless` instead of `frontmost_application_if`, so someone already just
collected exotic cornercases for you.

## Features

Overall objective: You are working on Linux/Windows on a regular basis and you don't want to notice any difference
whenever using MacOS. So, under MacOS, whenever you hit a key on either a Mac or PC keyboard you should get the exact
same experience as under a Linux/Windows PC.

* US keyboard layout only (at least on the main branch of this repo; for German, a recommendation would be to import
https://ke-complex-modifications.pqrs.org/#german_iso_pc_mapping)
* 'control' key order from left to right: ctrl, win/command, alt/option - regardless of what label is being shown on
your keyboard - this holds true for your Mac native notebook keyboard as well as an external PC keyboard (different
keyboards should be identifiable in this repo's configuration)
* working with Visual Studio keymap (the Mac version!; perhaps little exceptions that would need to be
changed/disabled on that side)
* Terminal just like Linux
* shortcuts to open Terminal, lock screen, search, just like Linux
* home/end keys as familiar, also with ctrl and shift, also in Terminal
* close apps/windows/tabs, add tabs, just like Linux
* working for textedit, vscode, jetbrains

Note, whenever I said Linux, perhaps I meant Ubuntu.

## Q&A on general karabiner config

| Question                                  | Answer                                                        |
|-------------------------------------------|---------------------------------------------------------------|
| Which key(s) did I presss?                | Use the Karabiner EventViewer app, tab Main .                 |
| How is that frontmost application called? | Use the Karabiner EventViewer app, tab Frontmost Application. |
| What about that assets folder?            | Showing up when trying to add rules over karabiner GUI.       |

## todos

(Sorted by prio from high to low.)


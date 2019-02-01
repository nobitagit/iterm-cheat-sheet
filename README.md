# iTerm Cheat Sheet

## How to install

```sh
brew update
brew tap caskroom/cask  
brew cask info iterm2
brew cleanup
```
## Commands
### Tabs and Windows

**Function** | **Shortcut**
-------- | --------
Previous Tab | `⌘`+ `Left Arrow`
Next Tab | `⌘`+ `Right Arrow`
Go to Tab | `⌘` + `Number`
Go to Window | `⌘` + `Option` + `Number`
Go to Split Pane by Direction | `⌘` + `Option` + `Arrow`
Go to Split Pane by Order of Use | `⌘` + `]` , `⌘` + `[`
Split Window Horizontally (same profile) | `⌘` + `D`
Split Window Vertically (same profile) | `⌘` + `d`
Split Window Horizontally (new profile) | `Option` + `⌘` + `H`
Split Window Vertically (new profile) | `Option` + `⌘` + `V`
Resize current splitted pane | `Ctrl` + `⌘` + `Arrow`
Set Mark | `⌘` + `M`
Jump to Mark | `⌘` + `J`

### Basic Moves

**Function** | **Shortcut**
-------- | --------
Move back one character | `Ctrl` + `b`
Move forward one character | `Ctrl` + `f`
Delete current character | `Ctrl` + `d`
Delete previous character | `Backspace`
Undo | `Ctrl` + `-`

### Moving Faster

**Function** | **Shortcut**
-------- | --------
Move to the start of line | `Ctrl` + `a`
Move to the end of line | `Ctrl` + `e`
Move forward a word | `Option` + `f`
Move backward a word | `Option` + `b`
Clear the screen | `⌘` + `k`

### Cut and Paste

**Function** | **Shortcut**
-------- | --------
Cut from cursor to the end of line | `Ctrl` + `k`
Cut from cursor to the end of word | `Option` + `d`
Cut from cursor to the start of word | `Option` + `Backspace`
Cut from cursor to previous whitespace | `Ctrl` + `w`
Paste the last cut text | `Ctrl` + `w`
Loop through and paste previously cut text | `Option` + `y`
Loop through and paste the last argument of previous commands | `Option` + `.`

### Search the Command History

**Function** | **Shortcut**
-------- | --------
Search as you type | `Ctrl` + `r` and type the search term; Repeat `Ctrl` + `r` to loop through result
Search the last remembered search term | `Ctrl` + `r` twice
End the search at current history entry  | `Ctrl` + `y`
Cancel the search and restore original line | `Ctrl` + `g`


## Bonus tricks

### Name the current tab [[>]](https://superuser.com/a/599156/325858)

![Title bash snippet](https://raw.githubusercontent.com/nobitagit/iterm-cheat-sheet/master/title-fn.gif)

```sh
# Add this to your .bash_profile and then:
# $ title tabName
function title {
    echo -ne "\033]0;"$*"\007"
}
```

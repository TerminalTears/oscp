<img src ="../../media/vimlogo.png" width="250">

<img src ="https://github.com/nvrmoar/oscp/blob/media/vimlogo.png?raw=true" width="150">
# Vim Cheatsheet

The best way to learn Vim, in my opinion, is to do Vimtutor. You can enter vimtutor on many distros of using the 'vimtutor' command, but you may have to 'apt install' it. This is a collection of the commands you will learn in Vimtutor.

## Vim Cheatsheet

### Modes

```text
    i - Insert at the cursor
    a - Insert after the cursor

    I - Insert at beginning of line
    A - Insert at end of line

    o - Insert below the current line
    O - Insert above the current line

    jj - Escape to Normal Mode (Custom)

    R - Replace mode (Like insert, but overwrites instead of inserting)

    v - Visual mode
```

### Motion

```text
    h - Left
    l - Right
    j - Down
    k - Up

    e - Move to end of a word
    b - Move to beginning of a word

    gg - Move to first line of file
    G - Move to end of file.
    number+G - Move to line number

    CTRL+O - Move back to older positions
    CTRL+I - Move to newer positions
```

### Deletion

```text
    x - Delete character

    dw - Delete word forward
    db - Delete word backwards

    d$ - Delete from cursor to end of line
    d0 - Delete from cursor to beginning of line

    dd - Delete current line
```

### Undo

```text
    u - Under previous action
    U - Under all the changes on a line
    Ctrl+R - Undu the undo
```

### Quick Edits \| Change Operator

```text
    p - Paste a previously deleted stuff
    r - Replace character under cursor
    ce - Replace from cursor to end of word
    c$ - Replace from cursor to end of line
    c0 - Replace from cursor to beginning of line

    R - En
```

### Sed functionlity

```text
    :s/old/new - Substitute first occurrence of 'old' with 'new'
    :s/old/new/g - Substitute 'new' for all 'old's on a line
    :#,#s/old/new/g - Substitute all occurrences of 'old' between the two line #s with 'new'
    :%s/old/new/g - Substitute all occurrences of 'old' with 'new' in the entire file. (Use gc to ask for confirmation)
```

### Searching a file

```text
    / - Search forward
    ? - Search backward

    /Search\c - Adding \c ignores case

    n - Next search result
    N - Previous search result
```

### Commands

```text
    :!command - Execute external command
    :w FILENAME - Writes the current file to disk as FILENAME
    v+motion :w FILENAME - Saves the visually selected lines in file FILENAME
    :r FILENAME - Retrieves file FILENAME and puts it below the cursor position
    :r !command - Reads the output of a command and puts it below the cursor position
```

### Yanking

```text
    y - Copies visually highlighted text
    p - Pastes text
```


## `git stripspace`

_[`git stripspace` documentation on git-scm.com](https://git-scm.com/docs/git-stripspace)_

"Remove unnecessary whitespace". This can also be used with a few flags to remove all comments. 

With no arguments, this will:

- remove trailing whitespace from all lines
- collapse multiple consecutive empty lines into one empty line
- remove empty lines from the beginning and end of the input
- add a missing \n to the last line if necessary.

In the case where the input consists entirely of whitespace characters, no output will be produced.

#### Examples 

Given the following noisy input with $ indicating the end of a line:

```
|A brief introduction   $
|   $
|$
|A new paragraph$
|# with a commented-out line    $
|explaining lots of stuff.$
|$
|# An old paragraph, also commented-out. $
|      $
|The end.$
|  $
```

Use git stripspace with no arguments to obtain:

```
|A brief introduction$
|$
|A new paragraph$
|# with a commented-out line$
|explaining lots of stuff.$
|$
|# An old paragraph, also commented-out.$
|$
|The end.$
```

Use git stripspace --strip-comments to obtain:

```
|A brief introduction$
|$
|A new paragraph$
|explaining lots of stuff.$
|$
|The end.$
```

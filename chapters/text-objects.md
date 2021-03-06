## Basic Usage

Text objects are Vim's representation of groups of text.

These are some of the text objects you'll use the most:

`w` represents a word

`s` represents a sentence

`p` represents a paragraph

You specify how you want an action to be applied with `a` or `i`:

`a` means all, and the action will be applied to the text object and succeeding white space

`i` means in, and the action will be applied only to the text

You can use text objects with the following pattern:

`<action><specifier><text object>`

Examples:

`dap` will delete an entire paragraph

`ciw` will change a word

## String-based Text objects

You can also use delimiters to specify text objects.

Available delimiters:

`"`

`'`

`)` or `(`

`]` or `[`

`}` or `{`

Examples:

`ci"` Change inside closest double quote

`ci'` Change inside closest single quote

`ci)` Change inside closest parentheses

`ci]` Change inside closest brackets

`ci}` Change inside closest braces

Note that if you do `ca)` instead of `ci)` then the parentheses will be
deleted.

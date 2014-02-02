# find-on-github

Functions in Emacs Lisp to determine a URL for a file & commit in a
GitHub.com repository and open it in a web browser.

This library was inspired by
[gleitz/browse-on-github.el](https://github.com/gleitz/browse-on-github.el)
but rewritten from scratch without an external script.


## Installation

Place the file `find-on-github.el` on your Emacs `load-path` and add
the following to your Emacs initialization file:

    (require 'find-on-github)



## Usage

While in a buffer viewing a file in a Git repository, call one of the
following:

    M-x browse-on-github

        Opens the current file, at the current commit, in the default
        web browser on GitHub.com.

    M-x find-on-github

        Displays a GitHub.com url for the current file, at the current
        commit, and copy it to the kill ring.

Both functions will create URLs that include the current line number
highlighted. If the region is active, they will show the lines in the
region highlighted. If point is at the beginning of the file, no lines
are highlighted.



## Copyright and License

The MIT License (MIT)

Copyright © 2013 Stuart Sierra

Permission is hereby granted, free of charge, to any person obtaining a copy of
this software and associated documentation files (the "Software"), to deal in
the Software without restriction, including without limitation the rights to
use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
the Software, and to permit persons to whom the Software is furnished to do so,
subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

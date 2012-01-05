# rcirc ucomplete

Unambiguous completion for rcirc.

If you don't like the cycling completion that is the default in rcirc,
try this instead.

## Installation

Install from [Marmalade](http://marmalade-repo.org) using package.el
if you have Emacs 24 or newer. If you aren't set up to install from
Marmalade, try this:

```lisp
(require 'package)
(add-to-list 'package-archives
             '("marmalade" . "http://marmalade-repo.org/packages/"))
(package-initialize)
```

Eval the above code, run `M-x package-refresh-contents`, and then do
`M-x package-install rcirc-ucomplete` to install.

Alternatively to do a manual install, place `rcirc-ucomplete.el` on
the classpath and add this to your Emacs config:

```lisp
(autoload rcirc-ucomplete "rcirc-ucomplete" "" t)
(eval-after-load 'rcirc
  '(define-key rcirc-mode-map (kbd "TAB") 'rcirc-ucomplete))
```

## License

Copyright © 2007, 2011 Phil Hagelberg

This program is free software; you can redistribute it and/or
modify it under the terms of the GNU General Public License as
published by the Free Software Foundation; either version 3 of
the License, or (at your option) any later version.

This program is distributed in the hope that it will be
useful, but WITHOUT ANY WARRANTY; without even the implied
warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR
PURPOSE.  See the GNU General Public License for more details.

You should have received a copy of the GNU General Public
License along with this program; if not, write to the Free
Software Foundation, Inc., 59 Temple Place, Suite 330, Boston,
MA 02111-1307 USA

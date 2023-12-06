[![Melpa Status](http://melpa.org/packages/edit-indirect-badge.svg)](http://melpa.org/#/edit-indirect)
[![Melpa Stable Status](http://stable.melpa.org/packages/edit-indirect-badge.svg)](http://stable.melpa.org/#/edit-indirect)

# edit-indirect

Edit regions in separate buffers, like `org-edit-src-code` but for arbitrary regions.

## Installation

The package is available in [MELPA](http://melpa.org/).

If you have MELPA in `package-archives`, use

    M-x package-install RET edit-indirect RET

If you don't, open `edit-indirect.el` in Emacs and call
`package-install-from-buffer`.

## Usage

To start editing, run:

    M-x edit-indirect-region

### Indirect buffer shortcuts

- `C-c '` or `C-c C-c` to commit the changes

- `C-c C-k` to abort


## Customization

- `edit-indirect-guess-mode-function`

the default value is `#'edit-indirect-default-guess-mode` (defaulting to `normal-mode`).

There is also a [third party addon](https://github.com/a13/language-detection-utils) that provides automatic language mode guessing powered by [language-detection](https://github.com/andreasjansson/language-detection.el).

## Hooks

- `edit-indirect-after-creation-hook`

- `edit-indirect-before-commit-hook`

- `edit-indirect-before-commit-functions`

- `edit-indirect-after-commit-functions`

# maid.el

Rule-based file management for Emacs.

## What is maid?

Maid helps you automatically organize and clean up your files using simple rules written in Emacs Lisp.

## Status

🚧 **Under Active Development** - Core functionality coming soon.

## Planned Features

- Define file organization rules in Emacs Lisp
- Dry-run mode to preview actions
- Move, copy, delete files based on age, size, or type
- Scheduled and manual cleaning

## Quick Example

```elisp
;; Future syntax (not yet implemented)
(maid-defrule "clean-downloads"
  :files (maid-dir "~/Downloads/*")
  :when (maid-older-than 7 'days)
  :action (lambda (file) (maid-trash file)))
```

## Installation

Not yet available. Watch this repo for updates.

## Roadmap

- [ ] Core rule engine
- [ ] File operation DSL
- [ ] Dry-run mode
- [ ] Interactive execution
- [ ] Directory watching

## Inspiration

Inspired by the Ruby [maid](https://github.com/benjaminoakes/maid) gem.

## License

GPL-3.0

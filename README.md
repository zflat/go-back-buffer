# go-back-buffer

## Introduction

go-back-buffer is a package that provides a minor mode and interactive function for easily switching to the most recently visited buffer in the active window. Think of it like Alt+Tab for buffers in emacs windows.

## Installation and Setup:

Install go-back-buffer from MELPA, or download it manually from GitHub. If you download manually, add these lines to your init file:

```
(add-to-list 'load-path "/path/to/go-back-buffer")
(require 'go-back-buffer)
```

To activate Purpose at start-up, add this line to your init file:

```
(go-back-buffer-mode)
```

Recommended key binding: bind a function key to 'gbb-display-prev-buffer

```
(global-set-key (kbd "<f1>") 'gbb--display-prev-buffer)
```

## Basic Usage:

1. Switch to the most recently viewed buffer in the given window
   ```
   (gbb--display-prev-buffer)
   ```

## Contributing

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request

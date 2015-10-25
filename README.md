
#### Iodine emacs color theme
  
![Screenshot](https://github.com/srdja/iodine-theme/blob/master/theme.png)

#### Installing the theme

##### Through [Melpa](https://melpa.org) (recomended)
Make sure you have the following lines in you `.emacs` file if you don't already have them:
```elisp
(require 'package) ;; You might already have this line
(add-to-list 'package-archives
             '("melpa" . "https://melpa.org/packages/"))
(when (< emacs-major-version 24)
  ;; For important compatibility libraries like cl-lib
  (add-to-list 'package-archives '("gnu" . "http://elpa.gnu.org/packages/")))
(package-initialize) ;; You might already have this line
```
You can now run `M-x package-install` `iodine-theme`

##### By cloning the repo  
Clone the repo and then add this line to your `.emacs` file:
```elisp
(add-to-list 'custom-theme-load-path "/path/to/theme-file.el")
```
This will make sure that emacs can find the theme file.

#### Using the theme
The theme can be loaded with `M-x load-theme` `iodine`

Or if you wish to load the theme on startup you can add this to your `.emacs`:
```elisp
(load-theme 'iodine t)
```

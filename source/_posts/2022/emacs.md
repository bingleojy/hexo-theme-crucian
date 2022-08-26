---
title: Emacs编辑器
author: Binglin Li
toc: true
tags:
  - Emacs
category:
  - Emacs
categories:
  - '2022'
date: 2022-06-30 19:54:45
---

#### Emacs是一个可扩展,可定制,可实时自动化显示编辑器

连续按ctrl x m（显示为C-x m）可以打开Emacs帮助文件
选项前的 -- 也可以简化为 - 是一样的效果 

### Emacs用法

	$ emacs.exe [--选项 文件名]...

### --batch
功能：不做交互式显示，隐含-q选项

	$ emacs --batch

### --chdir
功能：改变启动目路

	$ cd $HOME
	$ emacs --chdir demos```

### --daemon, --bg-daemon[=NAME]
功能：打开一个以NAME命名的隐藏守护进程（我经常使用此选项）

	$ emacs --daemon


### --fg-daemon[=NAME]
功能：打开一个以NAME命名的显示守护进程

	$ emacs --fg-daemon

### --debug-init
打开Emacs lisp调试

	$ emacs --debug-init


### --display, -d DISPLAY
功能：use X server DISPLAY

	$ emacs --display

	--module-assertions         assert behavior of dynamic modules

	--dump-file FILE            read dumped state from FILE

	--no-build-details          do not add build details such as time stamps

	--no-desktop                do not load a saved desktop

	--no-init-file, -q          load neither ~/.emacs nor default.el

	--no-loadup, -nl            do not load loadup.el into bare Emacs

	--no-site-file              do not load site-start.el

	--no-x-resources            do not load X resources

	--no-site-lisp, -nsl        do not add site-lisp directories to load-path

	--no-splash                 do not display a splash screen on startup

	--no-window-system, -nw     do not communicate with X, ignoring $DISPLAY

	--quick, -Q                 equivalent to:
                              -q --no-site-file --no-site-lisp --no-splash
                              --no-x-resources

	--script FILE               run FILE as an Emacs Lisp script

	--terminal, -t DEVICE       use DEVICE for terminal I/O

	--user, -u USER             load ~USER/.emacs instead of your own

Action options:

	FILE                    visit FILE
	+LINE                   go to line LINE in next FILE
	+LINE:COLUMN            go to line LINE, column COLUMN, in next FILE
	--directory, -L DIR     prepend DIR to load-path (with :DIR, append DIR)
	--eval EXPR             evaluate Emacs Lisp expression EXPR
	--execute EXPR          evaluate Emacs Lisp expression EXPR
	--file FILE             visit FILE
	--find-file FILE        visit FILE
	--funcall, -f FUNC      call Emacs Lisp function FUNC with no arguments
	--insert FILE           insert contents of FILE into current buffer
	--kill                  exit without asking for confirmation
	--load, -l FILE         load Emacs Lisp FILE using the load function
	--visit FILE            visit FILE

Display options:

	--background-color, -bg COLOR   window background color
	--basic-display, -D             disable many display features;
                                  used for debugging Emacs
	--border-color, -bd COLOR       main border color
	--border-width, -bw WIDTH       width of main border
	--color, --color=MODE           override color mode for character terminals;
                                  MODE defaults to `auto', and
                                  can also be `never', `always',
                                  or a mode name like `ansi8'
	--cursor-color, -cr COLOR       color of the Emacs cursor indicating point
	--font, -fn FONT                default font; must be fixed-width
	--foreground-color, -fg COLOR   window foreground color
	--fullheight, -fh               make the first frame high as the screen
	--fullscreen, -fs               make the first frame fullscreen
	--fullwidth, -fw                make the first frame wide as the screen
	--maximized, -mm                make the first frame maximized
	--geometry, -g GEOMETRY         window geometry
	--no-bitmap-icon, -nbi          do not use picture of gnu for Emacs icon
	--iconic                        start Emacs in iconified state
	--internal-border, -ib WIDTH    width between text and main border
	--line-spacing, -lsp PIXELS     additional space to put between lines
	--mouse-color, -ms COLOR        mouse cursor color in Emacs window
	--name NAME                     title for initial Emacs frame
	--no-blinking-cursor, -nbc      disable blinking cursor
	--reverse-video, -r, -rv        switch foreground and background
	--title, -T TITLE               title for initial Emacs frame
	--vertical-scroll-bars, -vb     enable vertical scroll bars
	--xrm XRESOURCES                set additional X resources
	--parent-id XID                 set parent window
	--help                          display this help and exit
	--version                       output version information and exit

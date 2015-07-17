# sublime-install

# First install package:
  - Just follow the instructions needed https://packagecontrol.io/installation
  
# Install the needed tools for development.
  To install a specific package, enter: `ctrl + shift + p`.

List of tools:  
  
## Emmet
  - Emmet is a plugin for many popular text editors which greatly improves HTML & CSS workflow
  - More on emmet: http://www.smashingmagazine.com/2013/03/26/goodbye-zen-coding-hello-emmet/
  
## Bracket Highlighter
  - Bracket Highlighter matches a variety of brackets such as: `[], (), {}, "", '', #!xml <tag></tag>, and even custom brackets`.
  - Customizable to highlight almost any bracket.
  - View documentation here: https://github.com/facelessuser/BracketHighlighter

## Git Gutter
  - A sublime text 2/3 plugin to show an icon in the gutter area indicating whether a line has been inserted, modified or deleted.

## Git
  - A sublime text plugin to show git features.


# Add this to sublime text preferences

- Click `preferences` then `Settings - User`
- Add these lines of code to file and then save
```
{
	"default_line_ending": "unix",
	"detect_indentation": false,
	"draw_white_space": "all",
	"ensure_newline_at_eof_on_save": false,
	"file_exclude_patterns":
	[
		".DS_Store",
		"Desktop.ini",
		"*.pyc",
		"._*",
		"Thumbs.db",
		".Spotlight-V100",
		".Trashes"
	],
	"folder_exclude_patterns":
	[
		".git",
		"node_modules"
	],
	"font_size": 12.0,
	"highlight_modified_tabs": true,
	"hot_exit": false,
	"ignored_packages":
	[
		"Vintage"
	],
	"line_padding_bottom": 6,
	"match_brackets": true,
	"match_brackets_angle": true,
	"remember_open_files": false,
	"rulers":
	[
		80
	],
	"save_on_focus_lost": true,
	"spell_check": true,
	"tab_size": 4,
	"translate_tabs_to_spaces": false,
	"trim_trailing_white_space_on_save": true,
	"va_alignment_chars":
	[
		{
			"alignment": "right",
			"char": "=",
			"left_space": true,
			"prefixes":
			[
				"+",
				"-",
				"&",
				"|",
				"<",
				">",
				"!",
				"~",
				"%",
				"/",
				"*",
				"."
			],
			"right_space": true
		},
		{
			"alignment": "right",
			"char": ":",
			"left_space": true,
			"prefixes":
			[
			],
			"right_space": true
		}
	],
	"word_wrap": true
}
```

# Sublime Packages and Config
This is used as a guide for sublime beginners on how to use sublime, what packages to install and many more. If you have any more suggestions or something to add with the current documentaion i'm open to pull-requests.

**Note:** some of the packages I got from this website http://www.hongkiat.com/blog/sublime-text-plugins/

# First install package:
   Just follow the instructions needed https://packagecontrol.io/installation
  
# Install the needed tools for development.
  To install a specific package, enter: `ctrl + shift + p` for **linux** and **windows**. `cmd + shift + p` for **mac**.

List of tools:  
  
### Emmet
  - In a nutshell, **Emmet** allows us to write HTML and CSS faster with abbreviations/shortcuts, then expand them in valid HTML tags.
  - More on emmet: http://www.smashingmagazine.com/2013/03/26/goodbye-zen-coding-hello-emmet/

### SideBar Enhancements
 - **SidebarEnhancements** has a few new things in the Sidebar menu including New File Creation in the current project folder, Moving File and Folder, Duplicating File and Folder, Open in Finder and Browser, Refresh, and a bunch more.
  
### Bracket Highlighter
  - **Bracket Highlighter** matches a variety of brackets such as: `[], (), {}, "", '', #!xml <tag></tag>, and even custom brackets`.
  - Customizable to highlight almost any bracket.
  - View documentation here: https://github.com/facelessuser/BracketHighlighter


### Git Gutter
  - A sublime text 2/3 plugin to show an icon in the gutter area indicating whether a line has been inserted, modified or deleted.

### Git
  - A sublime text plugin to show git features.
  - This plugin integrates SublimeText with Git so you can run some Git commands from SublimeText such as Add and Committing Files, Viewing Log, and Annotating Files.

### Jshint
  - JSHint is a community-driven tool to detect errors and potential problems in JavaScript code. It is very flexible so you can easily adjust it to your particular coding guidelines and the environment you expect your code to execute in
  - https://github.com/jshint/jshint

### HTML-CSS-PRETTIFY
  - This is a Sublime Text 2 and 3 plugin allowing you to format your HTML, CSS, JavaScript and JSON code. It uses a set of nice beautifier scripts made by Einar Lielmanis. The formatters are written in JavaScript, so you'll need something (node.js) to interpret JavaScript code outside the browser.

### Terminal
  - This plugin lets you open your project folders in Terminal directly from SublimeText – with a hotkey. It is a very helpful plugin when you need to execute command lines at the given folder.
  
### CanIUse
  - With this plugin, you can check the browser support for CSS properties and HTML elements that you are using. To use it, highlight the CSS property or the HTML element, and it will bring you to the appropriate page in CanIUse.com.
 
### Trimmer
  - This plugin helps you remove unnecessary spaces, as well as trailing spaces, which could cause some errors In JavaScript.
  
### ColorPicker
  - With this plugin you can select and add colors to SublimeText with the native color wheel from your OS.
 
  
### DocBlockr
  - DocBlokr lets you create documentation or annotation for your codes with ease, by parsing the functions, parameters, variables, and automatically adding some possible documentation (see the screenshot below).


# Add this to sublime text preferences

- Click `preferences` then `Settings - User`
- Add these lines of code to file and then save
```
{
	"default_line_ending": "unix",
	"detect_indentation": false,
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
	"font_size": 10.0,
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
		90
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

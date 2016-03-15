# Sublime Packages and Config
This is used as a guide for sublime beginners on how to use sublime, what packages to install and many more. If you have any more suggestions or something to add with the current documentaion i'm open to pull-requests.

It's best to use **Sublime Text 3** for all of the packages I written here to work. [Download here](http://www.sublimetext.com/3)

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

- After installing, Click `preferences` then `Package - Settings` then `HTML/CSS/JS prettify`
- Add these lines of code to file and then save

```
{
  // The plugin looks for a .jsbeautifyrc file in the same directory as the
  // source file you're prettifying (or any directory above if it doesn't exist,
  // or in your home folder if everything else fails) and uses those options
  // along the default ones.

  // Details: https://github.com/victorporof/Sublime-HTMLPrettify#using-your-own-jsbeautifyrc-options
  // Documentation: https://github.com/einars/js-beautify/
  "html": {
    "allowed_file_extensions": ["htm", "html", "xhtml", "shtml", "xml", "svg"],
    "brace_style": "collapse", // [collapse|expand|end-expand|none] Put braces on the same line as control statements (default), or put braces on own line (Allman / ANSI style), or just put end braces on own line, or attempt to keep them where they are
    "end_with_newline": false, // End output with newline
    "indent_char": " ", // Indentation character
    "indent_handlebars": false, // e.g. {{#foo}}, {{/foo}}
    "indent_inner_html": false, // Indent <head> and <body> sections
    "indent_scripts": "keep", // [keep|separate|normal]
    "indent_size": 4, // Indentation size
    "indent_with_tabs": true, // Indent with tabs, overrides `indent_size` and `indent_char`
    "max_preserve_newlines": 0, // Maximum number of line breaks to be preserved in one chunk (0 disables)
    "preserve_newlines": true, // Whether existing line breaks before elements should be preserved (only works before elements, not inside tags or for text)
    "unformatted": ["a", "span", "img", "code", "pre", "sub", "sup", "em", "strong", "b", "i", "u", "strike", "big", "small", "pre", "h1", "h2", "h3", "h4", "h5", "h6"], // List of tags that should not be reformatted
    "wrap_line_length": 0 // Lines should wrap at next opportunity after this number of characters (0 disables)
  },
  "css": {
    "allowed_file_extensions": ["css", "scss", "sass", "less"],
    "end_with_newline": false, // End output with newline
    "indent_char": " ", // Indentation character
    "indent_size": 4, // Indentation size
    "indent_with_tabs": true, // Indent with tabs, overrides `indent_size` and `indent_char`
    "newline_between_rules": true, // Add a new line after every css rule
    "selector_separator": " ",
    "selector_separator_newline": true // Separate selectors with newline or not (e.g. "a,\nbr" or "a, br")
  },
  "js": {
    "allowed_file_extensions": ["js", "json", "jshintrc", "jsbeautifyrc"],
    "brace_style": "collapse", // [collapse|expand|end-expand|none] Put braces on the same line as control statements (default), or put braces on own line (Allman / ANSI style), or just put end braces on own line, or attempt to keep them where they are
    "break_chained_methods": false, // Break chained method calls across subsequent lines
    "e4x": false, // Pass E4X xml literals through untouched
    "end_with_newline": false, // End output with newline
    "indent_char": " ", // Indentation character
    "indent_level": 0, // Initial indentation level
    "indent_size": 4, // Indentation size
    "indent_with_tabs": true, // Indent with tabs, overrides `indent_size` and `indent_char`
    "jslint_happy": true, // If true, then jslint-stricter mode is enforced
    "keep_array_indentation": false, // Preserve array indentation
    "keep_function_indentation": false, // Preserve function indentation
    "max_preserve_newlines": 0, // Maximum number of line breaks to be preserved in one chunk (0 disables)
    "preserve_newlines": true, // Whether existing line breaks should be preserved
    "space_after_anon_function": true, // Should the space before an anonymous function's parens be added, "function()" vs "function ()"
    "space_before_conditional": true, // Should the space before conditional statement be added, "if(true)" vs "if (true)"
    "space_in_empty_paren": false, // Add padding spaces within empty paren, "f()" vs "f( )"
    "space_in_paren": true, // Add padding spaces within paren, ie. f( a, b )
    "unescape_strings": false, // Should printable characters in strings encoded in \xNN notation be unescaped, "example" vs "\x65\x78\x61\x6d\x70\x6c\x65"
    "wrap_line_length": 0 // Lines should wrap at next opportunity after this number of characters (0 disables)
  }
}
```
  To use, enter: `ctrl + shift + h`


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

### VALign
  - A plugin for Sublime Text 2 and 3 that adds a shortcut to easily vertically-align the text around the cursor. Just press ```Cmd+\``` (Mac) or ```Ctrl+\``` (Windows/Linux) and the code around you will align itself.

### Install theme
  - https://github.com/wesbos/cobalt2

### Apply Emmet on JSX
  - http://wesbos.com/emmet-react-jsx-sublime/

# Add this to sublime text preferences

- Click `preferences` then `Settings - User`
- Add these lines of code to file and then save

```
{
	"always_prompt_for_file_reload": false,
	"always_show_minimap_viewport": false,
	"animation_enabled": true,
	"atomic_save": false,
	"auto_close_tags": true,
	"auto_complete": true,
	"auto_complete_commit_on_tab": false,
	"auto_complete_cycle": false,
	"auto_complete_delay": 50,
	"auto_complete_selector": "source - comment, meta.tag - punctuation.definition.tag.begin",
	"auto_complete_size_limit": 4194304,
	"auto_complete_triggers":
	[
		{
			"characters": "<",
			"selector": "text.html"
		}
	],
	"auto_complete_with_fields": false,
	"auto_find_in_selection": false,
	"auto_indent": true,
	"auto_match_enabled": true,
	"binary_file_patterns":
	[
		"*.jpg",
		"*.jpeg",
		"*.png",
		"*.gif",
		"*.ttf",
		"*.tga",
		"*.dds",
		"*.ico",
		"*.eot",
		"*.pdf",
		"*.swf",
		"*.jar",
		"*.zip"
	],
	"bold_folder_labels": false,
	"caret_extra_bottom": 3,
	"caret_extra_top": 3,
	"caret_extra_width": 2,
	"caret_style": "smooth",
	"close_windows_when_empty": false,
	"copy_with_empty_selection": true,
	"create_window_at_startup": true,
	"default_encoding": "UTF-8",
	"default_line_ending": "system",
	"detect_indentation": true,
	"dictionary": "Packages/Language - English/en_US.dic",
	"drag_text": false,
	"draw_centered": false,
	"draw_indent_guides": true,
	"draw_minimap_border": false,
	"draw_white_space": "all",
	"enable_hexadecimal_encoding": true,
	"enable_tab_scrolling": true,
	"enable_telemetry": "auto",
	"ensure_newline_at_eof_on_save": false,
	"fade_fold_buttons": true,
	"fallback_encoding": "Western (Windows 1252)",
	"file_exclude_patterns":
	[
		"*.pyc",
		"*.pyo",
		"*.exe",
		"*.dll",
		"*.obj",
		"*.o",
		"*.a",
		"*.lib",
		"*.so",
		"*.dylib",
		"*.ncb",
		"*.sdf",
		"*.suo",
		"*.pdb",
		"*.idb",
		".DS_Store",
		"*.class",
		"*.psd",
		"*.db",
		"*.sublime-workspace"
	],
	"find_selected_text": true,
	"fold_buttons": true,
	"folder_exclude_patterns":
	[
		".DS_Store",
		"Desktop.ini",
		"*.pyc",
		"._*",
		"Thumbs.db",
		".Spotlight-V100",
		".Trashes",
		".svn",
		".git",
		".hg",
		"CVS"
	],
	"font_face": "Andale Mono",
	"font_options":
	[
	],
	"font_size": 12,
	"gpu_window_buffer": "auto",
	"gutter": true,
	"highlight_line": true,
	"highlight_modified_tabs": false,
	"hot_exit": true,
	"ignored_packages":
	[
		"Vintage"
	],
	"indent_guide_options":
	[
		"draw_normal"
	],
	"indent_subsequent_lines": true,
	"indent_to_bracket": false,
	"index_exclude_patterns":
	[
		"*.log"
	],
	"index_files": true,
	"index_workers": 0,
	"line_numbers": true,
	"line_padding_bottom": 0,
	"line_padding_top": 0,
	"margin": 4,
	"match_brackets": true,
	"match_brackets_angle": false,
	"match_brackets_braces": true,
	"match_brackets_content": true,
	"match_brackets_square": true,
	"match_selection": true,
	"match_tags": true,
	"move_to_limit_on_up_down": false,
	"open_files_in_new_window": true,
	"overlay_scroll_bars": "system",
	"preview_on_click": true,
	"remember_full_screen": false,
	"rulers":
	[
	],
	"save_on_focus_lost": false,
	"scroll_past_end": true,
	"scroll_speed": 1.0,
	"shift_tab_unindent": false,
	"show_encoding": false,
	"show_full_path": true,
	"show_line_endings": false,
	"show_panel_on_build": true,
	"show_tab_close_buttons": true,
	"smart_indent": true,
	"spell_check": false,
	"spelling_selector": "markup.raw, source string.quoted - punctuation - meta.preprocessor.c.include, source comment - source comment.block.preprocessor, -(source, constant, keyword, storage, support, variable, markup.underline.link, meta.tag)",
	"tab_completion": true,
	"tab_size": 4,
	"translate_tabs_to_spaces": false,
	"tree_animation_enabled": true,
	"trim_automatic_white_space": true,
	"trim_trailing_white_space_on_save": false,
	"use_simple_full_screen": false,
	"use_tab_stops": true,
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
	"word_separators": "./\\()\"'-:,.;<>~!@#$%^&*|+=[]{}`~?",
	"word_wrap": "auto",
	"wrap_width": 0
}
```

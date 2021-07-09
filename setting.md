# setting เก่า

```text
{
	"editor.fontFamily": "FiraCode NF, Sarabun",
	"editor.fontLigatures": true,
	"editor.fontWeight": "300",
	"editor.colorDecorators": false,
	"editor.cursorBlinking": "smooth",
	"editor.maxTokenizationLineLength": 100000,
	"editor.suggestSelection": "first",

	"workbench.colorTheme": "Monokai Pro (Filter Spectrum)",
	"workbench.iconTheme": "material-icon-theme",
	"workbench.tree.indent": 15,
	"workbench.list.horizontalScrolling": true,
	"workbench.editor.wrapTabs": true,
	"workbench.editor.decorations.badges": true,
	"workbench.productIconTheme": "fluent-icons",

	"explorer.compactFolders": false,
	"explorer.autoReveal": false,

	"css.validate": false,
	"less.validate": false,
	"scss.validate": false,

	"editor.semanticTokenColorCustomizations": {
		"enabled": true
	},
	"editor.tokenColorCustomizations": {
		"[Monokai Pro (Filter Spectrum)]": {
			"comments": "#8b949e",
			"textMateRules": [
				{
					"scope": "constant.other.class.php",
					"settings": {
						"foreground": "#948AE3"
					}
				},
				{
					"scope": "entity.name.function.php",
					"settings": {
						"foreground": "#60db57"
					}
				}
			]
		}
	},

	"sync.gist": "dbf20d5df0c067ed4ed5ad8ac1c9fda4",
	"sync.forceUpload": true,

	"terminal.integrated.rendererType": "dom",
	"terminal.integrated.shell.windows": "C:\\WINDOWS\\System32\\WindowsPowerShell\\v1.0\\powershell.exe",
	"terminal.integrated.fontFamily": "FiraCode NF",
	"terminal.integrated.cursorStyle": "line",
	"terminal.integrated.cursorBlinking": true,

	"emmet.includeLanguages": {
		"javascript": "javascriptreact"
	},

	"php.suggest.basic": false,
	"php.validate.enable": false,
	"[php]": {
		"editor.defaultFormatter": "bmewburn.vscode-intelephense-client"
	},
	"intelephense.telemetry.enabled": false,
	"intelephense.format.enable": true,
	"intelephense.completion.triggerParameterHints": true,
	"intelephense.completion.insertUseDeclaration": true,
	"intelephense.trace.server": "messages",
	"intelephense.environment.shortOpenTag": true,
	"intelephense.files.exclude": [
		"**/.git/**",
		"**/.svn/**",
		"**/.hg/**",
		"**/CVS/**",
		"**/.DS_Store/**",
		"**/node_modules/**",
		"**/bower_components/**",
		"**/storage",
		"**/storage/**",
		"**/tests/**"
	],

	"[json]": {
		"editor.defaultFormatter": "esbenp.prettier-vscode",
		"editor.tabSize": 2
	},

	"[html]": {
		"editor.defaultFormatter": "esbenp.prettier-vscode"
	},

	"vetur.validation.template": true,
	"[vue]": {
		"editor.formatOnSave": false,
		"editor.defaultFormatter": "octref.vetur"
	},

	"[javascript]": {
		"editor.defaultFormatter": "esbenp.prettier-vscode",
		"editor.tabSize": 2
	},
	"javascript.updateImportsOnFileMove.enabled": "always",

	"eslint.alwaysShowStatus": true,

	"prettier.singleQuote": true,
	"prettier.semi": false,
	"prettier.useTabs": true,

	"[jsonc]": {
		"editor.defaultFormatter": "esbenp.prettier-vscode"
	},
	"gitlens.codeLens.enabled": false,

	"[dart]": {
		"editor.formatOnSave": true,
		"editor.formatOnType": true,
		"editor.rulers": [80],
		"editor.selectionHighlight": false,
		"editor.suggest.snippetsPreventQuickSuggestions": false,
		"editor.suggestSelection": "first",
		"editor.tabCompletion": "onlySnippets",
		"editor.wordBasedSuggestions": false
	},

	"html.format.wrapLineLength": 200,
	"[scss]": {
		"editor.defaultFormatter": "esbenp.prettier-vscode"
	},

	"headwind.prependCustomClasses": true,
	"headwind.customTailwindPrefix": "-",

	"html-css-class-completion.excludeGlobPattern": "{**/vendor/**,**/node_modules/**}",

	"namespaceResolver.sortAlphabetically": true,

	"[blade]": {
		"editor.defaultFormatter": "shufo.vscode-blade-formatter"
	},
	"blade.format.enable": true,

	"rest-client.requestNameAsResponseTabTitle": true,
	"rest-client.decodeEscapedUnicodeCharacters": true,

	"tailwindCSS.includeLanguages": {
		"php": "php",
		"html": "html",
		"blade php": "blade.php",
		"blade": "blade",
		"javascript": "javascript",
		"vue": "vue"
	},
	"rest-client.previewColumn": "current",
	"gitlens.menus": {
		"editor": {
			"blame": false,
			"clipboard": true,
			"compare": true,
			"history": false,
			"remote": false
		},
		"editorGroup": {
			"blame": false,
			"compare": true
		},
		"editorTab": {
			"clipboard": true,
			"compare": true,
			"history": true,
			"remote": true
		},
		"explorer": {
			"clipboard": true,
			"compare": true,
			"history": true,
			"remote": true
		},
		"scm": {
			"authors": true
		},
		"scmGroupInline": {
			"stash": true
		},
		"scmGroup": {
			"compare": true,
			"openClose": true,
			"stash": true
		},
		"scmItem": {
			"clipboard": true,
			"compare": true,
			"history": true,
			"remote": false,
			"stash": true
		}
	},

	"vetur.format.styleInitialIndent": true,
	"vetur.format.scriptInitialIndent": true,

	// custom color
	"workbench.colorCustomizations": {
		"focusBorder": "#388bfd",
		"foreground": "#c9d1d9",
		"descriptionForeground": "#8b949e",
		"errorForeground": "#f85149",
		"textLink.foreground": "#58a6ff",
		"textLink.activeForeground": "#58a6ff",
		"textBlockQuote.background": "#06090f",
		"textBlockQuote.border": "#3b434b",
		"textCodeBlock.background": "#f0f6fc26",
		"textPreformat.foreground": "#8b949e",
		"textSeparator.foreground": "#21262d",
		"button.background": "#238636",
		"button.foreground": "#ffffff",
		"button.hoverBackground": "#2ea043",
		"checkbox.background": "#161b22",
		"checkbox.border": "#30363d",
		"dropdown.background": "#21262d",
		"dropdown.border": "#30363d",
		"dropdown.foreground": "#c9d1d9",
		"dropdown.listBackground": "#21262d",
		"input.background": "#0d1117",
		"input.border": "#21262d",
		"input.foreground": "#c9d1d9",
		"input.placeholderForeground": "#484f58",
		"badge.foreground": "#79c0ff",
		"badge.background": "#0d419d",
		"progressBar.background": "#1f6feb",
		"titleBar.activeForeground": "#F0F6FC",
		"titleBar.activeBackground": "#161B22",
		"titleBar.inactiveForeground": "#F0F6FC",
		"titleBar.inactiveBackground": "#161B22",
		"titleBar.border": "#30363d",
		"activityBar.foreground": "#C9D1D9",
		"activityBar.inactiveForeground": "#8b949e",
		"activityBar.background": "#161B22",
		"activityBarBadge.foreground": "#F0F6FC",
		"activityBarBadge.background": "#DA3633",
		"activityBar.activeBorder": "#DA3633",
		"activityBar.border": "#30363d",
		"sideBar.foreground": "#C9D1D9",
		"sideBar.background": "#0D1117",
		"sideBar.border": "#30363D",
		"sideBarTitle.foreground": "#fff",
		"sideBarSectionHeader.foreground": "#c9d1d9",
		"sideBarSectionHeader.background": "#06090f",
		"sideBarSectionHeader.border": "#30363d",
		"list.hoverForeground": "#8b949e",
		"list.inactiveSelectionForeground": "#E3B341",
		"list.activeSelectionForeground": "#E3B341",
		"list.hoverBackground": "#161b22",
		"list.inactiveSelectionBackground": "#161b22",
		"list.activeSelectionBackground": "#21262d",
		"list.focusForeground": "#f0f6fc",
		"list.focusBackground": "#30363D",
		"list.inactiveFocusBackground": "#161b22",
		"list.highlightForeground": "#388bfd",
		"tree.indentGuidesStroke": "#21262d",
		"notificationCenterHeader.foreground": "#6e7681",
		"notificationCenterHeader.background": "#0d1117",
		"notifications.foreground": "#8b949e",
		"notifications.background": "#161b22",
		"notifications.border": "#30363d",
		"notificationsErrorIcon.foreground": "#f85149",
		"notificationsWarningIcon.foreground": "#f0883e",
		"notificationsInfoIcon.foreground": "#58a6ff",
		"pickerGroup.border": "#21262d",
		"pickerGroup.foreground": "#8b949e",
		"quickInput.background": "#0d1117",
		"quickInput.foreground": "#c9d1d9",
		"statusBar.foreground": "#58A6FF",
		"statusBar.background": "#161B22",
		"statusBar.border": "#30363d",
		"statusBar.noFolderBackground": "#0d1117",
		"statusBar.debuggingBackground": "#da3633",
		"statusBar.debuggingForeground": "#f0f6fc",
		"statusBarItem.prominentBackground": "#161b22",
		"editorGroupHeader.tabsBackground": "#06090f",
		"editorGroupHeader.tabsBorder": "#30363d",
		"editorGroup.border": "#30363d",
		"tab.activeForeground": "#C9D1D9",
		"tab.inactiveForeground": "#8b949e",
		"tab.inactiveBackground": "#0D1117",
		"tab.activeBackground": "#161B22",
		"tab.hoverBackground": "#161B22",
		"tab.unfocusedHoverBackground": "#161B22",
		"tab.border": "#30363D",
		"tab.unfocusedActiveBorderTop": "#30363d",
		"tab.activeBorder": "#DA3633",
		"tab.unfocusedActiveBorder": "#0d1117",
		"tab.activeBorderTop": "#DA3633",
		"breadcrumb.foreground": "#8b949e",
		"breadcrumb.focusForeground": "#c9d1d9",
		"breadcrumb.activeSelectionForeground": "#8b949e",
		"breadcrumbPicker.background": "#21262d",
		"editor.foreground": "#c9d1d9",
		"editor.background": "#0D1117",
		"editorWidget.background": "#21262d",
		"editor.foldBackground": "#06090f",
		"editor.lineHighlightBackground": "#1073cf2d",
		"editorLineNumber.foreground": "#51565C",
		"editorLineNumber.activeForeground": "#959BA0",
		"editorIndentGuide.background": "#21262d",
		"editorIndentGuide.activeBackground": "#30363d",
		"editorWhitespace.foreground": "#484f58",
		"editorCursor.foreground": "#79c0ff",
		"editor.findMatchBackground": "#ffd33d44",
		"editor.findMatchHighlightBackground": "#ffd33d22",
		"editor.inactiveSelectionBackground": "#3392FF22",
		"editor.selectionBackground": "#3392FF44",
		"editor.selectionHighlightBackground": "#17E5E633",
		"editor.selectionHighlightBorder": "#17E5E600",
		"editor.wordHighlightBackground": "#17E5E600",
		"editor.wordHighlightStrongBackground": "#17E5E600",
		"editor.wordHighlightBorder": "#17E5E699",
		"editor.wordHighlightStrongBorder": "#17E5E666",
		"editorBracketMatch.background": "#515a6b0f",
		"editorBracketMatch.border": "#ddddddaf",
		"editorGutter.modifiedBackground": "#9e6a03",
		"editorGutter.addedBackground": "#196c2e",
		"editorGutter.deletedBackground": "#b62324",
		"diffEditor.insertedTextBackground": "#23863626",
		"diffEditor.removedTextBackground": "#da363326",
		"scrollbar.shadow": "#0008",
		"scrollbarSlider.background": "#4e566660",
		"scrollbarSlider.hoverBackground": "#5a637580",
		"scrollbarSlider.activeBackground": "#747d9180",
		"editorOverviewRuler.border": "#010409",
		"panel.background": "#06090f",
		"panel.border": "#30363d",
		"panelTitle.activeBorder": "#f9826c",
		"panelTitle.activeForeground": "#c9d1d9",
		"panelTitle.inactiveForeground": "#8b949e",
		"panelInput.border": "#30363d",
		"terminal.foreground": "#F0F6FC",
		"gitDecoration.addedResourceForeground": "#56d364",
		"gitDecoration.modifiedResourceForeground": "#e3b341",
		"gitDecoration.deletedResourceForeground": "#f85149",
		"gitDecoration.untrackedResourceForeground": "#56d364",
		"gitDecoration.ignoredResourceForeground": "#8b949e",
		"gitDecoration.conflictingResourceForeground": "#e3b341",
		"gitDecoration.submoduleResourceForeground": "#8b949e",
		"debugToolBar.background": "#21262d",
		"editor.stackFrameHighlightBackground": "#a707",
		"editor.focusedStackFrameHighlightBackground": "#b808",
		"peekViewEditor.matchHighlightBackground": "#ffd33d33",
		"peekViewResult.matchHighlightBackground": "#30363D",
		"peekViewEditor.background": "#0D1117",
		"peekViewResult.background": "#0D1117",
		"settings.headerForeground": "#8b949e",
		"settings.modifiedItemIndicator": "#9e6a03",
		"welcomePage.buttonBackground": "#21262d",
		"welcomePage.buttonHoverBackground": "#30363d",
		"menu.background": "#21262D",
		"menu.foreground": "#C9D1D9",
		"menu.selectionBackground": "#1F6FEB",
		"menu.selectionForeground": "#F0F6FC",
		"tab.unfocusedActiveBackground": "#161B22",
		"editorGutter.background": "#0D1117",
		"editorSuggestWidget.background": "#21262D",
		"editorSuggestWidget.selectedBackground": "#30363D",
		"editorSuggestWidget.foreground": "#F0F6FC",
		"editorHoverWidget.background": "#21262D",
		"editorHoverWidget.statusBarBackground": "#30363D",
		"editor.hoverHighlightBackground": "#30363D",
		"problemsWarningIcon.foreground": "#F0883E",
		"problemsInfoIcon.foreground": "#388BFD",
		"problemsErrorIcon.foreground": "#DA3633",
		"peekViewEditorGutter.background": "#21262D",
		"peekView.border": "#30363D",
		"peekViewResult.selectionForeground": "#C8D0D8",
		"peekViewResult.selectionBackground": "#30363D",
		"peekViewResult.lineForeground": "#C8D0D8",
		"peekViewResult.fileForeground": "#C8D0D8",
		"peekViewTitle.background": "#21262D",
		"peekViewTitleDescription.foreground": "#C8D0D8",
		"terminal.background": "#0D1117",
		"terminalCursor.background": "#C5C8C6",
		"terminalCursor.foreground": "#C5C8C6",
		"terminal.ansiBlack": "#1D1F21",
		"terminal.ansiBlue": "#399ced",
		"terminal.ansiBrightBlack": "#969896",
		"terminal.ansiBrightBlue": "#388BFD",
		"terminal.ansiBrightCyan": "#388BFD",
		"terminal.ansiBrightGreen": "#3FB950",
		"terminal.ansiBrightMagenta": "#6E40C9",
		"terminal.ansiBrightRed": "#DA3633",
		"terminal.ansiBrightWhite": "#FFFFFF",
		"terminal.ansiBrightYellow": "#E3B341",
		"terminal.ansiCyan": "#388BFD",
		"terminal.ansiGreen": "#3FB950",
		"terminal.ansiMagenta": "#6E40C9",
		"terminal.ansiRed": "#DA3633",
		"terminal.ansiWhite": "#C5C8C6",
		"terminal.ansiYellow": "#E3B341",
		"editor.lineHighlightBorder": "#9fced11f"
	},
	"vetur.experimental.templateInterpolationService": true,
	"intelephense.references.exclude": ["**/vendor/**", "**/node_modules/**"],
	"intelephense.rename.exclude": ["**/vendor/**", "**/node_modules/**"],
	"tabnine.experimentalAutoImports": true,
	"diffEditor.ignoreTrimWhitespace": false,
	"editor.linkedEditing": true,
	"workbench.editor.untitled.hint": "hidden",
	"editor.wordWrap": "off",
	"diffEditor.wordWrap": "off",
	"[markdown]": {
		"editor.wordWrap": "off",
		"editor.quickSuggestions": false
	},
	"editor.renderIndentGuides": false,
	"editor.highlightActiveIndentGuide": false,
	"bladeFormatter.format.wrapAttributes": "force",
	"remote.SSH.remotePlatform": {
		"139.180.214.34": "linux",
		"root": "linux"
	},
	"tailwindCSS.experimental.classRegex": [
		// https://github.com/tailwindlabs/tailwindcss-intellisense/issues/129
		// javascript object
		[":\\s*?[\"'`]([^\"'`]*).*?,"]
	],
	"editor.inlineSuggest.enabled": true,
	"typescript.tsserver.log": "verbose"
}

```


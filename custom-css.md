# custom css

{% embed url="https://github.com/be5invis/vscode-custom-css" %}



{% embed url="https://github.com/microsoft/vscode/issues/70413" %}

```text
.monaco-workbench
	.part.editor
	> .content
	.editor-group-container
	> .title.tabs
	> .tabs-and-actions-container
	> .monaco-scrollable-element {
	height: initial !important;
}

.monaco-workbench
	.part.editor
	> .content
	.editor-group-container
	> .title
	.tabs-container {
	height: initial !important;
	flex-wrap: wrap;
}

.monaco-workbench
	.part.editor
	> .content
	.editor-group-container
	> .title
	.tabs-container
	> .tab {
	flex-grow: 1;
	border-bottom: 1px solid rgba(128, 128, 128, 0.5);
}

```


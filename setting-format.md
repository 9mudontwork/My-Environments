# setting ตัวช่วย format

.editorconfig

```text
# EditorConfig is awesome: https://EditorConfig.org

# top-most EditorConfig file
root = true

[*]
indent_style = space
indent_size = 4
end_of_line = crlf
charset = utf-8
trim_trailing_whitespace = true
insert_final_newline = true
```

.prettierrc

```text
{
  "printWidth": 160,
  "tabWidth": 2,
  "useTabs": false,
  "semi": false,
  "singleQuote": true,
  "trailingComma": "es5",
  "bracketSpacing": true,
  "arrowParens": "always"
}

```

jsconfig.json \(ตัวอย่าง\)

```text
{
    "compilerOptions": {
        "baseUrl": ".",
        "paths": {
            "@frontendHelpers/*": ["./frontend/resources/js/helpers/*"],
            "@frontendUtils/*": ["./frontend/resources/js/utils/*"],

            "@backendHelpers/*": ["./backend/resources/js/helpers/*"],
            "@backendUtils/*": ["./backend/resources/js/utils/*"],
        }
    },
    "exclude": ["node_modules", "vendor"]
}

```


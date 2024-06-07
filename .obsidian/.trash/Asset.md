## 1.47.15512 (May 28, 2024)

### Blade `.Blade.Php` Support

- Supports `@use` directive including type aliases. The code completion and IntelliSense recognized imported and aliased classes properly.
- Highlighting of `@class` directive and other inside HTML tags.
- Opening and closing blade tags highlighted as PHP keywords and HTML begin/end token.
- Improves completion of PHP code, PHP functions signature help, and PHP code folding in blade files.
- Stability fixes.

![Blade @Use completion](https://raw.githubusercontent.com/DEVSENSE/phptools-docs/master/docs/vscode/imgs/vsc-blade-use.gif)

### Diagnostics

- Respects `/** @ignore $variablename */` so if the `$variablename` is unused, the problem is not reported.
- Supports more complex conditional return type, i.e. `@return ($name is class-string<T> ? T : bool)` ([#538](https://github.com/DEVSENSE/phptools-docs/issues/538 "https://github.com/DEVSENSE/phptools-docs/issues/538")).
- Fixes false unreachable code warning ([#556](https://github.com/DEVSENSE/phptools-docs/issues/556 "https://github.com/DEVSENSE/phptools-docs/issues/556")).
- Handles checks for `method_exists` and `function_exists` to avoid false warning about unknown functions.

### New Features

- Infering lambda function parameters type from target `callable()` PHPDoc type annotation.
- Added inlay hint for infered lambda parameter types. Enable `"php.inlayHints.types.lambdaParameter"` setting.

![Inlay for infered lambda parameters](https://raw.githubusercontent.com/DEVSENSE/phptools-docs/master/docs/vscode/imgs/inlay-lambda-parameter-type.png)

### Rename Refactoring

The rename refactoring has been partially reimplemented, new rename scenarios have been implemented, and various cases fixed. The refactoring handles class/const/function imports correctly, template type names, occurences of names in strings and arrays, and more.

#### New Features

- **Renaming aliased type names correctly** so when renaming a type alias which differs from the original type, only the alias is renamed.
- **Renaming aliased functions and constants** behaves correctly now.
- **Renaming generic types** has been fixed and optimized.
- **Renaming imported template types** has been implemented. This works for various PHPDoc tags like `@phpstan-import-from`, `@psalm-type`, etc.
- **Find references** to template type names and type names fixed and new scenarios handled correctly.

Please let us know if there any issues with rename refactoring - we’re keen to improve.

_Known missing features:_ rename namespace, rename named arguments. Work in progress.

### Improvements

- Folding for colon blocks (`if:`, `switch:`, `while:`, `for:`, `foreach:`).
- Improves mouse hovers for `by-ref` functions.
- Blade formatter indents PHPDoc blocks in `.blade.php` files correctly.
- Adds selection range inside function header parameters.
- Expanding selection range to corresponding PHPDoc block.
- Generating getters/setters adjust the whole identifier to match `"php.completion.namingConvention"` setting. ([#2011](https://community.devsense.com/d/2011-getters-setters-function-case "https://community.devsense.com/d/2011-getters-setters-function-case"))

### Fixes

- Fixes unwanted space before named arguments which happens to be keywords as well. [#555](https://github.com/DEVSENSE/phptools-docs/issues/555 "https://github.com/DEVSENSE/phptools-docs/issues/555")
- All PHP child processes are killed after stopping debug sessions. [#542](https://github.com/DEVSENSE/phptools-docs/issues/542 "https://github.com/DEVSENSE/phptools-docs/issues/542")
- Fixes _Outline_ when there is an anonymus `class` ([#557](https://github.com/DEVSENSE/phptools-docs/issues/557 "https://github.com/DEVSENSE/phptools-docs/issues/557")).
- Fixes L-Value variables type in mouse hover.
- Fixes unwatend space after `empty` in lambda function [#564](https://github.com/DEVSENSE/phptools-docs/issues/564 "https://github.com/DEVSENSE/phptools-docs/issues/564")
- Resolved an issue where setting or removing breakpoints during an active debug session caused VSCode to incorrectly flag them as unverified.

## 1.46.15409 (May 9, 2024)

### Features

- Inline suggestion after `namespace`.
- Folding blade blocks.
- Completion for blade tags.
- `.blade.php` files formatting (must be opened as a PHP file).

### Blade Formatting

The blade (`.blade.php` files) code formatting has been implemented. The formatter combines HTML/CSS/JS and PHP pretty print and PHP indentation, together with blade blocks indentation.

There are no further settings (yet). Based on your feedback, we’ll be adding more settings and fixes!

![Blade Formatting](https://raw.githubusercontent.com/DEVSENSE/phptools-docs/master/docs/vscode/imgs/vsc-blade-format.gif)

> Note, if you have another Blade extension, this feature might not be available. Make sure, the language of opened `.blade.php` file is set to `PHP` (the lower right corner of your VSCode window).

### HTML Auto Closing Tags And Attributes

In PHP code, HTML tag elements now close automatically when you type the `>` of the opening tag. Similarly, when you enter the `/` of the closing tag, a matching closing tag is inserted seamlessly.

Additionally, HTML attribute quotes are now automatically included when you type `=`.

### Auto Renaming HTML Tags

Auto-renaming HTML tags is enabled by default now. You can disable this feature using the following setting in your VSCode’s `settings.json`:

```json
"[php]": {
    "editor.linkedEditing": false
}
```

![Auto-Renaming HTML Tags](https://raw.githubusercontent.com/DEVSENSE/phptools-docs/master/docs/vscode/imgs/vsc-html-linkededit.gif)

### Improvements

- Performance and memory usage improvements.
- Shrink/expand selection works in HTML part of the php files and blade files (`Shift+Alt+Left` and `Shift+Alt+Right`)

### Fixes

- Fixes override checks for `static` return types.
- Fixes inlay hints in `.blade.php` files when modifying code.
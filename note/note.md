# Note
To learn more about how to install and use SASS, [click on this link](https://sass-lang.com).

## Why even use SASS?
- Separation of concerns
- DRY
- Readability
- Maintainability
- Additional useful functionality like `@mixin`s

## Installation of SASS
### Via NPM
```pwsh
npm install -g sass
```

Somewhat slower than the default Dart implementation.

### Via Chocolatey
```pwsh
choco install sass
```

### Via Scoop
```pwsh
scoop install sass
```

### Via downloading on GitHub
Head over to https://github.com/sass/dart-sass/releases/tag/1.86.3
> Check if a newer version is released and install the latest version 


## Folder structure
```md
|---- scss
|   |---- base
|   |   |---- animations
|   |   |---- callouts
|   |   |---- checkboxes
|   |   |---- editor
|   |   |---- foundations
|   |   |   |---- background
|   |   |   |---- buttons
|   |   |   |---- colors
|   |   |   |---- editor
|   |   |   |---- embeds
|   |   |   |---- metadata
|   |   |   |---- min_widths
|   |   |   |---- slider
|   |   |   |---- tags
|   |   |   |---- toggles
|   |   |   |---- typography
|   |   |---- icons
|   |   |---- links
|   |   |---- metadata
|   |   |---- modals
|   |   |---- navigation
|   |   |---- new_tab
|   |   |---- prompts
|   |   |---- scrollbar
|   |   |---- search
|   |   |---- settings
|   |   |---- slider
|   |   |---- status_bar
|   |   |---- tables
|   |   |---- tabs
|   |---- modifiers
|   |   |---- plugins
|   |   |   |---- dataview
|   |   |   |---- kanban
|   |   |---- snippets
```

## What I have done
In each folder, there is a corresponding `_<folder_name>.scss`. This is a partial CSS file (which tells the SASS compiler not to output a separate CSS file) which holds references to other `_<function_name>.scss` files in their current or sub-directories.
> Partial files are prefixed with `_`. E.g. `_tables.scss`

### Do I have to learn another set of syntax?
Not really. Other than some handy add-ons for SASS.
> Which will be covered briefly

SASS is very much committed to be completely compatible with CSS, specifically for files with the `.scss` extension. 
Files with the `.sass` extension are more YAML flavoured but still have feature parity but a different syntax.

### An example
Let's take the example of how the CSS defined in `_dataview.scss` gets renders in `theme.css` eventually.

#### 1. Calling the command
Open a terminal of your choice. Ensure the current directory is at the project root.
Then, run `sass --watch --no-source-map scss/theme.scss theme.css`.

> ##### What do the flags mean?
> `--watch`: Watch for changes when the command is running. Will recompile the `.scss` files into `theme.css` when changes are made in any of them while the command is running.
>
> `--no-source-map`: By default, SASS adds the source map (a list of references to `.scss` files) to the output css file. This flag disables that behaviour

#### 2. The SASS compiler checks for references between `.scss/.sass` files. 
These are defined with `@use` calls.

```scss
// scss/modifiers/plugins/_plugins.scss
@use "./dataview/dataview";
@use "./kanban/kanban";
```

> `@use` takes the contents of the referenced `.scss` file and adds it to what will be rendered for `_plugins.scss`

The `_plugins.scss` file is then referenced by the `_modifiers.scss` file.
> This will bring over the `@use` references from `_plugins.scss`

```scss
// scss/modifiers/_modifiers.scss
@use "./plugins/plugins";
```

and so on

```scss
// scss/theme.scss
@use "./base/base";
@use "./modifiers/modifiers";
```

#### 3. Parsing
At this step the compiler recognises that the `scss/theme.scss` file is not a partial file. It also knows that we want are telling it to take `theme.scss` (along with its references), and output the compiled css to a file called `theme.css` at the project root.

It compiles and we get `theme.css`.

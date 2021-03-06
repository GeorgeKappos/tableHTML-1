# tableHTML 1.0.1

* Fixed a bug where characters < or > in the data would open / close tags and would cause problem with the rendering of the table.
* Argument column_names in `add_css_column` has been deprecated. Use `columns` instead.
* Argument columns in `add_css_column` `add_css_column` now can accept both column names and indices.
* Changed the way ids are created for table (table_xxxx), column (tableHTML_column_x), header (tableHTML_header_x)
* Added argument `headers` in `tableHTML()` to allow the user input alternative headers.
* Fixed other small bugs.
* Small code optimisations.

# tableHTML 0.2.11

* Added `make_css` function. This function makes it easy to generate a css file. In shiny it can be used either to create a a file or directly in the ui.R file. You can see the `make_css` vignette for a detailed explanation.
* Added `render_tableHTML` and `tableHTML_output` functions to use with shiny. This makes it easier for users to find the appropriate functions (people had to see the online documentation or the vignettes in order to understand that they needed to use `renderUI` and `uiOutput`, so I decided to add these new functions in the package) in order to implement tableHTML with shiny. These functions are directly included in the package so users can call them directly (internally these functions are simple calls to `renderUI` and `uiOutput` which could also be called instead).
* Added a `make_css` vignette with examples and detailed explanations about `make_css` function.
* Added more information in the package documentation.
* Various code optimizations.

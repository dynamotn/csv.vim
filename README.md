INTRODUCTION
==============================================================================

A mirror of the [wikia csv plugin](http://vim.wikia.com/wiki/Csv)
and integrate with vim-airline

KEYBOARD
==============================================================================

Key | Mode   | Description
--- | ----   | -----------
H   | normal | Move left one column in the CSV.
J   | normal | Move down one row in the CSV (stay in focused column).
K   | normal | Move up one row in the CSV (stay in focused column).
L   | normal | Move right one column in the CSV.
0   | normal | Move to the first column.
$   | normal | Move to the last column.
gm  | normal | Jump back to focused column/row.

COMMAND
==============================================================================

Command    | Description
-------    | -----------
:Delimiter | Change the delimiter for a file. Takes a single character.
:DC        | Delete the current column.
:SC        | Search the current column.
:Csv #     | Highlight a specific column (0 to turn off).
:HL #      | Set the heading line number
:Sort      | Sort by the current column. Can sort visually selected regions.
:CC        | Copy the current column.
:GC #      | Go to a specific column

VARIABLE
==============================================================================

Variable                  | Description                           | Default
-------                   | -----------                           | -------
b:csv_heading_line_number | Index of column header line in buffer | 1
g:csv_show_column         | Show column header on status line     | 1
g:csv_excel_column_format | Show column number by Excel format    | 0

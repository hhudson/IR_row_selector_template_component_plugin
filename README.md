# IR Row Selector plugin

## Description

A Plugin for Interactive Reports to replicate the APEX$ROW_SELECTOR functionality of the Interactive Grid. With this column type to your Interactive Report, selecting rows will automatically add the "primary key" of your choice to a javascript array named `irrs.PKs`:
![Intro image](img/intro.png)

## How to configure

- Step 1 : Install the plugin
  ![Install image](img/import.png)
- Step 2 : Create an Interactive Report
- Step 3 : Designate / create a column to become your "row selector" column
  ![column type image](img/column_type.png)
- Step 4: Replace the heading
  ![heading image](img/heading.png)
  Add the following heading for "Select All" functionality:
  `<span class="irrsHeader u-selector" role="checkbox" aria-checked="false" aria-label="Select All Rows" title="Select All" aria-disabled="false" onclick="javascript:irrs.SelectAll(this);"></span>`.
  (Be sure to align the heading and the column so that it looks good.)

## Recommendation on how to use

Once configured, selecting rows in your IR will automatically populate a javascript array named `irrs.PKs`:
![Intro image](img/intro.png)

- Step 1: Add a page item
- Step 2 : Add a button
  ...

---
title: HeaderTooltips
permalink: /next/api/header-tooltips
canonicalUrl: /api/header-tooltips
---

# {{ $frontmatter.title }}

[[toc]]

## Description


Allows to add a tooltip to the table headers.

Available options:
* the `rows` property defines if tooltips should be added to row headers,
* the `columns` property defines if tooltips should be added to column headers,
* the `onlyTrimmed` property defines if tooltips should be added only to headers, which content is trimmed by the header itself (the content being wider then the header).


**Example**  
```js
const container = document.getElementById('example');
const hot = new Handsontable(container, {
  data: getData(),
  // enable and configure header tooltips
  headerTooltips: {
    rows: true,
    columns: true,
    onlyTrimmed: false
  }
});
```
## Functions:

### destroy
`headerTooltips.destroy()`

Destroys the plugin instance.



### disablePlugin
`headerTooltips.disablePlugin()`

Disables the plugin functionality for this Handsontable instance.



### enablePlugin
`headerTooltips.enablePlugin()`

Enables the plugin functionality for this Handsontable instance.



### isEnabled
`headerTooltips.isEnabled() ⇒ boolean`

Checks if the plugin is enabled in the handsontable settings. This method is executed in [Hooks#beforeInit](./Hooks/#beforeInit)
hook and if it returns `true` than the [enablePlugin](#HeaderTooltips+enablePlugin) method is called.


---
id: dxTreeList.Options.onDataErrorOccurred
type: function(e)
---
---
##### shortDescription
A function that is executed when an error occurs in the data source.

##### param(e): ui/tree_list:DataErrorOccurredEvent
Information on the occurred error.

##### field(e.component): {WidgetName}
The UI component's instance.

##### field(e.element): DxElement
#include common-ref-elementparam with { element: "UI component" }

##### field(e.model): any
Model data. Available only if you use Knockout.

##### field(e.error): Error
The standard <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Error" target="_blank">Error</a> object that defines the error.

---
Handles errors that might occur in the data source. To obtain a human-readable description of the error in the function, use the **error.message** field.
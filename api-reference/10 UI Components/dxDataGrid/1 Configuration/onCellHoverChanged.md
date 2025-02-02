---
id: dxDataGrid.Options.onCellHoverChanged
type: function(e)
default: null
---
---
##### shortDescription
A function that is executed after the pointer enters or leaves a cell.

##### param(e): ui/data_grid:CellHoverChangedEvent
Information about the event that caused the function's execution.

##### field(e.cellElement): DxElement
#include common-ref-elementparam with { element: "cell" }

##### field(e.column): dxDataGridColumn
This column's [configuration](/api-reference/10%20UI%20Components/dxDataGrid/1%20Configuration/columns '/Documentation/ApiReference/UI_Components/dxDataGrid/Configuration/columns/').

##### field(e.columnIndex): Number
The index of the column to which the cell belongs. For details on indexes, see the [Column and Row Indexes](/concepts/05%20UI%20Components/DataGrid/15%20Columns/12%20Column%20and%20Row%20Indexes.md '/Documentation/Guide/UI_Components/DataGrid/Columns/Column_and_Row_Indexes/') topic.

##### field(e.component): {WidgetName}
The UI component's instance.

##### field(e.data): Object
The data of the row to which the cell belongs.

##### field(e.displayValue): any
The cell's displayed value. Differs from the **value** field only when the column to which the current cell belongs uses [lookup](/api-reference/_hidden/GridBaseColumn/lookup '/Documentation/ApiReference/UI_Components/dxDataGrid/Configuration/columns/lookup/').

##### field(e.element): DxElement
#include common-ref-elementparam with { element: "UI component" }

##### field(e.eventType): String
Indicates whether the pointer entered or left the cell. Can be either *"mouseover"* or *"mouseout"*.

##### field(e.key): any
The row's key. If a field providing keys is not specified in the [data source](/api-reference/10%20UI%20Components/GridBase/1%20Configuration/dataSource.md '/Documentation/ApiReference/UI_Components/dxDataGrid/Configuration/#dataSource'), the whole data object is considered the key.

##### field(e.model): any
Model data. Available only if you use Knockout.

##### field(e.row): dxDataGridRowObject
The row [properties](/api-reference/10%20UI%20Components/dxDataGrid/6%20Row '/Documentation/ApiReference/UI_Components/dxDataGrid/Row/').

##### field(e.rowIndex): Number
The row's index. Refer to [Column and Row Indexes](/concepts/05%20UI%20Components/DataGrid/15%20Columns/12%20Column%20and%20Row%20Indexes.md '/Documentation/Guide/UI_Components/DataGrid/Columns/Column_and_Row_Indexes/') for more information.

##### field(e.rowType): String
The row's [type](/api-reference/10%20UI%20Components/dxDataGrid/6%20Row/rowType.md '/Documentation/ApiReference/UI_Components/dxDataGrid/Row/#rowType').

##### field(e.text): String
The cell's [formatted](/api-reference/_hidden/dxDataGridColumn/format.md '/Documentation/ApiReference/UI_Components/dxDataGrid/Configuration/columns/#format') value converted to a string.

##### field(e.value): any
The cell's raw value.

---
To identify whether the pointer has entered or left the cell, check the **eventType** field's value.

#include btn-open-github with {
    href: "https://github.com/DevExpress-Examples/devextreme-datagrid-multiple-cell-selection"
}
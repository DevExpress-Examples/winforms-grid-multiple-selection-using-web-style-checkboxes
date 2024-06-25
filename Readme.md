<!-- default badges list -->
![](https://img.shields.io/endpoint?url=https://codecentral.devexpress.com/api/v1/VersionRange/128632513/13.1.4%2B)
[![](https://img.shields.io/badge/Open_in_DevExpress_Support_Center-FF7200?style=flat-square&logo=DevExpress&logoColor=white)](https://supportcenter.devexpress.com/ticket/details/E1271)
[![](https://img.shields.io/badge/📖_How_to_use_DevExpress_Examples-e9f6fc?style=flat-square)](https://docs.devexpress.com/GeneralInformation/403183)
[![](https://img.shields.io/badge/💬_Leave_Feedback-feecdd?style=flat-square)](#does-this-example-address-your-development-requirementsobjectives)
<!-- default badges end -->


# Multiple selection using checkbox (web style)

Starting with version **13.2**, <strong>GridView</strong> provides a built-in checkbox column for multiple row selection. So, to enable this type of multiple row selection in newer versions, it is sufficient to enable the <a href="https://documentation.devexpress.com/WindowsForms/DevExpress.XtraGrid.Views.Base.ColumnViewOptionsSelection.MultiSelect.property"><strong>GridViewOptionsSelection.MultiSelect</strong></a><strong> </strong>option and then set the <a href="https://documentation.devexpress.com/WindowsForms/DevExpress.XtraGrid.Views.Grid.GridOptionsSelection.MultiSelectMode.property"><strong>GridView.OptionsSelection.MultiSelectMode</strong></a><strong> </strong>property to the <a href="https://documentation.devexpress.com/WindowsForms/DevExpress.XtraGrid.Views.Grid.GridMultiSelectMode.enum"><strong>GridMultiSelectMode.CheckBoxRowSelect</strong></a><strong> </strong>value. 

Starting with version **18.1**, in multiple row selection mode, you can sync row selected states with a Boolean field in the bound data source. The selection binding mode ensures that row selection persists whenever you filter or group grid data. Refer to the [Multiple Row Selection via Built-In Check Column and Selection Binding](https://documentation.devexpress.com/WindowsForms/16439/Controls-and-Libraries/Data-Grid/Focus-and-Selection-Handling/Multiple-Row-Selection-via-Built-In-Check-Column-and-Selection-Binding) help article for more information.

## ***If the built-in CheckBox column does not suit you, we will be happy to find the most appropriate solution for you if you describe your real-life scenario. Just click   [here](https://www.devexpress.com/Support/Center/Question/Create) to submit a ticket to our Support Center.***


<b>See also:</b>

[DevExpress WinForms Troubleshooting - Grid Control](https://go.devexpress.com/CheatSheets_WinForms_Examples_T934742.aspx)
=======
![](https://img.shields.io/endpoint?url=https://codecentral.devexpress.com/api/v1/VersionRange/128632513/13.1.4%2B)
[![](https://img.shields.io/badge/Open_in_DevExpress_Support_Center-FF7200?style=flat-square&logo=DevExpress&logoColor=white)](https://supportcenter.devexpress.com/ticket/details/E1271)
[![](https://img.shields.io/badge/📖_How_to_use_DevExpress_Examples-e9f6fc?style=flat-square)](https://docs.devexpress.com/GeneralInformation/403183)
<!-- default badges end -->
# Multiple selection using checkbox (web style)


<p><strong>Important note.</strong></p>
<p>Starting with version 13.2, <strong>GridView</strong> provides a built-in checkbox column for multiple row selection. So, to enable this type of multiple row selection in newer versions, it is sufficient to enable the <a href="https://documentation.devexpress.com/WindowsForms/DevExpress.XtraGrid.Views.Base.ColumnViewOptionsSelection.MultiSelect.property"><strong>GridViewOptionsSelection.MultiSelect</strong></a><strong> </strong>option and then set the <a href="https://documentation.devexpress.com/WindowsForms/DevExpress.XtraGrid.Views.Grid.GridOptionsSelection.MultiSelectMode.property"><strong>GridView.OptionsSelection.MultiSelectMode</strong></a><strong> </strong>property to the <a href="https://documentation.devexpress.com/WindowsForms/DevExpress.XtraGrid.Views.Grid.GridMultiSelectMode.enum"><strong>GridMultiSelectMode.CheckBoxRowSelect</strong></a><strong> </strong>value. Take a look at the <strong><a href="https://www.devexpress.com/Support/Center/p/E990">How to use an unbound check box column to select grid rows</a> </strong>example for sample code.<br><br><br>This example demonstrates how to add a check column to allow web-style multiple row selection. End-users can select/deselect rows, group rows or select/deselect all rows by clicking the column header. Changing a check box value does not initiate row editing. </p>
<p><img src="https://raw.githubusercontent.com/DevExpress-Examples/multiple-selection-using-checkbox-web-style-e1271/13.1.4+/media/17ac6e9d-e756-49eb-8d10-b57b281569cd.png"><br><br></p>
<p>All code related to selection resides in the <strong>GridCheckMarksSelection </strong>helper class. So, to implement this functionality in your application, you can simply add this class to your project and then create a new <strong>GridCheckMarksSelection </strong>instance.<br>Please note if you use the <strong><a href="http://documentation.devexpress.com/#WindowsForms/DevExpressXtraGridViewsGridGridViewAppearances_EvenRowtopic"><u>AppearanceEvenRow</u></a> </strong>and <strong><a href="http://documentation.devexpress.com/#WindowsForms/DevExpressXtraGridViewsGridGridViewAppearances_OddRowtopic"><u>AppearanceOddRow</u></a> </strong>styles, by default they have a higher priority than the <strong><a href="http://documentation.devexpress.com/#WindowsForms/DevExpressXtraGridViewsGridGridView_RowStyletopic"><u>RowStyle</u></a> </strong>event used for the selection in this example. To avoid drawing incorrect selected rows, enable the <strong><a href="http://documentation.devexpress.com/#WindowsForms/DevExpressXtraGridViewsGridRowStyleEventArgs_HighPrioritytopic"><u>e.HighPriority</u></a></strong> option. <br><br>The <strong>GridCheckMarksSelection </strong>class also provides different ~<strong>Select</strong> methods which allow selecting data and group rows in code. To obtain selected rows, you can use the <strong>SelectedCount</strong> property and <strong>GetSelectedRow</strong> method.</p>

<br/>

>>>>>>> 13.1.4+

<!-- feedback -->
## Does this example address your development requirements/objectives?

[<img src="https://www.devexpress.com/support/examples/i/yes-button.svg"/>](https://www.devexpress.com/support/examples/survey.xml?utm_source=github&utm_campaign=winforms-grid-multiple-row-selection-web-style-checkboxes&~~~was_helpful=yes) [<img src="https://www.devexpress.com/support/examples/i/no-button.svg"/>](https://www.devexpress.com/support/examples/survey.xml?utm_source=github&utm_campaign=winforms-grid-multiple-row-selection-web-style-checkboxes&~~~was_helpful=no)

(you will be redirected to DevExpress.com to submit your response)
<!-- feedback end -->

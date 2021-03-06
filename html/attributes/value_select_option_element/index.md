---
title: 'value (select, option element)'
attributions:
  - 'Microsoft Developer Network: [[Windows Internet Explorer API reference](http://msdn.microsoft.com/en-us/library/ie/hh828809%28v=vs.85%29.aspx) Article]'
compatibility:
  feature: 'value (select, option element)'
  topic: html
notes:
  - 'Review import; Remove MS bias; Update/improve example; Update descriptions; Fix lists & compatibility info'
readiness: 'Not Ready'
tags:
  - Markup_Attributes
  - HTML
  - Needs_Summary
uri: 'html/attributes/value (select, option element)'

---
<table class="wikitable">
<tr>
<th>
Applies to

</th>
<td>
 ?

</td>
</tr>
</table>
## Examples

This example sets the value for each **option** element to a supply stock number.

``` html
<SCRIPT>
<script>
function fnShowText(){
   /* Use the selectedIndex property of the SELECT control
   to retrieve the text from the options collection. */

   var sText = "Stock Number = " + oSel.options(oSel.selectedIndex).value;
   alert(sText);
}
</script>
<SELECT ID="oSel" onchange = "fnShowText()">
<OPTION VALUE="STK#45">Item One - Basketball</OPTION>
<OPTION VALUE="STK#347">Item Two - Baseball</OPTION>
<OPTION VALUE="STK#67">Item Three - Hockey Puck</OPTION>
</SELECT>
</SCRIPT>
```

## Notes

### Remarks

Individual control objects return a value to the server only if they have been selected by the user. You may pass server-friendly data directly to the server without confusing the user. The user sees only the innerText displayed, and not the **value**.

### Syntax

### Standards information

-   [Document Object Model (DOM) Level 1 Specification](http://go.microsoft.com/fwlink/p/?linkid=161725), Section 2.5.5
-   [HTML 4.01 Specification](http://go.microsoft.com/fwlink/p/?linkid=25320), Section 17.6.1

## See also

### Related pages

-   `option`
-   `select`

---
title: 'createRangeCollection'
attributions:
  - 'Microsoft Developer Network: [[Windows Internet Explorer API reference](http://msdn.microsoft.com/en-us/library/ie/hh828809%28v=vs.85%29.aspx) Article]'
notes:
  - "there is no createRangeCollection Method of the HTMLSelection object.\nPlease delete."
readiness: 'Out of Date'
relationships:
  method_of:
    predicate: 'Method of '
    value: dom/Selection
    href: /dom/Selection
  return_type:
    predicate: 'Returns an object of type  '
    value: 'DOM Node'
    href: /dom/Selection
tags:
  - API_Object_Methods
  - DOM
  - Needs_Summary
  - Needs_Examples
uri: dom/Selection/createRangeCollection

---
Method of [dom/Selection](/dom/Selection)[dom/Selection](/dom/Selection)

## Syntax

``` js
var object = object.createRangeCollection();
```

## Return Value

Returns an object of type DOM NodeDOM Node

Object

Returns a collection of [**TextRange**](/dom/TextRange) objects.

## Notes

### Remarks

Host applications can provide a multiple selection mechanism and can return a collection of [**TextRange**](/dom/TextRange) objects that represents discontinuous selections. The host application provides the collection through the **ISegmentList** interface. *MSHTML* requests this interface through the **ISelectionServices** interface. Microsoft Internet Explorer 5.5 does not provide multiple selection. The default implementation of this method returns a collection consisting of a single [**TextRange**](/dom/TextRange) object.

### Syntax

### Standards information

There are no standards that apply here.

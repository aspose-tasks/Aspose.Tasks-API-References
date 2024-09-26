---
title: Enum CurrencySymbolPositionType
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.CurrencySymbolPositionType enum. Specifies the position of a currency symbol
type: docs
weight: 370
url: /net/aspose.tasks/currencysymbolpositiontype/
---
## CurrencySymbolPositionType enumeration

Specifies the position of a currency symbol.

```csharp
public enum CurrencySymbolPositionType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Undefined | `-1` | Indicates undefined value means that the field was not defined in original project file. |
| Before | `0` | Indicates Before currency symbol position type. |
| After | `1` | Indicates After currency symbol position type. |
| BeforeWithSpace | `2` | Indicates BeforeWithSpace currency symbol position type. |
| AfterWithSpace | `3` | Indicates AfterWithSpace currency symbol position type. |

## Remarks

While exporting into XML the Undefined values will be eliminated from resulting XML.

## Examples

Shows how to specify the placement of the currency symbol (CurrencySymbolPositionType.Before).

```csharp
var project = new Project(DataDir + "Project2.mpp");
// set the placement of the currency symbol
// Before, no space ($0).
project.Set(Prj.CurrencySymbolPosition, CurrencySymbolPositionType.Before);
// work with the project...
```

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)



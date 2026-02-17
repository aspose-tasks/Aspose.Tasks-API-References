---
title: Class GlobalizationSettings
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.GlobalizationSettings class. Represents the projects globalization settings
type: docs
weight: 720
url: /net/aspose.tasks/globalizationsettings/
---
## GlobalizationSettings class

Represents the project's globalization settings.

```csharp
public class GlobalizationSettings
```

## Constructors

| Name | Description |
| --- | --- |
| [GlobalizationSettings](globalizationsettings/)() | The default constructor. |

## Properties

| Name | Description |
| --- | --- |
| virtual [FalseLiteral](../../aspose.tasks/globalizationsettings/falseliteral/) { get; } | Gets a string for boolean 'false' literal used in a formula. |
| virtual [FormulaDateNA](../../aspose.tasks/globalizationsettings/formuladatena/) { get; } | Gets "NA" (empty value) literal used in a formula for a date field. |
| virtual [TrueLiteral](../../aspose.tasks/globalizationsettings/trueliteral/) { get; } | Gets a string for boolean 'true' literal used in a formula. |

## Remarks

The recommended way is to use culture-invariant literals or formats throughout the project. However, if a project uses culture-specific literals, this class can be used to help the formula-calculation engine parse those literals.

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)



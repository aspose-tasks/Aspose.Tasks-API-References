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

## Examples

Shows how set project's language-specific settings.

```csharp
var project = new Project();

var attribute = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Number1, "Number");
attribute.Formula = "IIf(ProjDateValue('n.a.')=[Date1];100;200)";

project.ExtendedAttributes.Add(attribute);

var task = project.RootTask.Children.Add("Task");

// Create extended attribute
var extendedAttribute = attribute.CreateExtendedAttribute();
task.ExtendedAttributes.Add(extendedAttribute);

var attributeDate = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Date1, "Date");

task.ExtendedAttributes.Add(attributeDate.CreateExtendedAttribute(DateTime.MinValue));

Console.WriteLine(extendedAttribute.NumericValue);

project.GlobalizationSettings = new MyGlobalizationSettings();

Console.WriteLine(extendedAttribute.NumericValue);
```

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)



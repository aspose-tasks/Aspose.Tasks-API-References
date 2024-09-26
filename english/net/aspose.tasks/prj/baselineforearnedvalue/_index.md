---
title: Prj.BaselineForEarnedValue
second_title: Aspose.Tasks for .NET API Reference
description: Prj field. The specific baseline used to calculate Variance values
type: docs
weight: 80
url: /net/aspose.tasks/prj/baselineforearnedvalue/
---
## Prj.BaselineForEarnedValue field

The specific baseline used to calculate Variance values.

```csharp
public static readonly Key<BaselineType, PrjKey> BaselineForEarnedValue;
```

## Examples

Shows how to read/write Prj.BaselineForEarnedValue property.

```csharp
var project = new Project();

project.Set(Prj.BaselineForEarnedValue, BaselineType.Baseline);

Console.WriteLine("Baseline For Earned Value: " + project.Get(Prj.BaselineForEarnedValue));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [BaselineType](../../baselinetype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)



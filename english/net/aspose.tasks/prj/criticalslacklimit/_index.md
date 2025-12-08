---
title: Prj.CriticalSlackLimit
second_title: Aspose.Tasks for .NET API Reference
description: Prj field. Tasks are considered critical by MS Project if total slack is less or equal to this number of days
type: docs
weight: 140
url: /net/aspose.tasks/prj/criticalslacklimit/
---
## Prj.CriticalSlackLimit field

Tasks are considered critical by MS Project if total slack is less or equal to this number of days.

```csharp
public static readonly Key<int, PrjKey> CriticalSlackLimit;
```

## Examples

Shows how to read/write Prj.CriticalSlackLimit property.

```csharp
var project = new Project();

project.Set(Prj.CriticalSlackLimit, 2);

Console.WriteLine("Critical Slack Limit: " + project.Get(Prj.CriticalSlackLimit));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)



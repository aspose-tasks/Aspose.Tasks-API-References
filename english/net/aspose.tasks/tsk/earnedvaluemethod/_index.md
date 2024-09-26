---
title: Tsk.EarnedValueMethod
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. Determines whether the  Complete or Physical  Complete field should be used to calculate budgeted cost of work performed BCWP
type: docs
weight: 350
url: /net/aspose.tasks/tsk/earnedvaluemethod/
---
## Tsk.EarnedValueMethod field

Determines whether the % Complete or Physical % Complete field should be used to calculate budgeted cost of work performed (BCWP).

```csharp
public static readonly Key<EarnedValueMethodType, TaskKey> EarnedValueMethod;
```

## Examples

Shows how to read/write Tsk.EarnedValueMethod property.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.EarnedValueMethod, EarnedValueMethodType.PercentComplete);

Console.WriteLine("Earned Value Method: " + task.Get(Tsk.EarnedValueMethod));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [EarnedValueMethodType](../../earnedvaluemethodtype/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)



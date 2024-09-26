---
title: FieldHelper.GetDefaultTaskFieldTitle
second_title: Aspose.Tasks for .NET API Reference
description: FieldHelper method. Returns a default title of the specific task field
type: docs
weight: 20
url: /net/aspose.tasks.util/fieldhelper/getdefaulttaskfieldtitle/
---
## FieldHelper.GetDefaultTaskFieldTitle method

Returns a default title of the specific task field.

```csharp
public static string GetDefaultTaskFieldTitle(TaskKey taskKey)
```

| Parameter | Type | Description |
| --- | --- | --- |
| taskKey | TaskKey | Task field to get a default title. |

### Return Value

A default title of the specific task field if the field can be displayed in MS Project's view, null otherwise.

## Examples

Shows how to get default field title for the specific task's field.

```csharp
Console.WriteLine("Title for Tsk.ActualCost: " + FieldHelper.GetDefaultTaskFieldTitle(Tsk.ActualCost.KeyType));
Console.WriteLine("Title for Tsk.PercentWorkComplete: " + FieldHelper.GetDefaultTaskFieldTitle(Tsk.PercentWorkComplete.KeyType));
```

### See Also

* enum [TaskKey](../../../aspose.tasks/taskkey/)
* class [FieldHelper](../)
* namespace [Aspose.Tasks.Util](../../fieldhelper/)
* assembly [Aspose.Tasks](../../../)



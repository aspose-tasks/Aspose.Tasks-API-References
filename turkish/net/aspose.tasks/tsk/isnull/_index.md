---
title: "Tsk.IsNull"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk field. Bir görevin null görev olup olmadığını belirler"
type: docs
weight: 640
url: /tr/net/aspose.tasks/tsk/isnull/
---
## Tsk.IsNull field

Bir görevin boş (null) görev olup olmadığını belirler.

```csharp
public static readonly Key<NullableBool, TaskKey> IsNull;
```

## Örnekler

Tsk.IsNull özelliğini okuma/yazma nasıl gösterir.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsNull, true);

Console.WriteLine("Is Null: " + task.Get(Tsk.IsNull));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)



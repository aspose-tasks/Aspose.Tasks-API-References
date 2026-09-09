---
title: "Prj.NewTasksEstimated"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Prj alanı. Varsayılan olarak tahmini sürenin gösterilip gösterilmeyeceğini belirler"
type: docs
weight: 570
url: /tr/net/aspose.tasks/prj/newtasksestimated/
---
## Prj.NewTasksEstimated field

Tahmini sürenin varsayılan olarak gösterilip gösterilmeyeceğini belirler.

```csharp
public static readonly Key<NullableBool, PrjKey> NewTasksEstimated;
```

## Örnekler

Prj.NewTasksEstimated özelliğini okuma/yazma nasıl yapılacağını gösterir.

```csharp
var project = new Project();

project.Set(Prj.NewTasksEstimated, true);

Console.WriteLine("New Tasks Estimated: " + project.Get(Prj.NewTasksEstimated));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)



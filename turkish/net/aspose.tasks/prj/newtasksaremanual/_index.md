---
title: "Prj.NewTasksAreManual"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Prj alanı. Yeni görevlerin manuel olarak oluşturulup oluşturulmayacağını belirler"
type: docs
weight: 550
url: /tr/net/aspose.tasks/prj/newtasksaremanual/
---
## Prj.NewTasksAreManual field

Yeni görevlerin manuel olarak oluşturulup oluşturulmayacağını belirler.

```csharp
public static readonly Key<NullableBool, PrjKey> NewTasksAreManual;
```

## Örnekler

Prj.NewTasksAreManual özelliğini okuma/yazma yöntemini gösterir.

```csharp
var project = new Project();

project.Set(Prj.NewTasksAreManual, true);

Console.WriteLine("New Tasks Are Manual: " + project.Get(Prj.NewTasksAreManual));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)



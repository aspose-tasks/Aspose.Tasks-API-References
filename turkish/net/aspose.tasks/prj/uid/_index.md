---
title: "Prj.Uid"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Prj alanı. Bir projenin benzersiz kimliği"
type: docs
weight: 760
url: /tr/net/aspose.tasks/prj/uid/
---
## Prj.Uid field

Bir projenin benzersiz kimliği.

```csharp
public static readonly Key<string, PrjKey> Uid;
```

## Örnekler

Prj.Uid özelliğini okuma/yazma nasıl yapılır gösterir.

```csharp
var project = new Project();

project.Set(Prj.Uid, "1234");

Console.WriteLine("Uid: " + project.Get(Prj.Uid));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)



---
title: "Prj.InsertedProjectsLikeSummary"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Prj alanı. Alt görevlerin özet görevler olarak hesaplanıp hesaplanmayacağını belirler"
type: docs
weight: 390
url: /tr/net/aspose.tasks/prj/insertedprojectslikesummary/
---
## Prj.InsertedProjectsLikeSummary field

Alt görevlerin özet görevler olarak hesaplanıp hesaplanmayacağını belirler.

```csharp
public static readonly Key<NullableBool, PrjKey> InsertedProjectsLikeSummary;
```

## Örnekler

Prj.InsertedProjectsLikeSummary özelliğini okuma/yazma nasıl yapılacağını gösterir.

```csharp
var project = new Project();

project.Set(Prj.InsertedProjectsLikeSummary, true);

Console.WriteLine("Inserted Projects Like Summary: " + project.Get(Prj.InsertedProjectsLikeSummary));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)



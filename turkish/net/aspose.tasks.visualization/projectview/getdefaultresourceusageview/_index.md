---
title: "ProjectView.GetDefaultResourceUsageView"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ProjectView yöntemi. Uid, ad, başlangıç, bitiş ve iş kaynak sütunlarını içerir."
type: docs
weight: 50
url: /tr/net/aspose.tasks.visualization/projectview/getdefaultresourceusageview/
---
## ProjectView.GetDefaultResourceUsageView method

Uid, ad, başlangıç, bitiş ve iş kaynağı sütunlarını içerir.

```csharp
public static ProjectView GetDefaultResourceUsageView()
```

### Dönüş Değeri

[`ResourceViewColumn`](../../resourceviewcolumn/) listesini içeren bir görünüm

## Örnekler

Kaynak kullanım görünümüyle bir projenin nasıl kaydedileceğini gösterir.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.Months,
    View = ProjectView.GetDefaultResourceUsageView()
};

project.Save(OutDir + "WorkWithProjectView_ResourceUsageView_out.pdf", options);
```

### Ayrıca Bakınız

* class [ProjectView](../)
* namespace [Aspose.Tasks.Visualization](../../projectview/)
* assembly [Aspose.Tasks](../../../)



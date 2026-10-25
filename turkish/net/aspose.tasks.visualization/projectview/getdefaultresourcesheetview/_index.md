---
title: "ProjectView.GetDefaultResourceSheetView"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ProjectView yöntemi. Uid, kaynak adı, tür, malzeme, etiket, baş harfler, grup, maksimum birimler, standart oran, fazla mesai oranı, kullanım başına maliyet, birikim, temel takvim ve kod kaynak sütunlarını içerir"
type: docs
weight: 40
url: /tr/net/aspose.tasks.visualization/projectview/getdefaultresourcesheetview/
---
## ProjectView.GetDefaultResourceSheetView method

Uid, kaynak adı, tip, malzeme etiketi, baş harfler, grup, maksimum birimler, standart oran, fazla mesai oranı, kullanım başına maliyet, birikim zamanı, temel takvim ve kod kaynak sütunlarını içerir.

```csharp
public static ProjectView GetDefaultResourceSheetView()
```

### Dönüş Değeri

[`ResourceViewColumn`](../../resourceviewcolumn/) listesini içeren bir görünüm

## Örnekler

Kaynak sayfası görünümüyle bir projeyi nasıl kaydedeceğinizi gösterir.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.Months,
    View = ProjectView.GetDefaultResourceSheetView()
};

project.Save(OutDir + "WorkWithProjectView_ResourceSheetView_out.pdf", options);
```

### Ayrıca Bakınız

* class [ProjectView](../)
* namespace [Aspose.Tasks.Visualization](../../projectview/)
* assembly [Aspose.Tasks](../../../)



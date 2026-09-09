---
title: "PageMargins.Left"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "PageMargins özelliği. Sol kenar boşluğunun boyutunu santimetre cinsinden alır veya ayarlar"
type: docs
weight: 40
url: /tr/net/aspose.tasks.visualization/pagemargins/left/
---
## PageMargins.Left property

Sol kenar boşluğunun boyutunu santimetre cinsinden alır veya ayarlar.

```csharp
public double Left { get; set; }
```

## Örnekler

Sayfa kenar boşluklarıyla nasıl çalışılacağını gösterir.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// varsayılan görünümü değiştirelim
var margins = project.DefaultView.PageInfo.Margins;

// kenar boşluklarını değiştirelim
margins.Left = 10d;
margins.Top = 10d;
margins.Right = 10d;
margins.Bottom = 10d;
margins.Borders = Border.OutsidePages;

project.Save(OutDir + "WorkWithPageMargins_out.mpp", SaveFileFormat.Mpp);
```

### Ayrıca Bakınız

* class [PageMargins](../)
* namespace [Aspose.Tasks.Visualization](../../pagemargins/)
* assembly [Aspose.Tasks](../../../)



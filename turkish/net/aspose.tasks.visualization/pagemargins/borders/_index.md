---
title: "PageMargins.Borders"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "PageMargins özelliği. Kenarların basılacağı konumu alır veya ayarlar. Border enum değerlerinden biri olabilir."
type: docs
weight: 20
url: /tr/net/aspose.tasks.visualization/pagemargins/borders/
---
## PageMargins.Borders property

Sınırların çizileceği konumu alır veya ayarlar. [`Border`](../../border/) enumarasyonunun değerlerinden biri olabilir.

```csharp
public Border Borders { get; set; }
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

* enum [Border](../../border/)
* class [PageMargins](../)
* namespace [Aspose.Tasks.Visualization](../../pagemargins/)
* assembly [Aspose.Tasks](../../../)



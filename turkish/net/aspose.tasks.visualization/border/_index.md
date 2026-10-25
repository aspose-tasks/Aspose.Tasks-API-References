---
title: "Enum Border"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Visualization.Border enum. Kenar tiplerini belirtir."
type: docs
weight: 2970
url: /tr/net/aspose.tasks.visualization/border/
---
## Border enumeration

Kenarlık türünü belirtir.

```csharp
public enum Border
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| NoBorder | `0` | Kenar yok. |
| AroundEveryPage | `1` | Her sayfanın etrafında. |
| OutsidePages | `2` | Dış sayfalarda. |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)



---
title: "Enum TextItemType"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Visualization.TextItemType enum. Metin stilini değiştirmek için öğe tipi"
type: docs
weight: 3410
url: /tr/net/aspose.tasks.visualization/textitemtype/
---
## TextItemType enumeration

Bir metin stilini değiştirmek için öğe türü.

```csharp
public enum TextItemType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| RowColumnTitles | `0` | Satır ve sütun başlıkları. |
| CriticalTasks | `1` | Kritik görevler. |
| NoncriticalTasks | `2` | Kritik olmayan görevler. |
| MilestoneTasks | `3` | Kilometre taşı görevleri. |
| InactiveTasks | `4` | Pasif görevler. |
| SummaryTasks | `5` | Özet görevler. |
| AssignmentRow | `6` | Atama satırı. |
| TopTimescaleTier | `7` | Üst zaman ölçeği katmanı. |
| BottomTimescaleTier | `8` | Alt zaman ölçeği katmanı. |
| MiddleTimescaleTier | `9` | Orta zaman ölçeği katmanı. |
| Resources | `10` | Kaynak sayfası. |
| OverallocatedResources | `11` | Aşırı tahsis edilmiş kaynaklar. |
| TaskFilterHighlight | `12` | Görev Filtresi Vurgulama metin öğesi. |
| BarTextBottom | `13` | Çubuk Metni Alt metin öğesi. |
| BarTextInside | `14` | Çubuk Metni İç metin öğesi. |
| BarTextLeft | `15` | Çubuk Metni Sol metin öğesi. |
| BarTextRight | `16` | Çubuk Metni Sağ metin öğesi. |
| BarTextTop | `17` | Çubuk Metni Üst metin öğesi. |
| MarkedTasks | `18` | İşaretlenmiş görev metin öğesi. |
| ProjectSummary | `19` | Proje özeti görev metin öğesi. |
| ExternalTasks | `20` | Harici görevler metin öğesi. |
| Allocated | `21` | Tahsis edilmiş metin öğesi. |
| ChangedCells | `22` | Değiştirilen hücreler. |

## Örnekler

Metin öğesi türleriyle nasıl çalışılacağını gösterir.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
SaveOptions options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.ResourceSheet
};

var style = new TextStyle(FontStyles.Italic | FontStyles.Bold)
{
    Color = Color.OrangeRed
};

style.ItemType = TextItemType.OverallocatedResources;

options.TextStyles = new List<TextStyle>
{
    style
};
project.Save(OutDir + "CustomizeTextStyle_out.pdf", options);
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)



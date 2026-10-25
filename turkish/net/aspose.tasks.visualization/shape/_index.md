---
title: "Enum Şekil"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Visualization.Shape enum. Çubuğun stilinin başında veya sonunda, görünüm verileri kaydedilirken bazı SaveFileFormat'larda işlenecek işaretçinin şekli."
type: docs
weight: 3360
url: /tr/net/aspose.tasks.visualization/shape/
---
## Shape enumeration

Çubuğun stilinin başında veya sonunda, görünüm verileri kaydedilirken bazı [`SaveFileFormat`](../../aspose.tasks.saving/savefileformat/) formatlarında işlenecek işaretçi şekli.

```csharp
public enum Shape
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| None | `0` | None şekli gösterir. |
| VerticalLine | `1` | Dikey çizgi şekli gösterir. |
| Pentagon | `2` | Pentagon şekli gösterir. |
| Triangle | `3` | Üçgen şekli gösterir. |
| LeftBracket | `4` | Sol köşeli parantez şekli gösterir. |
| RightBracket | `5` | Sağ köşeli parantez şekli gösterir. |
| ArrowDown | `6` | Aşağı ok şekli gösterir. |
| LeftFade | `7` | Sol solma şekli gösterir. |
| RightFade | `8` | Sağ solma şekli gösterir. |
| Diamond | `9` | Elmas şekli gösterir. |
| Circle | `10` | Daire şekli gösterir. |

## Örnekler

Özel çubuk stillerinin nasıl kullanılacağını gösterir.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    BarStyles = new List<BarStyle>()
};

// kilometre taşı görevleri için bir çubuk stili ekle
var style = new BarStyle();
// çubuk stilinin <see cref="T:Aspose.Tasks.Visualization.BarItemType" /> ayarla
style.ItemType = BarItemType.Milestone;
// çubuk stilinin <see cref="T:System.Drawing.Color" /> ayarla.
style.BarColor = Color.Green;
// çubuk stilinin <see cref="P:Aspose.Tasks.Visualization.BarStyle.BarShape" /> ayarla
style.BarShape = BarShape.HalfHeight;
// çubuğun başlangıcında <see cref="T:Aspose.Tasks.Visualization.Shape" /> ayarla
style.StartShape = Shape.LeftBracket;
// çubuğun başlangıcında şeklin <see cref="T:System.Drawing.Color" /> ayarla
style.StartShapeColor = Color.Aqua;
// çubuğun sonunda <see cref="T:Aspose.Tasks.Visualization.Shape" /> ayarla
style.EndShape = Shape.RightBracket;
// çubuğun sonunda şeklin <see cref="T:System.Drawing.Color" /> ayarla
style.EndShapeColor = Color.Aquamarine;
// çubuğun sağ tarafında render edilecek metnin ayarı.
style.TextStyle = new TextStyle();
style.TextStyle.BackgroundColor = Color.Black;

// çubuğun metnini dönüştürmeye izin veren bir özellik vardır.
// çubuğun render edilmesi için metni alacak dönüştürücüyü ayarlayalım.
style.LeftBarTextConverter = task =>
{
    if (!task.Get(Tsk.Name).StartsWith("T"))
    {
        task.Set(Tsk.Name, "T" + task.Get(Tsk.Name));
    }

    return task.Get(Tsk.Name);
};

options.BarStyles.Add(style);

// projeyi kaydet
project.Save(OutDir + "WorkWithBarStyle_out.mpp", options);
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)



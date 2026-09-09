---
title: "BarStyle.StartShape"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "BarStyle özelliği. Çubuğun başlangıcındaki Shape'i alır veya ayarlar"
type: docs
weight: 170
url: /tr/net/aspose.tasks.visualization/barstyle/startshape/
---
## BarStyle.StartShape property

Çubuğun başlangıcındaki [`Shape`](../../shape/) alır veya ayarlar.

```csharp
public Shape StartShape { get; set; }
```

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

* enum [Shape](../../shape/)
* class [BarStyle](../)
* namespace [Aspose.Tasks.Visualization](../../barstyle/)
* assembly [Aspose.Tasks](../../../)



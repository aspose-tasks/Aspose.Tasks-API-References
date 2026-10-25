---
title: "Sınıf BarStyle"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Visualization.BarStyle sınıfı. Proje görünümündeki öğenin çubuğunun görsel stilini değiştirir."
type: docs
weight: 2960
url: /tr/net/aspose.tasks.visualization/barstyle/
---
## BarStyle class

Proje görünümündeki öğe için çubuğun görsel stilini değiştir.

```csharp
public class BarStyle
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [BarStyle](barstyle/)() | `BarStyle` sınıfının yeni bir örneğini başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [BarColor](../../aspose.tasks.visualization/barstyle/barcolor/) { get; set; } | Çubuğun stilinin Color özelliğini alır veya ayarlar. |
| [BarShape](../../aspose.tasks.visualization/barstyle/barshape/) { get; set; } | Çubuğun stilinin [`BarShape`](./barshape/) özelliğini alır veya ayarlar. |
| [BottomBarTextConverter](../../aspose.tasks.visualization/barstyle/bottombartextconverter/) { get; set; } | Görevin çubuğunun alt kısmında görüntülenecek metni almak için kullanıcı tanımlı dönüştürücüyü alır veya ayarlar. [`BottomField`](./bottomfield/) özelliğinin değerini geçersiz kılar. |
| [BottomField](../../aspose.tasks.visualization/barstyle/bottomfield/) { get; set; } | Çubuğun alt kısmında görüntülenecek bir alanı alır veya ayarlar. |
| [EndShape](../../aspose.tasks.visualization/barstyle/endshape/) { get; set; } | Çubuğun sonunda [`Shape`](../shape/) özelliğini alır veya ayarlar. |
| [EndShapeColor](../../aspose.tasks.visualization/barstyle/endshapecolor/) { get; set; } | Çubuğun sonunda şeklin Color özelliğini alır veya ayarlar. |
| [EndShapeType](../../aspose.tasks.visualization/barstyle/endshapetype/) { get; set; } | Son şeklin tipini alır veya ayarlar. [`GanttBarType`](../ganttbartype/). |
| [From](../../aspose.tasks.visualization/barstyle/from/) { get; set; } | Gantt çubuğunun başlangıç noktası konumunu alır veya ayarlar. [`Field`](../../aspose.tasks/field/). |
| [InsideBarTextConverter](../../aspose.tasks.visualization/barstyle/insidebartextconverter/) { get; set; } | Görevin çubuğunun içinde görüntülenecek metni almak için kullanıcı tanımlı dönüştürücüyü alır veya ayarlar. [`InsideField`](./insidefield/) özelliğinin değerini geçersiz kılar. |
| [InsideField](../../aspose.tasks.visualization/barstyle/insidefield/) { get; set; } | Çubuğun içinde görüntülenecek bir alanı alır veya ayarlar. |
| [ItemType](../../aspose.tasks.visualization/barstyle/itemtype/) { get; set; } | Çubuğun stilinin [`BarItemType`](../baritemtype/) özelliğini alır veya ayarlar. |
| [LeftBarTextConverter](../../aspose.tasks.visualization/barstyle/leftbartextconverter/) { get; set; } | Görev çubuğunun sol tarafında render edilecek metni almak için kullanıcı tanımlı dönüştürücüyü alır veya ayarlar. [`LeftField`](./leftfield/) özelliğinin değerini geçersiz kılar. |
| [LeftField](../../aspose.tasks.visualization/barstyle/leftfield/) { get; set; } | Çubuğun sol tarafında görüntülenecek bir alanı alır veya ayarlar. |
| [RightBarTextConverter](../../aspose.tasks.visualization/barstyle/rightbartextconverter/) { get; set; } | Görevin çubuğunun sağ tarafında görüntülenecek metni almak için kullanıcı tanımlı dönüştürücüyü alır veya ayarlar. [`RightField`](./rightfield/) özelliğinin değerini geçersiz kılar. |
| [RightField](../../aspose.tasks.visualization/barstyle/rightfield/) { get; set; } | Çubuğun sağında görüntülenecek bir alanı alır veya ayarlar. |
| [StartShape](../../aspose.tasks.visualization/barstyle/startshape/) { get; set; } | Çubuğun başında [`Shape`](../shape/) alır veya ayarlar. |
| [StartShapeColor](../../aspose.tasks.visualization/barstyle/startshapecolor/) { get; set; } | Çubuğun başındaki şeklin Rengini alır veya ayarlar. |
| [StartShapeType](../../aspose.tasks.visualization/barstyle/startshapetype/) { get; set; } | Başlangıç şeklinin tipini alır veya ayarlar. |
| [TextStyle](../../aspose.tasks.visualization/barstyle/textstyle/) { get; set; } | Çubuğun metninin stilini alır veya ayarlar. |
| [To](../../aspose.tasks.visualization/barstyle/to/) { get; set; } | Gantt çubuğunun bitiş noktası konumunu alır veya ayarlar. |
| [TopBarTextConverter](../../aspose.tasks.visualization/barstyle/topbartextconverter/) { get; set; } | Görev çubuğunun üst kısmında render edilecek metni almak için kullanıcı tanımlı dönüştürücüyü alır veya ayarlar. [`TopField`](./topfield/) özelliğinin değerini geçersiz kılar. |
| [TopField](../../aspose.tasks.visualization/barstyle/topfield/) { get; set; } | Çubuğun üstünde görüntülenecek bir alanı alır veya ayarlar. |

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



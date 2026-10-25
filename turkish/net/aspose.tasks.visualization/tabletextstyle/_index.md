---
title: "Sınıf TableTextStyle"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Visualization.TableTextStyle sınıfı. Görünüm tablosunda bir metin stilini temsil eder."
type: docs
weight: 3370
url: /tr/net/aspose.tasks.visualization/tabletextstyle/
---
## TableTextStyle class

Bir görünüm tablosundaki metin stilini temsil eder.

```csharp
public class TableTextStyle : TextStyle
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [TableTextStyle](tabletextstyle/#constructor)(int) | `TableTextStyle` sınıfının yeni bir örneğini başlatır. |
| [TableTextStyle](tabletextstyle/#constructor_1)(int, FontDescriptor) | `TableTextStyle` sınıfının belirtilen yazı tipiyle yeni bir örneğini başlatır. |
| [TableTextStyle](tabletextstyle/#constructor_2)(int, FontStyles) | `TableTextStyle` sınıfının varsayılan yazı tipi ayarları ve belirtilen yazı tipi stiliyle yeni bir örneğini başlatır. |
| [TableTextStyle](tabletextstyle/#constructor_3)(int, float, FontStyles) | `TableTextStyle` sınıfının belirtilen yazı tipi boyutu ve yazı tipi stiliyle yeni bir örneğini başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [BackgroundColor](../../aspose.tasks.visualization/textstyle/backgroundcolor/) { get; set; } | Metin stilinin arka plan rengini alır veya ayarlar. [`Color`](../textstyle/color/). |
| [BackgroundPattern](../../aspose.tasks.visualization/textstyle/backgroundpattern/) { get; set; } | Metin stilinin arka plan desenini alır veya ayarlar. [`BackgroundPattern`](../textstyle/backgroundpattern/). |
| [Color](../../aspose.tasks.visualization/textstyle/color/) { get; set; } | Metnin rengini alır veya ayarlar. |
| [Field](../../aspose.tasks.visualization/tabletextstyle/field/) { get; set; } | Stilin uygulanacağı bir alanı alır veya ayarlar. [`Field`](./field/). |
| [Font](../../aspose.tasks.visualization/textstyle/font/) { get; set; } | Metin stilinin yazı tipini alır veya ayarlar. |
| override [ItemType](../../aspose.tasks.visualization/tabletextstyle/itemtype/) { get; } | [`TextItemType`](../textitemtype/) enum değerini döndürür. |
| [RowUid](../../aspose.tasks.visualization/tabletextstyle/rowuid/) { get; } | Bir satırın benzersiz kimliğini alır. Stil bir görünümdeki tüm satırlara uygulanacaksa -1 döndürür. |

## Örnekler

Bir projedeki farklı metin öğelerini biçimlendirmek için kullanılan tablo metin stillerinin nasıl özelleştirileceğini gösterir.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.NewTasksAreManual, false);

var view = (GanttChartView)project.Views.ToList()[0];

// ilk görev adı metin stilini ayarla
var style1 = new TableTextStyle(1);
// stilin uygulanacağı bir alan ayarla.
style1.Field = Field.TaskName;
// metin stilinin <see cref="P:Aspose.Tasks.Visualization.TextStyle.Font" /> ayarla.
style1.Font = new FontDescriptor("Impact", 12F, FontStyles.Bold | FontStyles.Italic);
// metin stili yazı tipinin punto cinsinden boyutunu ayarla.

// ikinci görev süresi metin stilini ayarla
var style2 = new TableTextStyle(2);
style2.Field = Field.TaskDurationText;
style2.Font = new FontDescriptor("Impact", 16F, FontStyles.Underline);

view.TableTextStyles.Add(style1);
view.TableTextStyles.Add(style2);

SimpleSaveOptions options = new MPPSaveOptions
{
    // görünüm verisinin yazılması gerektiğini gösteren bir bayrak ayarla
    WriteViewData = true
};
project.Save(OutDir + "WorkWithTableTextStyle_out.mpp", options);
```

### Ayrıca Bakınız

* class [TextStyle](../textstyle/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)



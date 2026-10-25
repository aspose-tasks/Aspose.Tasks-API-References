---
title: "Sınıf TextStyle"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Visualization.TextStyle sınıfı. Proje görünümündeki bir öğe için metnin görsel stilini değiştirin."
type: docs
weight: 3420
url: /tr/net/aspose.tasks.visualization/textstyle/
---
## TextStyle class

Proje görünümündeki bir öğe için metnin görsel stilini değiştir.

```csharp
public class TextStyle
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [TextStyle](textstyle/#constructor)() | `TextStyle` sınıfının yeni bir örneğini varsayılan ayarlarla başlatır. |
| [TextStyle](textstyle/#constructor_1)(FontDescriptor) | `TextStyle` sınıfının yeni bir örneğini belirtilen yazı tipi ayarlarıyla başlatır. |
| [TextStyle](textstyle/#constructor_2)(FontStyles) | `TextStyle` sınıfının yeni bir örneğini varsayılan yazı tipi ve belirtilen yazı tipi stiliyle başlatır. |
| [TextStyle](textstyle/#constructor_3)(float, FontStyles) | `TextStyle` sınıfının yeni bir örneğini varsayılan yazı tipi ve belirtilen yazı tipi boyutu ve stiliyle başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [BackgroundColor](../../aspose.tasks.visualization/textstyle/backgroundcolor/) { get; set; } | Metin stilinin arka plan rengini alır veya ayarlar. [`Color`](./color/). |
| [BackgroundPattern](../../aspose.tasks.visualization/textstyle/backgroundpattern/) { get; set; } | Metin stilinin arka plan desenini alır veya ayarlar. [`BackgroundPattern`](./backgroundpattern/). |
| [Color](../../aspose.tasks.visualization/textstyle/color/) { get; set; } | Metnin rengini alır veya ayarlar. |
| [Font](../../aspose.tasks.visualization/textstyle/font/) { get; set; } | Metin stilinin yazı tipini alır veya ayarlar. |
| virtual [ItemType](../../aspose.tasks.visualization/textstyle/itemtype/) { get; set; } | Metin stilinin [`TextItemType`](../textitemtype/) değerini alır veya ayarlar. |

## Örnekler

Bir projedeki farklı metin öğelerini biçimlendirmek için kullanılan metin stillerinin nasıl özelleştirileceğini gösterir.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
SaveOptions options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.ResourceSheet
};

var style = new TextStyle();
style.Color = Color.OrangeRed;
style.Font = new FontDescriptor(FontFamily.GenericMonospace.Name, 10F, FontStyles.Bold | FontStyles.Italic);
style.ItemType = TextItemType.OverallocatedResources;
style.BackgroundColor = Color.Aqua;
style.BackgroundPattern = BackgroundPattern.DarkDither;

options.TextStyles = new List<TextStyle>
{
    style
};
project.Save(OutDir + "CustomizeTextStyle_out.pdf", options);
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)



---
title: "Enum BackgroundPattern"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.BackgroundPattern enum. Arka plan desenini belirtir"
type: docs
weight: 100
url: /tr/net/aspose.tasks/backgroundpattern/
---
## BackgroundPattern enumeration

Arka plan desenini belirtir.

```csharp
public enum BackgroundPattern
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| DarkDiagonalLeft | `7` | Koyu sol çapraz arka plan desenini gösterir. |
| DarkDiagonalRight | `8` | Koyu sağ çapraz arka plan desenini gösterir. |
| DarkDither | `13` | Koyu benekli arka plan desenini gösterir. |
| DarkFill | `4` | Koyu doldurulmuş arka plan desenini gösterir. |
| DiagonalLeft | `5` | Sol çapraz arka plan desenini gösterir. |
| DiagonalRight | `6` | Sağ çapraz arka plan desenini gösterir. |
| Hollow | `0` | Boş arka plan desenini gösterir. |
| LightDither | `11` | Açık titreme arka plan desenini gösterir. |
| LightFill | `2` | Açık dolgu arka plan desenini gösterir. |
| MediumDither | `12` | Orta titreme arka plan desenini gösterir. |
| MediumFill | `3` | Orta dolgu arka plan desenini gösterir. |
| MediumVerticalStripe | `10` | Orta dikey şerit arka plan desenini gösterir. |
| SolidFill | `1` | Katı dolgu arka plan desenini gösterir. |
| ThinVerticalStripe | `9` | İnce dikey şerit arka plan desenini gösterir. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)



---
title: "TextStyle.TextStyle"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "TextStyle yapıcı. TextStyle sınıfının yeni bir örneğini varsayılan ayarlarla başlatır"
type: docs
weight: 10
url: /tr/net/aspose.tasks.visualization/textstyle/textstyle/
---
## TextStyle() {#constructor}

Yeni bir örnek oluşturur [`TextStyle`](../) sınıfını varsayılan ayarlarla.

```csharp
public TextStyle()
```

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

* class [TextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../textstyle/)
* assembly [Aspose.Tasks](../../../)

---

## TextStyle(float, FontStyles) {#constructor_3}

Yeni bir örnek oluşturur [`TextStyle`](../) sınıfını varsayılan yazı tipi ve belirtilen yazı tipi boyutu ve stiliyle.

```csharp
public TextStyle(float fontSize, FontStyles fontStyle)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fontSize | Single | TextStyle yazı tipinin boyutu. |
| fontStyle | FontStyles | TextStyle yazı tipinin stili. |

### Ayrıca Bakınız

* enum [FontStyles](../../fontstyles/)
* class [TextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../textstyle/)
* assembly [Aspose.Tasks](../../../)

---

## TextStyle(FontStyles) {#constructor_2}

Yeni bir örnek oluşturur [`TextStyle`](../) sınıfını varsayılan yazı tipi ve belirtilen yazı tipi stiliyle.

```csharp
public TextStyle(FontStyles fontStyle)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fontStyle | FontStyles | Varsayılan yazı tipine uygulanacak yazı tipi stili. |

### Ayrıca Bakınız

* enum [FontStyles](../../fontstyles/)
* class [TextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../textstyle/)
* assembly [Aspose.Tasks](../../../)

---

## TextStyle(FontDescriptor) {#constructor_1}

Yeni bir örnek oluşturur [`TextStyle`](../) sınıfını belirtilen yazı tipi ayarlarıyla.

```csharp
public TextStyle(FontDescriptor font)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| font | FontDescriptor | TextStyle yazı tipi. |

### Ayrıca Bakınız

* class [FontDescriptor](../../fontdescriptor/)
* class [TextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../textstyle/)
* assembly [Aspose.Tasks](../../../)



---
title: TextStyle.TextStyle
second_title: Aspose.Tasks for .NET API Reference
description: TextStyle constructor. Initializes a new instance of the TextStyle class with default settings
type: docs
weight: 10
url: /net/aspose.tasks.visualization/textstyle/textstyle/
---
## TextStyle() {#constructor}

Initializes a new instance of the [`TextStyle`](../) class with default settings.

```csharp
public TextStyle()
```

## Examples

Shows how to customize text styles which are used to style different text items in a project.

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

### See Also

* class [TextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../textstyle/)
* assembly [Aspose.Tasks](../../../)

---

## TextStyle(float, FontStyles) {#constructor_3}

Initializes a new instance of the [`TextStyle`](../) class with the default font and specified font size and style.

```csharp
public TextStyle(float fontSize, FontStyles fontStyle)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fontSize | Single | Size of font of TextStyle. |
| fontStyle | FontStyles | Style of font of TextStyle. |

### See Also

* enum [FontStyles](../../fontstyles/)
* class [TextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../textstyle/)
* assembly [Aspose.Tasks](../../../)

---

## TextStyle(FontStyles) {#constructor_2}

Initializes a new instance of the [`TextStyle`](../) class with the default font and specified font style.

```csharp
public TextStyle(FontStyles fontStyle)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fontStyle | FontStyles | Style of font to apply to default font. |

### See Also

* enum [FontStyles](../../fontstyles/)
* class [TextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../textstyle/)
* assembly [Aspose.Tasks](../../../)

---

## TextStyle(FontDescriptor) {#constructor_1}

Initializes a new instance of the [`TextStyle`](../) class with the specified font settings.

```csharp
public TextStyle(FontDescriptor font)
```

| Parameter | Type | Description |
| --- | --- | --- |
| font | FontDescriptor | Font of the TextStyle. |

### See Also

* class [FontDescriptor](../../fontdescriptor/)
* class [TextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../textstyle/)
* assembly [Aspose.Tasks](../../../)



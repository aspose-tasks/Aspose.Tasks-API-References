---
title: "TextStyle.TextStyle"
second_title: "Aspose.Tasks for .NET API 参考"
description: "TextStyle 构造函数。使用默认设置初始化 TextStyle 类的新实例"
type: docs
weight: 10
url: /zh/net/aspose.tasks.visualization/textstyle/textstyle/
---
## TextStyle() {#constructor}

使用默认设置初始化 [`TextStyle`](../) 类的新实例。

```csharp
public TextStyle()
```

## 示例

展示如何自定义文本样式，这些样式用于为项目中的不同文本项设置样式。

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

### 另见

* class [TextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../textstyle/)
* assembly [Aspose.Tasks](../../../)

---

## TextStyle(float, FontStyles) {#constructor_3}

使用默认字体以及指定的字体大小和样式初始化 [`TextStyle`](../) 类的新实例。

```csharp
public TextStyle(float fontSize, FontStyles fontStyle)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fontSize | Single | TextStyle 的字体大小。 |
| fontStyle | FontStyles | TextStyle 的字体样式。 |

### 另见

* enum [FontStyles](../../fontstyles/)
* class [TextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../textstyle/)
* assembly [Aspose.Tasks](../../../)

---

## TextStyle(FontStyles) {#constructor_2}

使用默认字体和指定的字体样式初始化 [`TextStyle`](../) 类的新实例。

```csharp
public TextStyle(FontStyles fontStyle)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fontStyle | FontStyles | 要应用于默认字体的字体样式。 |

### 另见

* enum [FontStyles](../../fontstyles/)
* class [TextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../textstyle/)
* assembly [Aspose.Tasks](../../../)

---

## TextStyle(FontDescriptor) {#constructor_1}

使用指定的字体设置初始化 [`TextStyle`](../) 类的新实例。

```csharp
public TextStyle(FontDescriptor font)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| font | FontDescriptor | TextStyle 的字体。 |

### 另见

* class [FontDescriptor](../../fontdescriptor/)
* class [TextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../textstyle/)
* assembly [Aspose.Tasks](../../../)



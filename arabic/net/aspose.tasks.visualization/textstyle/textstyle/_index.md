---
title: "TextStyle.TextStyle"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "منشئ TextStyle. يهيئ نسخة جديدة من فئة TextStyle بالإعدادات الافتراضية"
type: docs
weight: 10
url: /ar/net/aspose.tasks.visualization/textstyle/textstyle/
---
## TextStyle() {#constructor}

يهيئ نسخة جديدة من الفئة [`TextStyle`](../) بالإعدادات الافتراضية.

```csharp
public TextStyle()
```

## الأمثلة

يوضح كيفية تخصيص أنماط النص التي تُستخدم لتنسيق عناصر النص المختلفة في المشروع.

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

### انظر أيضًا

* class [TextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../textstyle/)
* assembly [Aspose.Tasks](../../../)

---

## TextStyle(float, FontStyles) {#constructor_3}

يهيئ نسخة جديدة من الفئة [`TextStyle`](../) بالخط الافتراضي وحجم الخط المحدد والنمط المحدد.

```csharp
public TextStyle(float fontSize, FontStyles fontStyle)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| fontSize | Single | حجم الخط لنمط TextStyle. |
| fontStyle | FontStyles | نمط الخط لنمط TextStyle. |

### انظر أيضًا

* enum [FontStyles](../../fontstyles/)
* class [TextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../textstyle/)
* assembly [Aspose.Tasks](../../../)

---

## TextStyle(FontStyles) {#constructor_2}

يهيئ نسخة جديدة من الفئة [`TextStyle`](../) بالخط الافتراضي والنمط المحدد للخط.

```csharp
public TextStyle(FontStyles fontStyle)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| fontStyle | FontStyles | نمط الخط لتطبيقه على الخط الافتراضي. |

### انظر أيضًا

* enum [FontStyles](../../fontstyles/)
* class [TextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../textstyle/)
* assembly [Aspose.Tasks](../../../)

---

## TextStyle(FontDescriptor) {#constructor_1}

يهيئ نسخة جديدة من الفئة [`TextStyle`](../) بالإعدادات المحددة للخط.

```csharp
public TextStyle(FontDescriptor font)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| font | FontDescriptor | خط TextStyle. |

### انظر أيضًا

* class [FontDescriptor](../../fontdescriptor/)
* class [TextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../textstyle/)
* assembly [Aspose.Tasks](../../../)



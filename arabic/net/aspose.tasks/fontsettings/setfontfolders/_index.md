---
title: "FontSettings.SetFontFolders"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة FontSettings. تحدد المجلدات التي يبحث فيها Aspose.Tasks عن خطوط TrueType عند عرض المشاريع."
type: docs
weight: 50
url: /ar/net/aspose.tasks/fontsettings/setfontfolders/
---
## FontSettings.SetFontFolders method

يضبط المجلدات التي يبحث فيها Aspose.Tasks عن خطوط TrueType عند تصيير عرض المشروع.

```csharp
public void SetFontFolders(string[] fontFolders, bool recursive)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| fontFolders | String[] | مصفوفة من المجلدات التي تحتوي على خطوط TrueType. |
| recursive | Boolean | إذا كان true، سيتم فحص المجلدات المحددة بشكل متكرر. |

## الأمثلة

يوضح كيفية تعيين مجلد خطوط مخصص.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.GanttChart,
};

// يجب أن تكون ملفات خطوط TrueType لجميع الخطوط المستخدمة في المشروع المفتوح موجودة في مجلد MyFonts.
options.FontSettings.SetFontFolders(new string[] { "c:\\MyFonts"}, true);

project.Save(OutDir + "EstimatedMilestoneTasks_out4.pdf", options);
```

### انظر أيضًا

* class [FontSettings](../)
* namespace [Aspose.Tasks](../../fontsettings/)
* assembly [Aspose.Tasks](../../../)



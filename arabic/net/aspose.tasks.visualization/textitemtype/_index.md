---
title: "التعداد TextItemType"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "التعداد Aspose.Tasks.Visualization.TextItemType. نوع العنصر لتغيير نمط النص."
type: docs
weight: 3410
url: /ar/net/aspose.tasks.visualization/textitemtype/
---
## TextItemType enumeration

نوع العنصر لتغيير نمط النص لـ.

```csharp
public enum TextItemType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| RowColumnTitles | `0` | عناوين الصفوف والأعمدة. |
| CriticalTasks | `1` | المهام الحرجة. |
| NoncriticalTasks | `2` | مهام غير حرجة. |
| MilestoneTasks | `3` | مهام معلم. |
| InactiveTasks | `4` | مهام غير نشطة. |
| SummaryTasks | `5` | مهام ملخص. |
| AssignmentRow | `6` | صف التعيين. |
| TopTimescaleTier | `7` | الطبقة العليا لمقياس الزمن. |
| BottomTimescaleTier | `8` | الطبقة السفلى لمقياس الزمن. |
| MiddleTimescaleTier | `9` | الطبقة المتوسطة لمقياس الزمن. |
| Resources | `10` | ورقة الموارد. |
| OverallocatedResources | `11` | موارد مخصصة بشكل مفرط. |
| TaskFilterHighlight | `12` | عنصر نص تمييز مرشح المهمة. |
| BarTextBottom | `13` | عنصر نص أسفل الشريط. |
| BarTextInside | `14` | عنصر نص داخل الشريط. |
| BarTextLeft | `15` | عنصر نص يسار الشريط. |
| BarTextRight | `16` | عنصر نص يمين الشريط. |
| BarTextTop | `17` | عنصر نص أعلى الشريط. |
| MarkedTasks | `18` | عنصر نص المهمة المعلَّمة. |
| ProjectSummary | `19` | عنصر نص مهمة ملخص المشروع. |
| ExternalTasks | `20` | عنصر نص المهام الخارجية. |
| Allocated | `21` | عنصر نص مخصص. |
| ChangedCells | `22` | الخلايا التي تم تغييرها. |

## الأمثلة

يظهر كيفية العمل مع أنواع عناصر النص.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
SaveOptions options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.ResourceSheet
};

var style = new TextStyle(FontStyles.Italic | FontStyles.Bold)
{
    Color = Color.OrangeRed
};

style.ItemType = TextItemType.OverallocatedResources;

options.TextStyles = new List<TextStyle>
{
    style
};
project.Save(OutDir + "CustomizeTextStyle_out.pdf", options);
```

### انظر أيضًا

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)



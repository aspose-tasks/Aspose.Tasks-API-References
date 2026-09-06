---
title: "تعداد GridlineType"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "تعداد Aspose.Tasks.Visualization.GridlineType. نوع خط الشبكة"
type: docs
weight: 3110
url: /ar/net/aspose.tasks.visualization/gridlinetype/
---
## GridlineType enumeration

نوع خط الشبكة.

```csharp
public enum GridlineType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| GanttRow | `0` | يشير إلى خط شبكة من نوع صف مخطط جانت. |
| TopTierColumn | `1` | يشير إلى خط شبكة من نوع عمود المستوى الأعلى. |
| BottomTierColumn | `2` | يشير إلى خط شبكة من نوع عمود المستوى السفلي. |
| SheetRow | `3` | يشير إلى خط شبكة من نوع صف ورقة. |
| SheetColumn | `4` | يشير إلى خط شبكة من نوع عمود ورقة. |
| UsageRow | `5` | يشير إلى خط شبكة من نوع صف الاستخدام. |
| UsageColumn | `6` | يشير إلى خط شبكة من نوع عمود الاستخدام. |
| GanttTitleVertical | `7` | يشير إلى نوع خط شبكة عمودي لعنوان مخطط جانت. |
| GanttTitleHorizontal | `8` | يشير إلى نوع خط شبكة أفقي لعنوان مخطط جانت. |
| BarRows | `9` | يشير إلى نوع خط شبكة لصفوف الأشرطة. |
| GanttProjectStart | `10` | يشير إلى نوع خط شبكة لبداية مشروع مخطط جانت. |
| GanttProjectFinish | `11` | يشير إلى نوع خط شبكة لنهاية مشروع مخطط جانت. |
| GanttStatusDate | `12` | يشير إلى نوع خط شبكة تاريخ الحالة في مخطط جانت. |
| GanttCurrentDate | `13` | يشير إلى نوع خط شبكة تاريخ اليوم الحالي في مخطط جانت. |
| GanttPageBreaks | `14` | يشير إلى نوع خط شبكة فواصل الصفحات في مخطط جانت. |
| MiddleTierColumn | `15` | يشير إلى نوع خط شبكة العمود من المستوى الأوسط. |

## الأمثلة

يوضح كيفية العمل مع خطوط الشبكة أثناء الحفظ بصيغ بصرية.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
var options = new ImageSaveOptions(SaveFileFormat.Png);

var gridline = new Gridline
{
    // تعيين نوع خط الشبكة (<see cref=\"P:Aspose.Tasks.Visualization.Gridline.GridlineType\" />).
    GridlineType = GridlineType.GanttRow, 
    // تعيين <see cref=\"T:Aspose.Tasks.Visualization.LinePattern\" /> لخط الشبكة
    Pattern = LinePattern.Dashed
};

options.Gridlines = new List<Gridline>();
options.Gridlines.Add(gridline);

project.Save(OutDir + "PrintProjectPagesToSeparateFiles_out.png", options);
```

### انظر أيضًا

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)



---
title: "الفئة ViewCollection"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.ViewCollection. تحتوي على قائمة من كائنات View. تنفذ واجهة ICollectionView"
type: docs
weight: 2900
url: /ar/net/aspose.tasks/viewcollection/
---
## ViewCollection class

تحتوي على قائمة من كائنات [`View`](../view/) . تنفذ واجهة ICollection&lt;View&gt;.

```csharp
public class ViewCollection : ICollection<View>
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Count](../../aspose.tasks/viewcollection/count/) { get; } | يحصل على عدد العناصر الموجودة في هذه المجموعة. |
| [IsReadOnly](../../aspose.tasks/viewcollection/isreadonly/) { get; } | يحصل على قيمة تشير إلى ما إذا كانت هذه المجموعة للقراءة فقط؛ وإلا، false. |
| [ParentProject](../../aspose.tasks/viewcollection/parentproject/) { get; } | يحصل على الأصل لكائن View. للقراءة فقط [`Project`](../project/). |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Add](../../aspose.tasks/viewcollection/add/)(View) | يضيف العنصر المحدد إلى هذه المجموعة. |
| [Clear](../../aspose.tasks/viewcollection/clear/)() | يزيل جميع العناصر من هذه المجموعة. |
| [Contains](../../aspose.tasks/viewcollection/contains/)(View) | يرجع true إذا تم العثور على العنصر المحدد في هذه المجموعة؛ وإلا، false. |
| [CopyTo](../../aspose.tasks/viewcollection/copyto/)(View[], int) | ينسخ عناصر هذه المجموعة إلى المصفوفة المحددة، بدءًا من الفهرس المحدد للمصفوفة. |
| [GetByName](../../aspose.tasks/viewcollection/getbyname/)(string) | يبحث عن View بالاسم، ويعيد أول ظهور داخل المجموعة. |
| [GetByViewScreen](../../aspose.tasks/viewcollection/getbyviewscreen/)(ViewScreen) | يبحث عن View بالخاصية Screen المحددة، ويعيد أول ظهور داخل المجموعة. |
| [GetEnumerator](../../aspose.tasks/viewcollection/getenumerator/)() | يرجع عدادًا لهذه المجموعة. |
| [Remove](../../aspose.tasks/viewcollection/remove/)(View) | يزيل الظهور الأول لكائن محدد من هذه المجموعة. |
| [ToList](../../aspose.tasks/viewcollection/tolist/)() | يحول مجموعة العرض إلى قائمة من كائنات [`View`](../view/). |

## الأمثلة

يظهر كيفية العمل مع مجموعات العرض.

```csharp
var project = new Project(DataDir + "Project1.mpp");

// تحويل إلى قائمة بسيطة من العروض
List<View> list = project.Views.ToList();
for (var index = 0; index < list.Count; index++)
{
    var viewToChange = list[index];
    viewToChange.PageInfo.Header.CenteredText = "Header " + index;
}

// إضافة عرض جديد
var view = new GanttChartView();
if (!project.Views.IsReadOnly)
{
    project.Views.Add(view);
}

// التكرار عبر العروض
Console.WriteLine("Iterate over views of " + project.Views.ParentProject.Get(Prj.Name) + " project.");
Console.WriteLine("Project view count: " + project.Views.Count);
Console.WriteLine();
foreach (var projectView in project.Views)
{
    Console.WriteLine("Name: " + projectView.Name);
}

// إزالة جميع العروض مرة واحدة
project.Views.Clear();

// أو واحدًا تلو الآخر
{
    // النهج 1
    List<View> listToDelete = project.Views.ToList();
    foreach (var v in listToDelete)
    {
        if (project.Views.Contains(v))
        {
            project.Views.Remove(v);
        }
    }
}

{
    // النهج 2
    var array = new View[project.Views.Count];
    project.Views.CopyTo(array, 0);
    foreach (var v in array)
    {
        if (project.Views.Contains(v))
        {
            project.Views.Remove(v);
        }
    }
}
```

### انظر أيضًا

* class [View](../view/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)



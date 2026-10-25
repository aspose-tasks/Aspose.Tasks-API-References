---
title: "ViewCollection.Add"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة ViewCollection. تضيف العنصر المحدد إلى هذه المجموعة"
type: docs
weight: 40
url: /ar/net/aspose.tasks/viewcollection/add/
---
## ViewCollection.Add method

يضيف العنصر المحدد إلى هذه المجموعة.

```csharp
public void Add(View item)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| العنصر | View | العنصر المحدد لإضافته إلى هذه المجموعة. |

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

* class [View](../../view/)
* class [ViewCollection](../)
* namespace [Aspose.Tasks](../../viewcollection/)
* assembly [Aspose.Tasks](../../../)



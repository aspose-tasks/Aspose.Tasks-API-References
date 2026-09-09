---
title: "ViewCollection.CopyTo"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ViewCollection yöntemi. Bu koleksiyonun öğelerini belirtilen diziye, belirtilen dizi indeksinden başlayarak kopyalar"
type: docs
weight: 70
url: /tr/net/aspose.tasks/viewcollection/copyto/
---
## ViewCollection.CopyTo method

Bu koleksiyonun öğelerini belirtilen diziye, belirtilen dizi indeksinden başlayarak kopyalar.

```csharp
public void CopyTo(View[] array, int arrayIndex)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizi | View[] | Elemanların kopyalanacağı belirtilen tek boyutlu dizi. |
| arrayIndex | Int32 | Kopyalamanın başlayacağı belirtilen dizinin sıfır tabanlı indeksi. |

## Örnekler

View koleksiyonlarıyla nasıl çalışılacağını gösterir.

```csharp
var project = new Project(DataDir + "Project1.mpp");

// view'ların düz bir listesine dönüştür
List<View> list = project.Views.ToList();
for (var index = 0; index < list.Count; index++)
{
    var viewToChange = list[index];
    viewToChange.PageInfo.Header.CenteredText = "Header " + index;
}

// yeni bir view ekle
var view = new GanttChartView();
if (!project.Views.IsReadOnly)
{
    project.Views.Add(view);
}

// view'lar üzerinde yinele
Console.WriteLine("Iterate over views of " + project.Views.ParentProject.Get(Prj.Name) + " project.");
Console.WriteLine("Project view count: " + project.Views.Count);
Console.WriteLine();
foreach (var projectView in project.Views)
{
    Console.WriteLine("Name: " + projectView.Name);
}

// tüm view'ları bir anda kaldır
project.Views.Clear();

// veya tek tek
{
    // yaklaşım 1
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
    // yaklaşım 2
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

### Ayrıca Bakınız

* class [View](../../view/)
* class [ViewCollection](../)
* namespace [Aspose.Tasks](../../viewcollection/)
* assembly [Aspose.Tasks](../../../)



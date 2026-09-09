---
title: "Sınıf ViewCollection"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.ViewCollection sınıfı. View nesnelerinin bir listesini içerir. ICollectionView arayüzünü uygular"
type: docs
weight: 2900
url: /tr/net/aspose.tasks/viewcollection/
---
## ViewCollection class

[`View`](../view/) nesnelerinin bir listesini içerir. ICollection&lt;View&gt; arayüzünü uygular.

```csharp
public class ViewCollection : ICollection<View>
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Count](../../aspose.tasks/viewcollection/count/) { get; } | Bu koleksiyonda bulunan öğe sayısını alır. |
| [IsReadOnly](../../aspose.tasks/viewcollection/isreadonly/) { get; } | Bu koleksiyonun yalnızca okunur olup olmadığını gösteren bir değer alır; aksi takdirde false. |
| [ParentProject](../../aspose.tasks/viewcollection/parentproject/) { get; } | View nesnesinin üst nesnesini alır. Salt okunur [`Project`](../project/). |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Add](../../aspose.tasks/viewcollection/add/)(View) | Belirtilen öğeyi bu koleksiyona ekler. |
| [Clear](../../aspose.tasks/viewcollection/clear/)() | Bu koleksiyondaki tüm öğeleri kaldırır. |
| [Contains](../../aspose.tasks/viewcollection/contains/)(View) | Belirtilen öğe bu koleksiyonda bulunursa true, aksi takdirde false döndürür. |
| [CopyTo](../../aspose.tasks/viewcollection/copyto/)(View[], int) | Bu koleksiyonun öğelerini belirtilen diziye, belirtilen dizi indeksinden başlayarak kopyalar. |
| [GetByName](../../aspose.tasks/viewcollection/getbyname/)(string) | İsimle bir View arar ve koleksiyon içinde ilk oluşumunu döndürür. |
| [GetByViewScreen](../../aspose.tasks/viewcollection/getbyviewscreen/)(ViewScreen) | Belirtilen Screen özelliğine sahip bir View arar ve koleksiyon içinde ilk oluşumunu döndürür. |
| [GetEnumerator](../../aspose.tasks/viewcollection/getenumerator/)() | Bu koleksiyon için bir enumerator döndürür. |
| [Remove](../../aspose.tasks/viewcollection/remove/)(View) | Bu koleksiyondan belirli bir nesnenin ilk oluşumunu kaldırır. |
| [ToList](../../aspose.tasks/viewcollection/tolist/)() | Bir view koleksiyonunu [`View`](../view/) nesnelerinin listesine dönüştürür. |

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

* class [View](../view/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)



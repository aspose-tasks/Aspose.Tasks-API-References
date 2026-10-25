---
title: "ViewCollection.ToList"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode ViewCollection. Mengonversi koleksi view menjadi daftar objek View"
type: docs
weight: 120
url: /id/net/aspose.tasks/viewcollection/tolist/
---
## ViewCollection.ToList method

Mengonversi koleksi view menjadi daftar objek [`View`](../../view/).

```csharp
public List<View> ToList()
```

### Nilai Kembali

Daftar generik objek [`View`](../../view/).

## Contoh

Menampilkan cara bekerja dengan koleksi view.

```csharp
var project = new Project(DataDir + "Project1.mpp");

// konversi menjadi daftar view biasa
List<View> list = project.Views.ToList();
for (var index = 0; index < list.Count; index++)
{
    var viewToChange = list[index];
    viewToChange.PageInfo.Header.CenteredText = "Header " + index;
}

// tambahkan view baru
var view = new GanttChartView();
if (!project.Views.IsReadOnly)
{
    project.Views.Add(view);
}

// iterasi atas view
Console.WriteLine("Iterate over views of " + project.Views.ParentProject.Get(Prj.Name) + " project.");
Console.WriteLine("Project view count: " + project.Views.Count);
Console.WriteLine();
foreach (var projectView in project.Views)
{
    Console.WriteLine("Name: " + projectView.Name);
}

// hapus semua view sekaligus
project.Views.Clear();

// atau satu per satu
{
    // pendekatan 1
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
    // pendekatan 2
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

### Lihat Juga

* class [View](../../view/)
* class [ViewCollection](../)
* namespace [Aspose.Tasks](../../viewcollection/)
* assembly [Aspose.Tasks](../../../)



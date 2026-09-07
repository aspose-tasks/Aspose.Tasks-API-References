---
title: "Kelas ViewCollection"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.ViewCollection. Berisi daftar objek View. Mengimplementasikan antarmuka ICollectionView"
type: docs
weight: 2900
url: /id/net/aspose.tasks/viewcollection/
---
## ViewCollection class

Berisi daftar objek [`View`](../view/). Mengimplementasikan antarmuka ICollection&lt;View&gt;.

```csharp
public class ViewCollection : ICollection<View>
```

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Count](../../aspose.tasks/viewcollection/count/) { get; } | Mendapatkan jumlah elemen yang terdapat dalam koleksi ini. |
| [IsReadOnly](../../aspose.tasks/viewcollection/isreadonly/) { get; } | Mendapatkan nilai yang menunjukkan apakah koleksi ini hanya-baca; jika tidak, false. |
| [ParentProject](../../aspose.tasks/viewcollection/parentproject/) { get; } | Mendapatkan induk dari objek View. Hanya-baca [`Project`](../project/). |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [Add](../../aspose.tasks/viewcollection/add/)(View) | Menambahkan item yang ditentukan ke koleksi ini. |
| [Clear](../../aspose.tasks/viewcollection/clear/)() | Menghapus semua item dari koleksi ini. |
| [Contains](../../aspose.tasks/viewcollection/contains/)(View) | Mengembalikan true jika item yang ditentukan ditemukan dalam koleksi ini; jika tidak, false. |
| [CopyTo](../../aspose.tasks/viewcollection/copyto/)(View[], int) | Menyalin elemen-elemen koleksi ini ke array yang ditentukan, mulai dari indeks array yang ditentukan. |
| [GetByName](../../aspose.tasks/viewcollection/getbyname/)(string) | Mencari View dengan nama tersebut, dan mengembalikan kemunculan pertama dalam koleksi. |
| [GetByViewScreen](../../aspose.tasks/viewcollection/getbyviewscreen/)(ViewScreen) | Mencari View dengan properti Screen yang ditentukan, dan mengembalikan kemunculan pertama dalam koleksi. |
| [GetEnumerator](../../aspose.tasks/viewcollection/getenumerator/)() | Mengembalikan enumerator untuk koleksi ini. |
| [Remove](../../aspose.tasks/viewcollection/remove/)(View) | Menghapus kemunculan pertama dari objek tertentu dari koleksi ini. |
| [ToList](../../aspose.tasks/viewcollection/tolist/)() | Mengonversi koleksi view menjadi daftar objek [`View`](../view/). |

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

* class [View](../view/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)



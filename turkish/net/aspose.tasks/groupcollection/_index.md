---
title: "Sınıf GroupCollection"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.GroupCollection sınıfı. Group nesnelerinin bir listesini içerir. ICollectionGroup arayüzünü uygular."
type: docs
weight: 780
url: /tr/net/aspose.tasks/groupcollection/
---
## GroupCollection class

[`Group`](../group/) nesnelerinin bir listesini içerir. ICollection&lt;Group&gt; arayüzünü uygular.

```csharp
public class GroupCollection : ICollection<Group>
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Count](../../aspose.tasks/groupcollection/count/) { get; } | Bu koleksiyonda bulunan öğe sayısını alır. |
| [IsReadOnly](../../aspose.tasks/groupcollection/isreadonly/) { get; } | Bu koleksiyonun yalnızca okunur olup olmadığını gösteren bir değeri alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Add](../../aspose.tasks/groupcollection/add/)(Group) | Belirtilen öğeyi bu koleksiyona ekler. |
| [Clear](../../aspose.tasks/groupcollection/clear/)() | Bu koleksiyondaki tüm öğeleri kaldırır. |
| [Contains](../../aspose.tasks/groupcollection/contains/)(Group) | Belirtilen öğe bu koleksiyonda bulunursa true, aksi takdirde false döndürür. |
| [CopyTo](../../aspose.tasks/groupcollection/copyto/)(Group[], int) | Bu koleksiyonun öğelerini belirtilen diziye, belirtilen dizi indeksinden başlayarak kopyalar. |
| [GetEnumerator](../../aspose.tasks/groupcollection/getenumerator/)() | Bu koleksiyon için bir enumerator döndürür. |
| [Remove](../../aspose.tasks/groupcollection/remove/)(Group) | Bu koleksiyondan belirli bir nesnenin ilk oluşumunu kaldırır. |
| [ToList](../../aspose.tasks/groupcollection/tolist/)() | Bir grup koleksiyonunu [`Group`](../group/) nesnelerinin bir listesine dönüştürür. |

## Örnekler

Grupların koleksiyonuyla nasıl çalışılacağını gösterir.

```csharp
var project = new Project(DataDir + "ReadGroupDefinitionData.mpp");

// görev grupları üzerinde yinele
Console.WriteLine("Print task groups of {0} project: ", project.Get(Prj.Name));
Console.WriteLine("Task Group Count: " + project.TaskGroups.Count);
foreach (var group in project.TaskGroups)
{
    Console.WriteLine("Name: " + group.Name);
    Console.WriteLine("Show In Menu: " + group.ShowInMenu);
    Console.WriteLine();
}

// kaynak grupları üzerinde yinele
Console.WriteLine("Project resource group count: " + project.ResourceGroups.Count);
foreach (var group in project.ResourceGroups)
{
    Console.WriteLine("Resource group Name: " + group.Name);
    Console.WriteLine("Resource group ShowInMenu" + group.ShowInMenu);
}

var otherProject = new Project(DataDir + "Blank2010.mpp");

// diğer projenin gruplarını temizle
otherProject.TaskGroups.Clear();

// grupları diğer projeye kopyala
var groups = new Group[project.TaskGroups.Count];
project.TaskGroups.CopyTo(groups, 0);

foreach (var group in groups)
{
    otherProject.TaskGroups.Add(group);
}

// özel görev grubu ekle
var customGroup = new Group
{
    Name = "Custom Group",
    ShowInMenu = true
};

if (!otherProject.TaskGroups.Contains(customGroup))
{
    if (!otherProject.TaskGroups.IsReadOnly)
    {
        otherProject.TaskGroups.Add(customGroup);
    }
}

// tüm grupları kaldır
List<Group> groupsToDelete = otherProject.TaskGroups.ToList();
foreach (var group in groupsToDelete)
{
    otherProject.TaskGroups.Remove(group);
}
```

### Ayrıca Bakınız

* class [Group](../group/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)



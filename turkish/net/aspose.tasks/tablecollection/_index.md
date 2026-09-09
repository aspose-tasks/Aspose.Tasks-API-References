---
title: "Sınıf TableCollection"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.TableCollection sınıfı. Table nesnelerinin bir listesini içerir. ICollectionTable arayüzünü uygular"
type: docs
weight: 2330
url: /tr/net/aspose.tasks/tablecollection/
---
## TableCollection class

[`Table`](../table/) nesnelerinin bir listesini içerir. ICollection&lt;Table&gt; arayüzünü uygular.

```csharp
public class TableCollection : ICollection<Table>
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Count](../../aspose.tasks/tablecollection/count/) { get; } | Bu koleksiyonda bulunan öğe sayısını alır. |
| [IsReadOnly](../../aspose.tasks/tablecollection/isreadonly/) { get; } | Bu koleksiyonun yalnızca okunur olup olmadığını gösteren bir değer alır; aksi takdirde false. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Add](../../aspose.tasks/tablecollection/add/)(Table) | Belirtilen öğeyi bu koleksiyona ekler. |
| [Clear](../../aspose.tasks/tablecollection/clear/)() | Bu koleksiyondaki tüm öğeleri kaldırır. |
| [Contains](../../aspose.tasks/tablecollection/contains/)(Table) | Belirtilen öğe bu koleksiyonda bulunursa true, aksi takdirde false döndürür. |
| [CopyTo](../../aspose.tasks/tablecollection/copyto/)(Table[], int) | Bu koleksiyonun öğelerini belirtilen diziye, belirtilen dizi indeksinden başlayarak kopyalar. |
| [GetEnumerator](../../aspose.tasks/tablecollection/getenumerator/)() | Bu koleksiyon için bir enumerator döndürür. |
| [Remove](../../aspose.tasks/tablecollection/remove/)(Table) | Bu koleksiyondan belirli bir nesnenin ilk oluşumunu kaldırır. |
| [ToList](../../aspose.tasks/tablecollection/tolist/)() | Bir tablo koleksiyonunu [`Table`](../table/) nesnelerinin bir listesine dönüştürür. |

## Örnekler

Tablo koleksiyonlarıyla nasıl çalışılacağını gösterir.

```csharp
var project = new Project(DataDir + "Project1.mpp");

Console.WriteLine("Is collection of tables read-only?: " + project.Tables.IsReadOnly);

// tablolar üzerinde yineleme yap
Console.WriteLine("Print tables of " + project.Get(Prj.Name) + " project.");
Console.WriteLine("Table count: " + project.Tables.Count);
foreach (var tbl in project.Tables)
{
    Console.WriteLine("Name: " + tbl.Name);

    Console.WriteLine("Fields:");

    foreach (var field in tbl.TableFields)
    {
        Console.WriteLine("    {0} - '{1}' - {2}", field.Field, field.Title, field.Width);
    }
}

// yeni bir tablo ekle
var tableToAdd = new Table
{
    Name = "New Table",
    ShowInMenu = true
};
project.Tables.Add(tableToAdd);

Console.WriteLine("The collection contains the new table?: " + project.Tables.Contains(tableToAdd));

// koleksiyonu iki şekilde temizleyebilirsiniz
if (deleteOneByOne)
{
    // tabloları diziye kopyalayın ve tek tek silin
    var tables = new Table[project.Tables.Count];
    project.Tables.CopyTo(tables, 0);
    foreach (var table in tables)
    {
        project.Tables.Remove(table);
    }
}
else
{
    // ya da bir tablo koleksiyonunu tamamen temizleyebilirsiniz
    project.Tables.Clear();
}

// koleksiyon, basit bir tablo listesine dönüştürülebilir
List<Table> list = project.Tables.ToList();
foreach (var table in list)
{
    Console.WriteLine("Name: " + table.Name);
}
```

### Ayrıca Bakınız

* class [Table](../table/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)



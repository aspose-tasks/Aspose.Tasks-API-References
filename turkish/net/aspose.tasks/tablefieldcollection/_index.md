---
title: "Sınıf TableFieldCollection"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.TableFieldCollection sınıfı. TableField nesnelerinin bir listesini içerir. IListTableField arayüzünü uygular"
type: docs
weight: 2350
url: /tr/net/aspose.tasks/tablefieldcollection/
---
## TableFieldCollection class

Bir liste [`TableField`](../tablefield/) nesnesi içerir. IList&lt;TableField&gt; arayüzünü uygular.

```csharp
public class TableFieldCollection : IList<TableField>
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Count](../../aspose.tasks/tablefieldcollection/count/) { get; } | Bu koleksiyonda bulunan öğe sayısını alır. |
| [IsReadOnly](../../aspose.tasks/tablefieldcollection/isreadonly/) { get; } | Bu koleksiyonun yalnızca okunur olup olmadığını gösteren bir değer alır; aksi takdirde false. |
| [Item](../../aspose.tasks/tablefieldcollection/item/) { get; set; } | Belirtilen indeksteki öğeyi döndürür veya ayarlar. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Add](../../aspose.tasks/tablefieldcollection/add/)(TableField) | Belirtilen öğeyi bu koleksiyona ekler. |
| [Clear](../../aspose.tasks/tablefieldcollection/clear/)() | Bu koleksiyondaki tüm öğeleri kaldırır. |
| [Contains](../../aspose.tasks/tablefieldcollection/contains/)(TableField) | Belirtilen öğe bu koleksiyonda bulunursa true, aksi takdirde false döndürür. |
| [CopyTo](../../aspose.tasks/tablefieldcollection/copyto/)(TableField[], int) | Bu koleksiyonun öğelerini belirtilen diziye, belirtilen dizi indeksinden başlayarak kopyalar. |
| [GetEnumerator](../../aspose.tasks/tablefieldcollection/getenumerator/)() | Bu koleksiyon için bir enumerator döndürür. |
| [IndexOf](../../aspose.tasks/tablefieldcollection/indexof/)(TableField) | Bu koleksiyondaki belirtilen öğenin dizinini belirler. |
| [Insert](../../aspose.tasks/tablefieldcollection/insert/)(int, TableField) | Belirtilen öğeyi belirtilen dizine ekler. |
| [Remove](../../aspose.tasks/tablefieldcollection/remove/)(TableField) | Bu koleksiyondan belirli bir nesnenin ilk oluşumunu kaldırır. |
| [RemoveAt](../../aspose.tasks/tablefieldcollection/removeat/)(int) | Belirtilen dizindeki bir öğeyi kaldırır. |

## Örnekler

Tablo alanı koleksiyonlarıyla nasıl çalışılacağını gösterir.

```csharp
var project = new Project(DataDir + "Project1.mpp");

foreach (var tbl in project.Tables)
{
    Console.WriteLine("Table name: " + tbl.Name);
    Console.WriteLine("Is collection of table fields read-only?: " + tbl.TableFields.IsReadOnly);

    // tablo alanları üzerinde yineleme yap
    Console.WriteLine("Print table fields of " + project.Get(Prj.Name) + " project.");
    Console.WriteLine("Table count: " + tbl.TableFields.Count);
    foreach (var fld in tbl.TableFields)
    {
        Console.WriteLine("Field Title: " + fld.Title);
        Console.WriteLine("Field Field: " + fld.Field);
        Console.WriteLine();
    }
}

// yeni bir tablo alanı ekle
var table = project.Tables.ToList()[0];
var field = new TableField();
field.Title = "New Table Field";
table.TableFields.Add(field);

var field2 = new TableField();
field2.Title = "New Table Field 2";

// yeni bir alanı belirtilen konuma ekle
var idx = table.TableFields.IndexOf(field);
table.TableFields.Insert(idx, field2);

// indeks erişimi kullanarak yeni tablo alanını düzenleyelim
table.TableFields[idx].WrapHeader = true;

Console.WriteLine("The collection contains the new table field?: " + table.TableFields.Contains(field));

// son zamanlarda alanı kaldırabiliriz
table.TableFields.RemoveAt(idx);

// koleksiyonu iki şekilde temizleyebilirsiniz
if (deleteOneByOne)
{
    // tablo alanlarını diziye kopyala ve tek tek sil
    var tableFields = new TableField[table.TableFields.Count];
    table.TableFields.CopyTo(tableFields, 0);
    foreach (var fld in tableFields)
    {
        table.TableFields.Remove(fld);
    }
}
else
{
    // ya da bir tablo alanı koleksiyonunu tamamen temizleyebilir
    table.TableFields.Clear();
}
```

### Ayrıca Bakınız

* class [TableField](../tablefield/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)



---
title: "TableFieldCollection.Count"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "TableFieldCollection özelliği. Bu koleksiyonda bulunan öğelerin sayısını alır"
type: docs
weight: 10
url: /tr/net/aspose.tasks/tablefieldcollection/count/
---
## TableFieldCollection.Count property

Bu koleksiyonda bulunan öğe sayısını alır.

```csharp
public int Count { get; }
```

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

* class [TableFieldCollection](../)
* namespace [Aspose.Tasks](../../tablefieldcollection/)
* assembly [Aspose.Tasks](../../../)



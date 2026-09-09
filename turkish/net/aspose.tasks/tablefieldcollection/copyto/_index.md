---
title: "TableFieldCollection.CopyTo"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "TableFieldCollection yöntemi. Bu koleksiyonun öğelerini belirtilen diziye, belirtilen dizi indeksinden başlayarak kopyalar"
type: docs
weight: 70
url: /tr/net/aspose.tasks/tablefieldcollection/copyto/
---
## TableFieldCollection.CopyTo method

Bu koleksiyonun öğelerini belirtilen diziye, belirtilen dizi indeksinden başlayarak kopyalar.

```csharp
public void CopyTo(TableField[] array, int arrayIndex)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizi | TableField[] | Elemanların kopyalanacağı belirtilen tek boyutlu dizi. |
| arrayIndex | Int32 | Kopyalamanın başlayacağı belirtilen dizinin sıfır tabanlı indeksi. |

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

* class [TableField](../../tablefield/)
* class [TableFieldCollection](../)
* namespace [Aspose.Tasks](../../tablefieldcollection/)
* assembly [Aspose.Tasks](../../../)



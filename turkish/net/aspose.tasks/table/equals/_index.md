---
title: "Table.Equals"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Table yöntemi. Bu örneğin belirtilen bir nesneye eşit olup olmadığını gösteren bir değer döndürür"
type: docs
weight: 120
url: /tr/net/aspose.tasks/table/equals/
---
## Table.Equals method

Bu örneğin belirtilen nesneye eşit olup olmadığını gösteren bir değer döndürür.

```csharp
public override bool Equals(object obj)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| obj | Object | Bu örnekle karşılaştırılacak nesne. |

### Dönüş Değeri

**True** if the specified object is a Table that has the same UID value as this instance; otherwise, **false**.

## Örnekler

Tablo eşitliğini nasıl kontrol edeceğinizi gösterir.

```csharp
var project = new Project(DataDir + "ReadFilterDefinitionData.mpp");
List<Table> tables = project.Tables.ToList();

var table1 = tables[0];
var table2 = tables[1];

// Tabloların eşitliği, tablonun UID'sine karşı kontrol edilir.
Console.WriteLine("Table 1 UID: " + table1.Uid);
Console.WriteLine("Table 2 UID: " + table2.Uid);
Console.WriteLine("Are tables equal: " + table1.Equals(table2));
```

### Ayrıca Bakınız

* class [Table](../)
* namespace [Aspose.Tasks](../../table/)
* assembly [Aspose.Tasks](../../../)



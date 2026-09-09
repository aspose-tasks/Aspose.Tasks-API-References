---
title: "Table.GetHashCode"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Table yöntemi. Bu Table için bir karma kod (hash code) döndürür"
type: docs
weight: 130
url: /tr/net/aspose.tasks/table/gethashcode/
---
## Table.GetHashCode method

Bu Tablo için bir karma kodu döndürür.

```csharp
public override int GetHashCode()
```

### Dönüş Değeri

Bu nesne için bir karma kod değeri döndürür.

## Örnekler

Bir tablonun karma kodunu nasıl alacağınızı gösterir.

```csharp
var project = new Project(DataDir + "ReadFilterDefinitionData.mpp");

List<Table> tables = project.Tables.ToList();

var table1 = tables[0];
var table2 = tables[1];

// Bir tablonun karma kodu, tablo UID'sine eşittir.
Console.WriteLine("Table UID: {0} Hash Code: {1}", table1.Uid, table1.GetHashCode());
Console.WriteLine("Table UID: {0} Hash Code: {1}", table2.Uid, table2.GetHashCode());
```

### Ayrıca Bakınız

* class [Table](../)
* namespace [Aspose.Tasks](../../table/)
* assembly [Aspose.Tasks](../../../)



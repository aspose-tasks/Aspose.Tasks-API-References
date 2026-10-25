---
title: "Table.GetHashCode"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Table method. Возвращает хеш‑код для этой Table"
type: docs
weight: 130
url: /ru/net/aspose.tasks/table/gethashcode/
---
## Table.GetHashCode method

Возвращает хеш-код для этой таблицы.

```csharp
public override int GetHashCode()
```

### Возвращаемое значение

Возвращает значение хэш‑кода для этого объекта.

## Примеры

Показывает, как получить хеш‑код таблицы.

```csharp
var project = new Project(DataDir + "ReadFilterDefinitionData.mpp");

List<Table> tables = project.Tables.ToList();

var table1 = tables[0];
var table2 = tables[1];

// хеш‑код таблицы равен UID таблицы
Console.WriteLine("Table UID: {0} Hash Code: {1}", table1.Uid, table1.GetHashCode());
Console.WriteLine("Table UID: {0} Hash Code: {1}", table2.Uid, table2.GetHashCode());
```

### См. также

* class [Table](../)
* namespace [Aspose.Tasks](../../table/)
* assembly [Aspose.Tasks](../../../)



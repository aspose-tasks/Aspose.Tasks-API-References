---
title: "Table.Equals"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Table method. Возвращает значение, указывающее, равен ли данный экземпляр указанному объекту"
type: docs
weight: 120
url: /ru/net/aspose.tasks/table/equals/
---
## Table.Equals method

Возвращает значение, указывающее, равен ли этот экземпляр указанному объекту.

```csharp
public override bool Equals(object obj)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| obj | Объект | Объект для сравнения с этим экземпляром. |

### Возвращаемое значение

**True** if the specified object is a Table that has the same UID value as this instance; otherwise, **false**.

## Примеры

Показывает, как проверить равенство таблиц.

```csharp
var project = new Project(DataDir + "ReadFilterDefinitionData.mpp");
List<Table> tables = project.Tables.ToList();

var table1 = tables[0];
var table2 = tables[1];

// равенство таблиц проверяется по UID таблицы.
Console.WriteLine("Table 1 UID: " + table1.Uid);
Console.WriteLine("Table 2 UID: " + table2.Uid);
Console.WriteLine("Are tables equal: " + table1.Equals(table2));
```

### См. также

* class [Table](../)
* namespace [Aspose.Tasks](../../table/)
* assembly [Aspose.Tasks](../../../)



---
title: "Gridline.Equals"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод Gridline. Возвращает флаг, указывающий, равен ли этот экземпляр указанному объекту."
type: docs
weight: 50
url: /ru/net/aspose.tasks.visualization/gridline/equals/
---
## Gridline.Equals method

Возвращает флаг, указывающий, равен ли этот экземпляр указанному объекту.

```csharp
public override bool Equals(object obj)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| obj | Объект | указанный объект для сравнения с этим экземпляром. |

### Возвращаемое значение

флаг, указывающий, равен ли этот экземпляр указанному объекту.

## Примеры

Показывает, как проверить равенство сеточных линий.

```csharp
var gridline1 = new Gridline();
var gridline2 = new Gridline();

// Равенство сеточных линий проверяется по типу сеточной линии.
Console.WriteLine("Gridline 1 Type: " + gridline1.GridlineType);
Console.WriteLine("Gridline 2 Type: " + gridline2.GridlineType);
Console.WriteLine("Are gridlines equal: " + gridline1.Equals(gridline2));

// изменить тип
gridline1.GridlineType = GridlineType.BarRows;
Console.WriteLine("Gridline 1 Type: " + gridline1.GridlineType);
Console.WriteLine("Are gridlines equal: " + gridline1.Equals(gridline2));
```

### См. также

* class [Gridline](../)
* namespace [Aspose.Tasks.Visualization](../../gridline/)
* assembly [Aspose.Tasks](../../../)



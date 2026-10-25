---
title: "NullableBool.GetHashCode"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод NullableBool. Возвращает значение хэш‑кода для экземпляра класса NullableBool"
type: docs
weight: 50
url: /ru/net/aspose.tasks/nullablebool/gethashcode/
---
## NullableBool.GetHashCode method

Возвращает значение хэш‑кода для экземпляра класса [`NullableBool`](../).

```csharp
public override int GetHashCode()
```

### Возвращаемое значение

возвращает значение хеш‑кода для этого объекта.

## Примеры

Показывает, как работать с методом &lt;see cref="Aspose.Tasks.NullableBool" /&gt;.GetHashCode.

```csharp
var bool1 = new NullableBool(true);
var bool2 = new NullableBool(true, false);

// Хеш‑код булевых значений основан на свойствах 'IsDefined' и 'Value'
Console.WriteLine("Bool 1: {0} Hash Code 1: {1}", bool1.ToString(), bool1.GetHashCode());
Console.WriteLine("Bool 2: {0} Hash Code 1: {1}", bool2.ToString(), bool2.GetHashCode());
```

### См. также

* struct [NullableBool](../)
* namespace [Aspose.Tasks](../../nullablebool/)
* assembly [Aspose.Tasks](../../../)



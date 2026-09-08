---
title: "NullableBool.op_Inequality"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод NullableBool. Возвращает значение, указывающее, не равен ли данный экземпляр указанному объекту"
type: docs
weight: 90
url: /ru/net/aspose.tasks/nullablebool/op_inequality/
---
## NullableBool Inequality operator

Возвращает значение, указывающее, не равен ли этот экземпляр указанному объекту.

```csharp
public static bool operator !=(NullableBool a, NullableBool b)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| a | NullableBool | Первый [`NullableBool`](../). |
| b | NullableBool | Второй [`NullableBool`](../). |

### Возвращаемое значение

значение, указывающее, не равен ли этот экземпляр указанному объекту

## Примеры

Показывает, как сравнивать экземпляры &lt;see cref=\"Aspose.Tasks.NullableBool\" /&gt;.

```csharp
var bool1 = new NullableBool(true);
var bool2 = new NullableBool(true, false);

// равенство булевых значений проверяется по свойствам 'IsDefined' и 'Value'.
Console.WriteLine("Nullable Bool 1: " + bool1.ToString());
Console.WriteLine("Nullable Bool 2: " + bool2.ToString());

// проверяет неявное преобразование в bool: bool1 равно True, потому что он определён и Value установлено в True.
if (bool1)
{
    Console.WriteLine("Nullable Bool 1 is True");
}
else
{
    Console.WriteLine("Nullable Bool 1 is False");
}

// проверяет неявное преобразование в bool: bool2 равно False, потому что он не определён.
if (bool2)
{
    Console.WriteLine("Nullable Bool 2 is True");
}
else
{
    Console.WriteLine("Nullable Bool 2 is False");
}

Console.WriteLine("Are bools equal: " + bool1.Equals(bool2));

// проверяет неявное преобразование в bool
if (bool2)
{
    Console.WriteLine("Nullable Bool 2 is True");
}
else
{
    Console.WriteLine("Nullable Bool 2 is False");
}
```

### См. также

* struct [NullableBool](../)
* namespace [Aspose.Tasks](../../nullablebool/)
* assembly [Aspose.Tasks](../../../)



---
title: "NullableBool.op_Implicit"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод NullableBool. Неявно преобразует экземпляр NullableBool в логическое значение. Возвращает true, когда Value равно true и IsDefined равно true"
type: docs
weight: 80
url: /ru/net/aspose.tasks/nullablebool/op_implicit/
---
## implicit operator {#op_implicit_1}

Неявно преобразует экземпляр [`NullableBool`](../) в логическое значение. Возвращает true, когда [`Value`](../value/) равно true и [`IsDefined`](../isdefined/) равно true.

```csharp
public static implicit operator bool(NullableBool val)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | NullableBool | Значение для преобразования. |

### Возвращаемое значение

логическое значение.

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

---

## implicit operator {#op_implicit}

Неявно преобразует логическое значение в экземпляр [`NullableBool`](../).

```csharp
public static implicit operator NullableBool(bool val)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | Boolean | Значение для преобразования. |

### Возвращаемое значение

Преобразованный экземпляр [`NullableBool`](../).

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



---
title: "NullableBool.Equals"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод NullableBool. Возвращает флаг, указывающий, равен ли данный экземпляр указанному экземпляру класса NullableBool"
type: docs
weight: 40
url: /ru/net/aspose.tasks/nullablebool/equals/
---
## Equals(NullableBool) {#equals}

Возвращает флаг, указывающий, равен ли данный экземпляр указанному экземпляру класса [`NullableBool`](../).

```csharp
public bool Equals(NullableBool other)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| другой | NullableBool | указанный объект для сравнения с этим экземпляром. |

### Возвращаемое значение

флаг, указывающий, равен ли данный экземпляр указанному экземпляру класса [`NullableBool`](../).

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

## Equals(object) {#equals_1}

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



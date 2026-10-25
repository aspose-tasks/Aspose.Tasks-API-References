---
title: "VbaReference.Equals"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод VbaReference. Возвращает значение, указывающее, равен ли данный экземпляр указанному объекту VbaReference"
type: docs
weight: 40
url: /ru/net/aspose.tasks/vbareference/equals/
---
## Equals(VbaReference) {#equals}

Возвращает значение, указывающее, равен ли данный экземпляр указанному объекту [`VbaReference`](../).

```csharp
public bool Equals(VbaReference other)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| other | VbaReference | Указанный объект [`VbaReference`](../) для сравнения с этим экземпляром. |

### Возвращаемое значение

Возвращает true, если данный экземпляр равен указанному объекту [`VbaReference`](../); в противном случае — false.

## Примеры

Показывает, как проверить равенство VBA‑ссылок.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

var reference1 = project.VbaProject.References.ToList()[0];
var reference2 = project.VbaProject.References.ToList()[1];

// Равенство ссылок проверяется по имени ссылки.
Console.WriteLine("VBA reference 1 Name: " + reference1.Name);
Console.WriteLine("VBA reference 2 Name: " + reference2.Name);
Console.WriteLine("Are references equal: " + reference1.Equals(reference2));
```

### См. также

* class [VbaReference](../)
* namespace [Aspose.Tasks](../../vbareference/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

Возвращает значение, указывающее, равен ли данный экземпляр указанному объекту [`VbaReference`](../).

```csharp
public override bool Equals(object obj)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| obj | Object | Указанный объект [`VbaReference`](../) для сравнения с этим экземпляром. |

### Возвращаемое значение

Возвращает true, если данный экземпляр равен указанному объекту [`VbaReference`](../); в противном случае — false.

## Примеры

Показывает, как проверить равенство VBA‑ссылок.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

var reference1 = project.VbaProject.References.ToList()[0];
var reference2 = project.VbaProject.References.ToList()[1];

// Равенство ссылок проверяется по имени ссылки.
Console.WriteLine("VBA reference 1 Name: " + reference1.Name);
Console.WriteLine("VBA reference 2 Name: " + reference2.Name);
Console.WriteLine("Are references equal: " + reference1.Equals(reference2));
```

### См. также

* class [VbaReference](../)
* namespace [Aspose.Tasks](../../vbareference/)
* assembly [Aspose.Tasks](../../../)



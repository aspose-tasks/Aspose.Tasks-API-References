---
title: "Resource.Equals"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод Resource. Возвращает значение, указывающее, равен ли данный экземпляр указанному экземпляру класса Resource."
type: docs
weight: 820
url: /ru/net/aspose.tasks/resource/equals/
---
## Equals(Resource) {#equals}

Возвращает значение, указывающее, равен ли данный экземпляр указанному экземпляру класса [`Resource`](../).

```csharp
public bool Equals(Resource other)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| other | Resource | Указанный экземпляр класса [`Resource`](../), с которым сравнивается данный экземпляр. |

### Возвращаемое значение

**True** if the specified instance of the [`Resource`](../) class has the same Uid value as this instance; otherwise, **false**.

## Примеры

Показывает, как проверить равенство ресурсов.

```csharp
var project = new Project(DataDir + "Baselines2010.mpp");

var resource1 = project.Resources.GetById(1);
var resource2 = project.Resources.GetById(1);

Console.WriteLine("Are resources equal: " + resource1.Equals(resource2));
```

### См. также

* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

Возвращает значение, указывающее, равен ли этот экземпляр указанному объекту.

```csharp
public override bool Equals(object obj)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| obj | Объект | Объект для сравнения с этим экземпляром. |

### Возвращаемое значение

**True** if the specified object is a Resource that has the same Uid value as this instance; otherwise, **false**.

## Примеры

Показывает, как проверить равенство ресурсов.

```csharp
var project = new Project(DataDir + "Baselines2010.mpp");

var resource1 = project.Resources.GetById(1);
var resource2 = project.Resources.GetById(1);

Console.WriteLine("Are resources equal: " + resource1.Equals(resource2));
```

### См. также

* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)



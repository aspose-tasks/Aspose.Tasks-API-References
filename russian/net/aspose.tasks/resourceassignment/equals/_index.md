---
title: "ResourceAssignment.Equals"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод ResourceAssignment. Возвращает значение, указывающее, равен ли данный экземпляр указанному экземпляру класса ResourceAssignment."
type: docs
weight: 690
url: /ru/net/aspose.tasks/resourceassignment/equals/
---
## Equals(ResourceAssignment) {#equals}

Возвращает значение, указывающее, равен ли данный экземпляр указанному экземпляру класса [`ResourceAssignment`](../).

```csharp
public bool Equals(ResourceAssignment other)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| other | ResourceAssignment | Указанный экземпляр класса [`ResourceAssignment`](../), с которым сравнивается данный экземпляр. |

### Возвращаемое значение

**True** if the specified instance of the [`ResourceAssignment`](../) class has the same UID value as this instance; otherwise, **false**.

## Примеры

Показывает, как проверить равенство назначений ресурсов.

```csharp
var project = new Project(DataDir + "BaselineTD2010_3.mpp");

var resourceAssignment1 = project.ResourceAssignments.GetByUid(1);
var resourceAssignment2 = project.ResourceAssignments.GetByUid(1);

Console.WriteLine("Are resource assignments equal: " + resourceAssignment1.Equals(resourceAssignment2));
```

### См. также

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
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

**True** if o is a ResourceAssignment that assign the same resource and task as this instance; otherwise, **false**.

## Примеры

Показывает, как проверить равенство назначений ресурсов.

```csharp
var project = new Project(DataDir + "BaselineTD2010_3.mpp");

var resourceAssignment1 = project.ResourceAssignments.GetByUid(1);
var resourceAssignment2 = project.ResourceAssignments.GetByUid(1);

Console.WriteLine("Are resource assignments equal: " + resourceAssignment1.Equals(resourceAssignment2));
```

### См. также

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)



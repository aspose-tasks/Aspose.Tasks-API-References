---
title: "VbaModuleAttribute.Equals"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод VbaModuleAttribute. Возвращает значение, указывающее, равен ли данный экземпляр указанному объекту VbaModuleAttribute"
type: docs
weight: 30
url: /ru/net/aspose.tasks/vbamoduleattribute/equals/
---
## Equals(VbaModuleAttribute) {#equals}

Возвращает значение, указывающее, равен ли данный экземпляр указанному объекту [`VbaModuleAttribute`](../).

```csharp
public bool Equals(VbaModuleAttribute other)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| other | VbaModuleAttribute | Указанный объект [`VbaModuleAttribute`](../) для сравнения с этим экземпляром. |

### Возвращаемое значение

Возвращает true, если данный экземпляр равен указанному объекту [`VbaModuleAttribute`](../); в противном случае — false.

## Примеры

Показывает, как проверить равенство атрибутов модуля VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");
var module = project.VbaProject.Modules.ToList()[0];

var attribute1 = module.Attributes.ToList()[0];
var attribute2 = module.Attributes.ToList()[0];
Console.WriteLine("Module attribute 1 Key: {0}, Value: {1}", attribute1.Key, attribute1.Value);
Console.WriteLine("Module attribute 2 Key: {0}, Value: {1}", attribute2.Key, attribute2.Value);
Console.WriteLine("Are module attributes equal: " + attribute1.Equals(attribute2));
```

### См. также

* class [VbaModuleAttribute](../)
* namespace [Aspose.Tasks](../../vbamoduleattribute/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

Возвращает значение, указывающее, равен ли данный экземпляр указанному объекту [`VbaModuleAttribute`](../).

```csharp
public override bool Equals(object obj)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| obj | Object | Указанный объект [`VbaModuleAttribute`](../) для сравнения с этим экземпляром. |

### Возвращаемое значение

Возвращает true, если данный экземпляр равен указанному объекту [`VbaModuleAttribute`](../); в противном случае — false.

## Примеры

Показывает, как проверить равенство атрибутов модуля VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");
var module = project.VbaProject.Modules.ToList()[0];

var attribute1 = module.Attributes.ToList()[0];
var attribute2 = module.Attributes.ToList()[0];
Console.WriteLine("Module attribute 1 Key: {0}, Value: {1}", attribute1.Key, attribute1.Value);
Console.WriteLine("Module attribute 2 Key: {0}, Value: {1}", attribute2.Key, attribute2.Value);
Console.WriteLine("Are module attributes equal: " + attribute1.Equals(attribute2));
```

### См. также

* class [VbaModuleAttribute](../)
* namespace [Aspose.Tasks](../../vbamoduleattribute/)
* assembly [Aspose.Tasks](../../../)



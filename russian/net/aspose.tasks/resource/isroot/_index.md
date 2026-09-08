---
title: "Resource.IsRoot"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство Resource. Получает флаг, указывающий, является ли ресурс корневым ресурсом. Корневой ресурс — это специальный ресурс, предназначенный для поддержки внутренностей форматов MS Projects и не предназначен для прямого использования в коде пользователя."
type: docs
weight: 470
url: /ru/net/aspose.tasks/resource/isroot/
---
## Resource.IsRoot property

Получает флаг, указывающий, является ли ресурс корневым ресурсом. Корневой ресурс — это специальный ресурс, предназначенный для поддержки внутренностей форматов MS Project и не предназначенный для прямого использования в коде пользователя.

```csharp
public virtual bool IsRoot { get; }
```

## Примеры

Показывает, как использовать свойство IsRoot для пропуска корневого ресурса.

```csharp
var project = new Project(DataDir + "ResourceCosts.mpp");

foreach (var resource in project.Resources)
{
    if (resource.IsRoot)
    {
        continue;
    }

    Console.WriteLine(resource.Get(Rsc.Name));
}
```

### См. также

* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)



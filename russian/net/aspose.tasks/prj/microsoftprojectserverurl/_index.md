---
title: "Prj.MicrosoftProjectServerURL"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Prj. Определяет, был ли проект создан пользователем Project Server, а не пользователем NT"
type: docs
weight: 460
url: /ru/net/aspose.tasks/prj/microsoftprojectserverurl/
---
## Prj.MicrosoftProjectServerURL field

Определяет, был ли проект создан пользователем Project Server, а не пользователем NT.

```csharp
public static readonly Key<NullableBool, PrjKey> MicrosoftProjectServerURL;
```

## Примеры

Показывает, как читать/записывать свойство Prj.MicrosoftProjectServerURL.

```csharp
var project = new Project();

project.Set(Prj.MicrosoftProjectServerURL, true);

Console.WriteLine("Microsoft Project Server U R L: " + project.Get(Prj.MicrosoftProjectServerURL));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)



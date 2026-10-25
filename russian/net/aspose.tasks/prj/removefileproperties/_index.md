---
title: "Prj.RemoveFileProperties"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Prj. Определяет, будут ли все свойства файлов удаляться при сохранении"
type: docs
weight: 600
url: /ru/net/aspose.tasks/prj/removefileproperties/
---
## Prj.RemoveFileProperties field

Определяет, будут ли все свойства файла удалены при сохранении.

```csharp
public static readonly Key<NullableBool, PrjKey> RemoveFileProperties;
```

## Примеры

Показывает, как читать/записывать свойство Prj.RemoveFileProperties.

```csharp
var project = new Project();

project.Set(Prj.RemoveFileProperties, true);

Console.WriteLine("Remove File Properties: " + project.Get(Prj.RemoveFileProperties));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)



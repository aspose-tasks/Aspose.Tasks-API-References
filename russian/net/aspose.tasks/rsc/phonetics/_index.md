---
title: "Rsc.Phonetics"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Rsc. Фонетическое написание имени ресурса. Только для японского языка"
type: docs
weight: 560
url: /ru/net/aspose.tasks/rsc/phonetics/
---
## Rsc.Phonetics field

Фонетическое написание имени ресурса. Только для использования с японским языком.

```csharp
public static readonly Key<string, RscKey> Phonetics;
```

## Примеры

Показывает, как читать/записывать свойство Rsc.Phonetics.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Phonetics, "Phonetics");

Console.WriteLine("Phonetics: " + resource.Get(Rsc.Phonetics));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


